---
icon: 
  type: line-md:edit
  color: e2ac08 
---
# Texto, listas y títulos
Una introducción a los tipos más sencillos de sintaxis

## Texto plano
Para escribir texto sin formato, solo se debe escribir normalmente. El estándar de decodificación Unicode es soportado, por lo que también es posible hacer uso de caracteres matemáticos, pictogramas, letras griegas y emoticones 😜.

Para empezar un nuevo párrafo, se debe dejar un renglón en blanco, y escribir en una nueva línea.

## Estilos de letra
### Negrita
Para escribir con letra **negrita**, se debe encerrar el texto entre **asteriscos**, dos de cada lado.

~~~markdown
	**negrita**
~~~

### Itálica
Para escribir con letra *itálica*, se debe encerrar el texto con un asterisco de cada lado.

~~~markdown
	*itálica*
~~~

## Usando ambos tipos de letra
También es posible escribir en itálica y negrita ***simultáneamente***, para lo cual se encierra el texto con tres asteriscos de cada lado.

~~~markdown
	***simultáneamente***
~~~

## Listas
### Numeradas
Para hacer listas numeradas, basta con usar una numeración con punto y espacio, los números no tienen que ir en un orden particular, y pueden hasta repetirse. Markdown se encarga de que la lista quede impecable.

Por ejemplo,
~~~markdown
100. Primer elemento
4. Segundo elemento
17. Tercer elemento
~~~
resulta en

100. Primer elemento
4. Segundo elemento
17. Tercer elemento

### No numeradas
Para listas no numeradas se debe marcar una entrada con cualquiera de los signos *,+, - seguido de un espacio.

~~~markdown
- A
* B
- C
+ D
+ E
~~~
Lo anterior resulta en 
- A
* B
- C
+ D
+ E

**A pesar de que funciona correctamente, no es bien visto mezclar signos.**

### Mezclando listas
Es posible mezclar listas usando identación.
1. Primer elemento
2. Segundo elemento
	+ Primer sub elemento
		+ Primer sub sub elemento
			+ Primer sub sub sub elemento
   				+ Primer sub sub sub sub elemento
	+ Segundo sub elemento
3. Tercer elemento

~~~markdown
1. Primer elemento
2. Segundo elemento
	+ Primer sub elemento
		+ Primer sub sub elemento
			+ Primer sub sub sub elemento
   				+ Primer sub sub sub sub elemento
	+ Segundo sub elemento
3. Tercer elemento
~~~

## Líneas horizontales
Usando ***, ___ o --- es posible insertar una línea horizontal en el documento.

~~~markdown
***

---
~~~

***

---

## Títulos
Para hacer títulos, se pueden colocar de uno a cuatro signos numerales (#) seguidos de un espacio y el texto del título, resultando respectivamente en un título de menor jerarquía.
~~~markdown
	# Título 1
	## Título 1
	### Título 1
	#### Título 1
	##### Título 1
~~~
# Título 1
## Título 1
### Título 1
#### Título 1