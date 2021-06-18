# :memo:&nbsp; <ins>RAPPORT D'ERREURS</ins>

## MAUVAISES PRATIQUES

### :mag_right:&nbsp; SEO

- [x] valeur invalide pour l'attribut `lang`
- [x] balises `meta` :

  - [x] `meta` "description": contenu vide
  - [ ] `meta` "keywords": contenu trop vague / répétitif --> pas grave, meta non prise en charge par la majorités des navigateurs

- [x] le titre du site `<title>` est vide
- [ ] structure syntaxique du document non optimale: absences de balises sémantiques
- [x] menu / barre de navigation :
  - [x] pas assez clair : lien vers page2 mal nommé
  - [x] problème de dimensions de la navbar sur la page2
  - [x] `<button>`"toggle navigation" inutile / pas clair
  - [x] les `<div class="keywords">` sont totalement inutiles (mauvaise pratique)
- [x] hiérarchisation érronée du heading: utilisation de `<h3>` au lieu de `<h2>`
- [ ] attribut `href`: pas de protocole http pour les liens externes (footer)
      <br></br>

### :wheelchair:&nbsp; ACCESSIBILITÉ

- [x] le titre du site `<title>` est vide
- [x] images-texte un peu partout dans le document
- [x] texte `alt` pour les img: trop long / non descriptif de l'img
- [x] font-size trop petite
- [ ] contraste texte/couleurs incorrect bloc-1, bloc-3, bloc-5
- [x] fond rayé du bloc-4
      <br></br>

### :rocket:&nbsp; PERFORMANCE

- [x] scripts bloquent le parsing du html
- [x] fichiers JS et CSS non minifiés
- [x] format img incorrect (taille des images, format .bmp)
- [ ] pas de `<li>` vide dans une `<ul>`
- [ ] css: trop de sélecteurs / sélecteurs inutilisés
- [ ] css: problème avec les media queries
- [x] erreur dans la console au chargement de la page  
       <br></br>

## :ledger:&nbsp; <ins>TABLEAU D'ANALYSE</ins>

|     Type     | Problème                                     | Description                                                                                                                                                         | Bonne pratique                                                                                                                                                                                                                                                         | Action recommendée                                                                                                             |
| :----------: | -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
|              |
| :mag_right:  | Balise `meta` _description_                  | son contenu est vide                                                                                                                                                | toujours renseigner la balise `meta` description en quelques mots clés, sous forme de courte présentation. [(référence)]()                                                                                                                                             | écrire une courte présentation de la Choutte agence.                                                                           |
| :mag_right:  | Balise `<title>`                             | son contenu est vide (contient juste un `.`)                                                                                                                        | toujours renseigner le titre de la page. [(référence)]()                                                                                                                                                                                                               | renseigner le titre du site (_La chouette agence_ par exemple)                                                                 |
| :mag_right:  | Structure syntaxique du document             | absence de balises syntaxiques décrivant la structure du document. Le document est une succession de `div`                                                          | utiliser les balises sémantiques appropriées comme `header`,`section`, `footer` etc..., pour indiquer au navigateur la structure de la page. [(référence)]()                                                                                                           | remplacer les `div class="bloc"` par des `section`, utiliser `footer` pour le bloc footer, `header` pour le bloc header etc... |
| :mag_right:  | Menu / barre de navigation                   | navigation peu claire et mal dimensionnée                                                                                                                           | toujours s'assurer que la barre de navigation est claire et bien structurée (très important niveau SEO mais accessibilité aussi). [(référence)]()                                                                                                                      | réorganiser et redimensionner la barre de navigation avec des noms de liens clairs (_Accueil_, _Réalisations_, _Contact_)      |
| :mag_right:  | `<div class="keywords">`                     | plusieurs `div` cachées contiennent des mots-clés censés améliorer le référencement. Cette pratique est contreproductive car condamnée par Google suite aux abus.   | ne JAMAIS utiliser de texte caché dans le document pour booster le SEO. [(référence)]()                                                                                                                                                                                | supprimer toutes ces `div class="keywords"` et focaliser sur les autres aspects SEO (`meta` description, `title` etc...).      |
| :mag_right:  | Hiérarchie du _heading_ incorrecte           | utilisation de `<h3>` au lieu de `<h2>`                                                                                                                             | respecter la hiérarchisation du _heading_ (utilisation des balises `<h2>`, `<h3>` etc... [(référence)]())                                                                                                                                                              | remplacer tous les `<h3>` par des `<h2>` là où nécessaire                                                                      |
|              |                                              |
| :wheelchair: | Attribut `lang`                              | l'attribut contient la valeur `Default`, invalide                                                                                                                   | toujours renseigner l'attribut `lang` avec une valeur valide. [(référence)]()                                                                                                                                                                                          | corriger la valeur de `Default` à `fr`                                                                                         |
| :wheelchair: | Images-texte un peu partout dans le document | des images sont utilisées pour afficher du texte. Cela réduit considérablement l'accessibilité du site (auvais impact sur le référencement et la performance aussi) | écrire le texte autre que logo ou header avec du texte html et non des images. [(référence)]()                                                                                                                                                                         | remplacer les images par du texte contenu dans un `<p>` ou autre                                                               |
| :wheelchair: | Texte `alt` pour les img                     | trop long / non descriptif de l'img, utlisé pour le référencement en utilisant des mots clés                                                                        | le texte `alt` doit contenir une description de l'image (elle s'affichera si l'image ne charge pas et sera lue par les screen-readers pour les personnes en situation de handicap). [(référence)]()                                                                    | réécrire les textes alternatifs des images du site                                                                             |
| :wheelchair: | Font-size trop petite                        | `<p>` font-size trop petite / difficile à lire                                                                                                                      | utiliser une taille de police lisible par tous. [(référence)]()                                                                                                                                                                                                        | changer la `font-size` de 11px à 14-16px                                                                                       |
| :wheelchair: | Contraste couleurs incorrect                 | contraste insuffisant du texte sur background image ou couleur                                                                                                      | s'assurer que les contrastes textes/couleurs sont suffisants grâce aux outils de vérification de l'accessibilité. [(référence)]()                                                                                                                                      | corriger les erreurs de contrastes avec l'outil WCAG - _Web Content Accessibility Guidelines_ par exemple                      |
|              |                                              |
|   :rocket:   | Scripts bloquants                            | le chargement des librairies bloque le parsing du html                                                                                                              | charger les scripts en `defer` ou `async` afin de ne pas interrompre le parsing html. [(référence)]()                                                                                                                                                                  | ajout de l'attribut `defer` dans les `<script>` qui chargent les librairies JS                                                 |
|   :rocket:   | Taille et format des images                  | Les images sont trop grandes par rapport à leurs conteneurs / leur format n'est pas optimisé pour le web                                                            | dimensionner les images préalablement, afin qu'elles soient à la taille de leur conteneur sur le site (ou prévoir plusieurs tailles d'image en fonction des apareils et utiliser les attribut `srcset` et `sizes`) + les sauvergarder à un format optimisé pour le web | redimensionner les images et les sauvegarder au format `.png` voire `WebP`. [(référence)]()                                    |
|   :rocket:   | HTML non utilisé                             | `<li>` vides dans une `<ul>`                                                                                                                                        | pas d'éléments vides ou inutilisé dans la page. Cela ralentit le parsing inutilement et nous dessert en terme de SEO. [(référence)]()                                                                                                                                  | supprimer les éléments vides ou inutilisés                                                                                     |
|   :rocket:   | CSS non utilisé                              | beaucoup trop de sélecteurs inutilisés                                                                                                                              | utiliser les sélecteurs nécessaires en étant le plus _spécifique_ possible. [(référence)]()                                                                                                                                                                            | supprimer les classes (html) ainsi que les sélecteurs (stylesheet) inutilisés                                                  |
|   :rocket:   | CSS: problème avec les media queries         | certaines syntaxes sont erronées: `min-device-width` et `max-device-width` sont dépréciées et à ne plus utiliser + `-webkit-device-pixel-ratio` est non standard    | utiliser `min-width` et `max-width` + `resolution` [(référence)](https://developer.mozilla.org/fr/docs/Web/CSS/@media/-webkit-device-pixel-ratio)                                                                                                                      | correction des media-queries avec `min-width`, `max-width` et `resolution`                                                     |
|   :rocket:   | `href` incorrect dans les liens              | pas de protocole http pour les liens externes                                                                                                                       |
|   :rocket:   | fichiers non minifiés                        | les fichiers non minifiés etraînent une ralentissement du temps de chargement de la page                                                                            | minifier les fichiers CSS et JS (nombreux outils disponibles) ou utiliser un bundler. [(référence)]()                                                                                                                                                                  | minification des fichiers CSS et JS (avec minifier extension Vscode par exemple)                                               |

<br></br>

OPTIMIZATION REPORT [HERE](OPTIMIZATION-REPORT.md).  
BACK TO [README](../README.md).
