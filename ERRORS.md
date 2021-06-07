# :memo:&nbsp; <ins>ERRORS REPORT</ins>

## BAD PRACTICES

### <ins>HTML</ins>

**:mag_right:&nbsp; SEO**

- [ ] improper value assigned to `lang` attribute
- [ ] meta "keywords": content is too vague/repetitive
- [ ] meta "description": no empty content
- [ ] title must be provided
- [ ] usage of `<h3>` instad of `<h2>`
- [ ] href attribute must include http protocol for external links
      <br></br>

**:wheelchair:&nbsp; ACCESSIBILITY**

- [ ] img alt text too long / not descriptive of the img
- [ ] font-size too small
- [ ] improper color contrast
      <br></br>

**:rocket:&nbsp; PERFORMANCE**

- [ ] scripts to defer
- [ ] no empty `<li>` in a `<ul>`
- [ ] css: too many selectors
- [ ] css: media queries issues
- [ ] improper img format (.bmp)
- [ ] error logged in the console

## :ledger:&nbsp; <ins>Analysis</ins>

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

<br></br>

Optimization report [here](/OPTIMIZATION-REPORT.md).  
Go back to [README](README.md).
