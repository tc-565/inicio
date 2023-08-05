# Líneas, bloques de código y citas
Inserción de código en línea y bloques con un ambiente especial

## Líneas de código
Para escribir código en una línea, hay que delimitarlo con los caracteres ``\.

~~~
`` print(‘Hola mundo’)``
~~~
`` print(‘Hola mundo’)``

## Bloques de código
Para escribir un bloque de código, se delimitan las líneas con ~~~, donde en la parte superior se escribe ~~~nombre_del_lenguaje.

~~~python
n = 10
num1 = 0
num2 = 1
next_number = num2 
count = 1
 
while count <= n:
    print(next_number, end=" ")
    count += 1
    num1, num2 = num2, next_number
    next_number = num1 + num2
print()
~~~

## Citas
Usando el caracter > al inicio de una línea, es posible hacer una cita de texto.

~~~markdown
> Texto citado
>
> Continuación de cita
~~~

> Texto citado
> 
> Continuación de cita