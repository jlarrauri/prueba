# Prueba de markdown

Esto es un prueba de listas
* Elemento 1
   * subelemento 1
   * subelemento 2
* Elemento 2
   * subelemento 3
   
```java
var markdownpdf = require("markdown-pdf")
  , fs = require("fs")

fs.createReadStream("/path/to/document.md")
  .pipe(markdownpdf())
  .pipe(fs.createWriteStream("/path/to/document.pdf"))

markdownpdf().from("/path/to/document.md").to("/path/to/document.pdf", function () {
  console.log("Done")
})
```


Esto ya es un texto

## Listas simples
  - uno
     -  rojo
     - verde
     - azul
  - dos
  - tres
