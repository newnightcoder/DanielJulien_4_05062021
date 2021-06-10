# :memo:&nbsp; <ins>RAPPORT D'ERREURS</ins>

## MAUVAISES PRATIQUES

### <ins>HTML</ins>

**:mag_right:&nbsp; SEO**

- [ ] valeur invalide pour l'attribut `lang`
- [ ] meta "keywords": contenu trop vague / répétitif
- [ ] meta "description": contenu vide
- [ ] `<title>` doit être renseigné
- [ ] utilisation de `<h3>` au lieu de `<h2>`
- [ ] attribut `href` doit inclure protocole http pour les liens externes
      <br></br>

**:wheelchair:&nbsp; ACCESSIBILITÉ**

- [ ] texte `alt` pour les img: trop long / non descriptif de l'img
- [ ] font-size trop petite
- [ ] contraste couleurs incorrect
      <br></br>

**:rocket:&nbsp; PERFORMANCE**

- [ ] scripts à charger en `defer`ou `async`
- [ ] pas de `<li>` vide dans une `<ul>`
- [ ] css: trop de sélecteurs / sélecteurs inutilisés
- [ ] css: problème avec les media queries
- [ ] format img incorrect (.bmp)
- [ ] erreur dans la console au chargement de la page

## :ledger:&nbsp; <ins>Analyse</ins>

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
