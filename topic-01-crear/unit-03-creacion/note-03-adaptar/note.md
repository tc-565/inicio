---
icon: 
  type: ph:archive
  color: e2ac08 
---
# Adaptación correcta de material
Adaptación correcta de `.tex`, presentaciones y documentos de texto

## .tex
Para adaptar un documento `.tex` en el sitio web, adapte el texto en notas markdown adecuadamente, adjunte el código fuente (esto incluye todos los archivos auxiliares, imágenes, macros, etc...) en un objeto `archive` y el archivo PDF compilado en un objeto `paneltalk` o `talk`.

## Presentaciones y beamer
Para presentaciones, convierta la presentación a PDF, e incluya ambos documentos, el PDF y la presentación en un objeto `paneltalk` o `talk`. En caso de ser beamer, incluya el código fuente en un objeto `archive` y el archivo PDF compilado en el objeto `paneltalk` o `talk`.

## Otros documentos de texto (Word)
Adapte el texto en notas markdown, e incluya el archivo de texto original como un archivo auxiliar en la primera de las notas. Recuerde mencionar este archivo en markdown con la sintaxis para adjuntar archivos.
