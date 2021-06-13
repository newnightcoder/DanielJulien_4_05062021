# :chart_with_upwards_trend:&nbsp; <ins>RAPPORT D'OPTIMISATION</ins>

## AVANT / APRÈS

**10 RECOMMANDATIONS**

:mag_right:&nbsp;<ins>**SEO**</ins>

- [x] Balise `meta` "description" à renseigner
- [x] Fournir un titre optimal à la balise `<title>`

:wheelchair:&nbsp;<ins>**Accessibilité**</ins>

- [x] Renseigner un language pour l'attribut `lang`
- [x] Fourir un titre à la balise `<title>`
- [x] Respecter la hiérarchisation du _heading_ (pas de `<h3>`au lieu de `<h2>` etc..)

:rocket:&nbsp;<ins>**Performance**</ins>

**LIGHTHOUSE REPORT AVANT CORRECTION**

<img src="img/lighthouse-before.png" height="120" width="320"/>

---

<h1 align="center">🔍 <ins>SEO</ins></h1>

:poop:&nbsp; **Balise `meta` description vide :**

<img src="img/code-meta-before1.png" height="20" />&nbsp;

:construction:&nbsp; **Correction** : petit texte de description pour l'attribut `content`

<img src="img/code-meta-after1.png" height="85"/>&nbsp;

:rocket:&nbsp; **Amélioration** : +10pts score SEO (de 80% à 90%)

<img src="img/lighthouse-meta-after.png" height="120" width="330"/>

---

:poop:&nbsp; **Balise `title` vide :**

<img src="img/code-title-before.png" height="35"/>

_NB : mettre un `.` dans `title` ne permettra pas d'être trouvé dans les moteurs de recherche_

:construction:&nbsp; **Correction** : titre fourni (nécessaire pour indexer la page correctement) :

<img src="img/code-title-after.png" height="35"/>&nbsp;

:rocket:&nbsp; **Amélioration** : score SEO à 100% sur l'audit Lighthouse!

<img src="img/lighthouse-title-after.png" height="120" width="330"/>

---

<h1 align="center">♿ <ins>ACCESSIBILITÉ</ins></h1>

:poop:&nbsp; **Attribut `lang` incorrect :**

<img src="img/code-lang-before.png" height="55"/>&nbsp;

:construction:&nbsp; **Correction** : modification de l'attribut `lang` avec une valeur valide (nécessaire pour les screen-reader) :

<img src="img/code-lang-after.png" height="55"/>&nbsp;

:rocket:&nbsp; **Amélioration** : +5pts Accessibility (de 76% à 81%)

<img src="img/lighthouse-lang-after.png" height="120" width="330"/>

---

:poop:&nbsp; **Balise `title` vide :**

<img src="img/code-title-before.png" height="35"/>

_NB : mettre un `.` dans `title` revient à ne rien écrire puisque le `.` ne fournit rien au screenreader_

:construction:&nbsp; **Correction** : titre fourni (nécessaire pour les screen-reader) :

<img src="img/code-title-after.png" height="35"/>&nbsp;

:rocket:&nbsp; **Amélioration** : +5pts Accessibility (de 81% à 86%)

<img src="img/lighthouse-title-after.png" height="120" width="330"/>

---

:poop:&nbsp; **Respect de la hiérarchisation du _heading_ :**
Ne pas utiliser de `<h3>` en l'absence de `<h2>` dans le même bloc.

<img src="img/code-h3-before.png" height="95"/>&nbsp;

:construction:&nbsp; **Correction** : tous les `<h3>` sont remplacés par des `<h2>` :

<img src="img/code-h3-after.png" height="95"/>&nbsp;

:rocket:&nbsp; **Amélioration** : +4pts Accessibility (de 86% à 90%)

<img src="img/lighthouse-h3-after.png" height="120" width="330"/>

---

<h1 align="center"> 🚀 <ins>PERFORMANCE</ins></h1>

---

Errors report is available [here](ERRORS.md).  
Go back to [README](../README.md).
