# Tablas y tablas de contenidos
Tablas y tablas de contenidos en Markdown

[[toc]]

## Tablas de contenidos
Note que al digitar `[toc]` en una línea aparte, es posible insertar una tabla de contenidos únicamente para los títulos de nivel 2 (##). Esta es una característica particular de la variante de Markdown utilizada en este sitio.

## Tablas simples
~~~markdown
Cabecera 1 | Cabecera 2
------ | -------
Celda 1 | Celda 2
Celda 3 | Celda 4
~~~

Cabecera 1 | Cabecera 2
------ | -------
Celda 1 | Celda 2
Celda 3 | Celda 4

## Tablas alineadas a la derecha
También es posible alinear el texto de la tabla a la derecha:
~~~markdown
Cabecera 1 | Cabecera 2
------: | -------:
Celda 1 | Celda 2
Celda 3 | Celda 4
~~~

Cabecera 1 | Cabecera 2
------: | -------:
Celda 1 | Celda 2
Celda 3 | Celda 4

## Tablas con listas
También es posible agregar listas dentro de una celda usando sintaxis de HTML.
~~~markdown
| Encabezado 1 | Encabezado 2 |
| ----------- | ----------- |
| Celda      | Título |
| Lista        | ¡Una lista dentro de una celda! <ul><li>Item one.</li><li>Item two.</li></ul> |
~~~

| Encabezado 1 | Encabezado 2 |
| ----------- | ----------- |
| Celda      | Título |
| Lista        | ¡Una lista dentro de una celda! <ul><li>Item one.</li><li>Item two.</li></ul> |