# La Chouette - Website optimization Project

The goal of this project is to improve:

- :mag_right:&nbsp; SEO
- :wheelchair:&nbsp; Accessibility
- :rocket:&nbsp; Performance

of the website [La Chouette](https://newnightcoder.github.io/DanielJulien_4_05062021), a design agency based in Lyon, France.

## :memo:&nbsp; <ins>Analysis</ins>

### 10 recommendations:

- [ ] meta "keywords": content is too vague/repetitive
- [ ] meta "description": no empty content
- [ ] scripts to defer ?
- [ ] title must be provided
- [ ] no empty `<li>` in a `<ul>`
- [ ] img alt text too long / not descriptive of the img
- [ ] usage of `<h3>` instad of `<h2>`
- [ ] href attribute must include http protocol for external links
- [ ] css: too many selectors
- [ ] css: media queries issues

| Category     | Issue                                | Description                                          | Good practice                      | Recommended action |
| ------------ | ------------------------------------ | ---------------------------------------------------- | ---------------------------------- | ------------------ |
| :mag_right:  | improper content for meta "keywords" | content is too vague / repetitive                    |
| :mag_right:  | empty content in meta "description"  |
| :mag_right:  | empty `<title>`                      |                                                      | always provide a title to the page |
| :wheelchair: | improper alt for img                 | img alt text too long / not descriptive of the img   |
| :wheelchair: | font-size too small                  | `<p>` font-size is too small / hard to read          |
| :wheelchair: | improper color contrast              | insufficient brightness of text on img background    |
| :rocket:     | too many scripts to load             | jquery + other libraries to load before html parsing |
| :rocket:     | unused html                          | empty `<li>` in `<ul>`                               |
| :rocket:     | improper heading hierarchy           | usage of `<h3>` instead of `<h2>`                    |
| :rocket:     | css: too many selectors              |
|              | css media query issues               |
|              | improper href in links               | no http protocol for external links                  |

## :chart_with_upwards_trend:&nbsp; <ins>Optimization Report</ins>

- SEO improvements
- Results comparison:
  - Accessibility
  - Performance / loading time
