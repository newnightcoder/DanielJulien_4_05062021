# :chart_with_upwards_trend:&nbsp; <ins>RAPPORT D'OPTIMISATION</ins>

## AVANT / APRÈS &nbsp;(**10 RECOMMANDATIONS**)

### :mag_right:&nbsp; <ins>**SEO**</ins>

- [x] Balise `meta` "description" à renseigner
- [x] Fournir un titre optimal à la balise `<title>`
- [ ] menu / barre de navigation :
  - [ ] pas assez clair : lien vers page2 mal nommé
  - [ ] problème de dimensions de la navbar sur la page2
  - [ ] `<button>`"toggle navigation" inutile / pas clair
  - [ ] les `<div class="keywords">` sont totalement inutiles (mauvaise pratique)

### :wheelchair:&nbsp; <ins>**ACCESSIBILITÉ**</ins>

- [x] Renseigner un language pour l'attribut `lang`
- [x] Fourir un titre à la balise `<title>`
- [x] Respecter la hiérarchisation du _heading_ (pas de `<h3>`au lieu de `<h2>` etc..)
- [x] font-size trop petite
- [x] images-texte un peu partout dans le document

### :rocket:&nbsp; <ins>**PERFORMANCE**</ins>

- [ ] scripts à charger en `defer`ou `async`
- [ ] format et taille incorrects des images

### 🔴&nbsp; **LIGHTHOUSE REPORT AVANT CORRECTION**

<img src="img/lighthouse-before.png" height="120" width="320"/>

---

<h1 align="center">🔍 <ins>SEO</ins></h1>

### 1 - <ins>DESCRIPTION DU SITE</ins>

:poop:&nbsp; **Balise `meta` description vide :**

<img src="img/code-meta-before1.png" height="20" />&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : petit texte de description pour l'attribut `content`

<img src="img/code-meta-after1.png" height="85"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +10pts score SEO (de 80% à 90%)

<img src="img/lighthouse-meta-after.png" height="120" width="330"/>

---

### 2 - <ins>TITRE DU SITE</ins> (SEO)

:poop:&nbsp; **Balise `title` vide :**

<img src="img/code-title-before.png" height="35"/> _NB : mettre un `.` dans `title` ne permettra pas d'être trouvé dans les moteurs de recherche_

:construction:&nbsp; <ins>**Correction**</ins> : titre fourni (nécessaire pour indexer la page correctement) :

<img src="img/code-title-after.png" height="35"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : score SEO à 100% sur l'audit Lighthouse!

<img src="img/lighthouse-title-after.png" height="120" width="330"/>

**_NB : <ins>le titre est aussi très important pour l'accessibilité</ins>.  
En effet le titre contenu dans `<title>`est nécessaire pour les screen-reader qui le liront à l'utilisateur. Bien renseigner la balise `<title>` améliore donc non seulement le SEO mais aussi l'accessibilité du site.
Suite à la correction, on gagne +5pts en Accessibilité! (de 81% à 86%)._**
<img src="img/lighthouse-title-after.png" height="120" width="330"/>

---

<h1 align="center">♿ <ins>ACCESSIBILITÉ</ins></h1>

### 3 - <ins>LANGUE DU SITE</ins>

:poop:&nbsp; **Attribut `lang` incorrect :**

<img src="img/code-lang-before.png" height="55"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : modification de l'attribut `lang` avec une valeur valide (nécessaire pour les screen-reader) :

<img src="img/code-lang-after.png" height="55"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +5pts Accessibility (de 76% à 81%)

<img src="img/lighthouse-lang-after.png" height="120" width="330"/>

---

### 4 - <ins>HIÉRARCHISATION DES TITRES DANS LA PAGE</ins>

:poop:&nbsp; **Respect de la hiérarchisation du _heading_ :** ne pas utiliser de `<h3>` en l'absence de `<h2>` dans le même bloc.

<img src="img/code-h3-before.png" height="95"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : tous les `<h3>` sont remplacés par des `<h2>` :

<img src="img/code-h3-after.png" height="95"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : +4pts Accessibility (de 86% à 90%)

<img src="img/lighthouse-h3-after.png" height="120" width="330"/>

---

### 5 - <ins>TAILLE DE LA POLICE</ins>

:poop:&nbsp; **Taille de police des paragraphes trop petite:** les textes sont difficiles à lire.

<img src="img/code-p-before.png" height="55"/>&nbsp;
<img src="img/p-before.png" height="130"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : augmenter la taille de la police (entre 14px et 16px):

<img src="img/code-p-after.png" height="55"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : les paragraphes sont lisibles correctement, sans effort.

<img src="img/p-after.png" height="155" />

---

### 6 - <ins>TEXTES</ins>

:poop:&nbsp; **Utilisation d'images pour afficher du texte:** certains textes sont sous forme d'image (ne peuvent être lus par les screenreader + impossible à crawler/indexer).

<img src="img/code-img-text-before1.png" height="100"/>&nbsp;
<img src="img/img-text-before.png" height="130"/>&nbsp;

:construction:&nbsp; <ins>**Correction**</ins> : remplacement des images par du texte sous forme de `<h2>`, `<p>` ou `<span>` selon les situations:

<img src="img/code-img-text-after1.png" height="100"/>&nbsp;

:rocket:&nbsp; <ins>**Amélioration**</ins> : tous les textes affichés sur le site peuvent être lus par les screenreaders + crawlés et indexés par Googlebot.

<img src="img/img-text-after.png" height="150" width="330"/>&nbsp;

_NB : à l'occasion de cette correction, le background du bloc-4 (lignes horizontales) a été remplacé par un fond blanc simple. Cela augmente la lisibilité des textes._

AVANT <img src="img/bg-lines-before.png" height="230" width="330"/> APR&Egrave;S <img src="img/bg-lines-after.png" height="230" width="330"/>&nbsp;

---

<h1 align="center"> 🚀 <ins>PERFORMANCE</ins></h1>

---

Errors report is available [here](ERRORS.md).  
Go back to [README](../README.md).
