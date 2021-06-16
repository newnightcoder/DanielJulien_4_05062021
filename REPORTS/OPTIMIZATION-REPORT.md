# :chart_with_upwards_trend:&nbsp; <ins>RAPPORT D'OPTIMISATION</ins>

## AVANT / APRÈS &nbsp;(**10 RECOMMANDATIONS**)

### :mag_right:&nbsp; <ins>**SEO**</ins>

- [x] Balise `meta` "description" à renseigner
- [x] Fournir un titre optimal à la balise `<title>`
- [x] Menu / barre de navigation

### :wheelchair:&nbsp; <ins>**ACCESSIBILITÉ**</ins>

- [x] Renseigner un language pour l'attribut `lang`
- [x] Respecter la hiérarchisation du _heading_ (pas de `<h3>`au lieu de `<h2>` etc..)
- [x] font-size trop petite
- [x] images-texte un peu partout dans le document
- [ ] problèmes de contraste de certains éléments

### :rocket:&nbsp; <ins>**PERFORMANCE**</ins>

- [x] format et taille incorrects des images (taille des images, format .bmp)
- [ ] fichiers JS et CSS non minifiés

### 🔴&nbsp; **LIGHTHOUSE REPORT AVANT CORRECTION**

<img src="img/lighthouse-before.png" height="120" width="320"/>

---

<h1 align="center">🔍 <ins>SEO</ins></h1>

### 1 - <ins>DESCRIPTION DU SITE</ins>

:poop:&nbsp; **Balise `meta` description vide.**

<img src="img/code-meta-before1.png" height="20" />&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : petit texte de description pour l'attribut `content`

<img src="img/code-meta-after1.png" height="85"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +10pts score SEO sur l'audit _Lighthouse_ (de 80% à 90%)

<img src="img/lighthouse-meta-after.png" height="120" width="330"/>

---

### 2 - <ins>TITRE DU SITE</ins>

:poop:&nbsp; **Balise `title` vide.**

<img src="img/code-title-before.png" height="35"/> _NB : mettre un `.` dans `title` ne permettra pas d'être trouvé dans les moteurs de recherche_

:construction:&nbsp; <ins>**Correction**</ins> : titre fourni (nécessaire pour indexer la page correctement) :

<img src="img/code-title-after.png" height="35"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : score SEO à 100% sur l'audit _Lighthouse_!

<img src="img/lighthouse-title-after.png" height="120" width="330"/>

**\_NB : <ins>le titre est AUSSI très important pour l'accessibilité</ins>.  
En effet le titre contenu dans `<title>`est nécessaire pour les screen-readers qui le liront à l'utilisateur. Bien renseigner la balise `<title>` améliore donc non seulement le SEO mais aussi l'accessibilité du site.
Suite à la correction, on gagne +5pts en Accessibilité sur l'audit _Lighthouse_! (de 81% à 86%).**

<img src="img/lighthouse-title-after.png" height="120" width="330"/>

---

### 3 - <ins>NAVIGATION / MENU</ins>

:poop:&nbsp; **Navigation / menu peu clair.**

- sur la page d'accueil:

  <img src="img/navbar-index-before.png" height="35"/>&nbsp;

- sur la page contact:

  <img src="img/navbar-page2-before.png" height="45"/>&nbsp;

- présence de `<div>` cachées contenant des mots-clés afin d'améliorer le référencement (attention: très mauvaise pratique, condamnée par Google! Donc aucune chance d'améliorer le référencement de cette façon.)

  <img src="img/div-keywords-code.png" height="45"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> :

- réorganisation et renommage des liens dans la `<navbar>`
- corrections des erreurs (liens css erronés) sur la page2.html
- suppression des `<div class="keywords">`
- ajout d'indice visuel lors du survol et focus des liens du menu (:wheelchair:)
- texte `alt` amélioré pour l'image du logo du site (:wheelchair:)&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : le menu `<navbar>` est maintenant beaucoup plus clair/explicite (pour améliorer le <ins>SEO</ins>) et aussi plus facilement compréhensible pour les utilisateurs (<ins>accessibilité</ins> améliorée).

<img src="img/navbar-after.png" height="45"/>

**_NB : en corrigeant les erreurs sur la page contact (page2.html), la mise en page de toute la page à été débuggée pour obtenir le layout voulu au départ :_**

<ins>AVANT</ins> <img src="img/page2-before.png" height="300"/> <ins>APRÈS</ins> <img src="img/page2-after.png" height="300"/>&nbsp;

---

<h1 align="center">♿ <ins>ACCESSIBILITÉ</ins></h1>

### 4 - <ins>LANGUE DU SITE</ins>

:poop:&nbsp; **Attribut `lang` incorrect.**
L'attribut `lang` est défini sur "Default", valeur qui n'existe pas. Il faut choisir le language adapté au site, ici le français.

<img src="img/code-lang-before.png" height="55"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : modification de l'attribut `lang` avec une valeur valide (nécessaire pour les screen-reader) :

<img src="img/code-lang-after.png" height="55"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +5pts Accessibility sur l'audit _Lighthouse_ (de 76% à 81%)

<img src="img/lighthouse-lang-after.png" height="120" width="330"/>

---

### 5 - <ins>HIÉRARCHISATION DES TITRES DANS LA PAGE</ins>

:poop:&nbsp; **Non-respect de la hiérarchisation du _heading_.**  
Ne pas utiliser de `<h3>` en l'absence de `<h2>` dans le même bloc.

<img src="img/code-h3-before.png" height="95"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : tous les `<h3>` sont remplacés par des `<h2>` :

<img src="img/code-h3-after.png" height="95"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +4pts Accessibility (de 86% à 90%)

<img src="img/lighthouse-h3-after.png" height="120" width="330"/> &nbsp;

**_NB : pour aller plus loin et dans le sens d'une bonne hiérarchisation / structuration du code html de la page, il serait bon d'utiliser certaines balises sémantiques comme `header`, `section`, `footer`etc... Mais le sujet ne sera pas abordé dans ce rapport, on focalise ici sur les 10 points les plus importants._**

---

### 6 - <ins>TAILLE DE LA POLICE</ins>

:poop:&nbsp; **Taille de police des paragraphes trop petite.**  
Les paragraphes de description contenus dans chacun des blocs de la pages sont difficiles à lire car trop petits.

<img src="img/code-p-before.png" height="55"/>&nbsp;
<img src="img/p-before.png" height="130"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : augmenter la taille de la police (entre 14px et 16px):

<img src="img/code-p-after.png" height="55"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : les paragraphes sont lisibles correctement, sans effort.

<img src="img/p-after.png" height="155" />

---

### 7 - <ins>TEXTES</ins>

:poop:&nbsp; **Utilisation d'images pour afficher du texte.**  
Certains textes sont sous forme d'image (ne peuvent être lus par les screenreader + impossible à crawler/indexer).

<img src="img/code-img-text-before1.png" height="100"/>&nbsp;
<img src="img/img-text-before.png" height="130"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : remplacement des images par du texte sous forme de `<h2>`, `<p>` ou `<span>` selon les situations:

<img src="img/code-img-text-after1.png" height="100"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : tous les textes affichés sur le site peuvent être lus par les screenreaders + crawlés et indexés par Googlebot.

<img src="img/img-text-after.png" height="150" width="330"/>&nbsp;

_NB : à l'occasion de cette correction, le background du bloc-4 (lignes horizontales) a été remplacé par un fond blanc simple. Cela augmente la lisibilité des textes._

<ins>AVANT</ins> <img src="img/bg-lines-before.png" height="230" width="330"/> <ins>APR&Egrave;S</ins> <img src="img/bg-lines-after.png" height="230" width="330"/>&nbsp;

---

<h1 align="center"> 🚀 <ins>PERFORMANCE</ins></h1>

### 8 - <ins>TAILLE DES IMAGES</ins>

:poop:&nbsp; **Taille et format incorrects pour les images.**  
Les images utilisées ne sont pas à la bonne taille ou au au bon format pour le web. Soit trop grandes comparées à leur conteneur/CSS, soit au format `.bmp` (ou `.jpeg` pour le favicon), formats non optimaux pour le web.

<img src="img/img-size-before1.png" height="100"/> <img src="img/img-size-before2.png" height="130"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> :

- images redimensionnées à 270px (taille du conteneur)
- attributs `width` et `height` stipulés dans le html
- formats `.bmp` et `jpeg` remplacés par `.png` (favicon et images de la section portfolio)

<!-- <img src="img/code-img-text-after1.png" height="100"/>&nbsp; -->

:rocket:&nbsp; <ins>**Amélioration**</ins> : on gagne en **taille (-0.4MB)** et en **rapidité(-0.5s)** d'affichage, d'après l'outil _Network_ des DevTools (Chrome):

<ins>AVANT / APR&Egrave;S</ins> :

<img src="img/network-img-before.png" height="30" width="600"/>

<img src="img/network-img-after.png" height="30" width="600"/>&nbsp;

<ins>Audit Lighthouse</ins> : on gagne +3pts en _Performance_ et +4pts en _Best Practices_!

<img src="img/lighthouse-img-after.png" height="120" width="320"/>&nbsp;

**_NB : à l'occasion de cette correction, certains détails liés à la <ins>responsivité du site</ins> ont aussi été corrigés :_**
_- images de la section portfolio centrées sur l'écran (au lieu d'être alignées à gauche)_
_- div "social" du footer qui contient les icônes réseaux sociaux : `display = flex` au lieu de `block` (colonne)_

<ins>AVANT</ins> <img src="img/responsive-img-before.png" height="230" width="150"/> <ins>APR&Egrave;S</ins> <img src="img/responsive-img-after.png" height="230" width="150"/>

<ins>AVANT</ins> <img src="img/footer-before.png" height="75" width="150"/> <ins>APR&Egrave;S</ins> <img src="img/footer-after.png" height="60" width="150"/>

---

### 9 - <ins>CHARGEMENT ET OPTIMISATION DES FICHIERS</ins>

:poop:&nbsp; **Scripts bloquants et fichiers non minifiés.**  
Les scripts JS bloquent le html parsing et les fichiers JS et CSS ne sont pas minifiés.&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> :

- ajout de l'attribut `defer` pour les scripts de librairies afin qu'ils ne bloquent pas le parsing du html
- minification des fichiers CSS et JS avec l'extension _Minifier_ de Vscode
- préchargement des polices

:rocket:&nbsp; <ins>**Amélioration**</ins> :

- on gagne au minimum +2pts en Performance sur l'audit _Lighthouse_ (de 92 à 94%):

<img src="img/lighthouse-min-after.png" height="120" width="320"/>&nbsp;

- on gagne en poids total des ressources du site d'après l'outil _Network_ de DevTools (sous la barre des 2MB):

<img src="img/network-min-after.png" height="30" width="280"/>&nbsp;

---

Errors report is available [here](ERRORS.md).  
Go back to [README](../README.md).
