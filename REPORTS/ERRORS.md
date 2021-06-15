# :memo:&nbsp; <ins>RAPPORT D'ERREURS</ins>

## MAUVAISES PRATIQUES

### <ins>HTML</ins>

**:mag_right:&nbsp; SEO**

- [x] valeur invalide pour l'attribut `lang`
- [x] balises `meta` :

  - [x] `meta` "description": contenu vide
  - [ ] `meta` "keywords": contenu trop vague / répétitif --> pas grave, meta non prise en charge par la majorités des navigateurs

- [x] le titre du site `<title>` est vide
- [ ] structure du document non optimale: absences de balises sémantiques
- [ ] menu / barre de navigation :
  - [ ] pas assez clair : lien vers page2 mal nommé
  - [ ] problème de dimensions de la navbar sur la page2
  - [ ] `<button>`"toggle navigation" inutile / pas clair
  - [ ] les `<div class="keywords">` sont totalement inutiles (mauvaise pratique)
- [ ] attribut `href`: pas de protocole http pour les liens externes (footer)
      <br></br>

**:wheelchair:&nbsp; ACCESSIBILITÉ**

- [x] le titre du site `<title>` est vide
- [x] hiérarchisation érronée du heading: utilisation de `<h3>` au lieu de `<h2>`
- [x] images-texte un peu partout dans le document
- [ ] texte `alt` pour les img: trop long / non descriptif de l'img
- [x] font-size trop petite
- [ ] contraste texte/couleurs incorrect bloc-1, bloc-3, bloc-5
- [x] fond rayé du bloc-4
      <br></br>

**:rocket:&nbsp; PERFORMANCE**

- [ ] scripts à charger en `defer`ou `async`
- [ ] format img incorrect (taille des images, format .bmp)
- [ ] pas de `<li>` vide dans une `<ul>`
- [ ] css: trop de sélecteurs / sélecteurs inutilisés
- [ ] css: problème avec les media queries
- [ ] erreur dans la console au chargement de la page  
       <br></br>

## :ledger:&nbsp; <ins>TABLEAU D'ANALYSE</ins>

| Categorie    | Problème                                        | Description                                            | Bonne pratique                          | Action recommendée |
| ------------ | ----------------------------------------------- | ------------------------------------------------------ | --------------------------------------- | ------------------ |
| :mag_right:  | `meta` "keywords"                               | contenu trop vague / répétitif                         |
| :mag_right:  | `meta` "description"                            | contenu vide                                           |
| :mag_right:  | balise `<title>`                                |                                                        | toujours renseigner le titre de la page |
| :wheelchair: | texte `alt` pour les img                        | trop long / non descriptif de l'img                    |
| :wheelchair: | font-size trop petite                           | `<p>` font-size trop petite / difficile à lire         |
| :wheelchair: | contraste couleurs incorrect                    | contraste insuffisant du texte sur les images          |
| :rocket:     | trop de scripts à charger                       | le chargement des librairies bloque le parsing du html |
| :rocket:     | html non utilisé                                | `<li>` vides dans une `<ul>`                           |
| :rocket:     | hierarchie heading incorrecte                   | utilisation de `<h3>` au lieu de `<h2>`                |
| :rocket:     | css: problème avec les media queries            |
|              | css: trop de sélecteurs / sélecteurs inutilisés |
|              | `href` incorrect dans les liens                 | pas de protocole http pour les liens externes          |

<br></br>

Optimization report [here](OPTIMIZATION-REPORT.md).  
Go back to [README](../README.md).
