# Contadores de listas
## Objetivo: 
Hemos descubierto unas misteriosas ruinas antiguas en el fondo del océano y  eres parte del equipo que viajará hasta el descubrimiento en un submarino :ocean: :ocean: :ocean:. El objetivo de la exploración es recupera objetos interesantes y traerlos a la superficie para estudiarlos. 

Antes de empezar la exploración, tu tarea es crear un programa que sirva como una lista sobre los objetos que deberán buscar entre las ruinas. Estos objetos pueden ser cosas como reliquias, fósiles o esculturas. Tu programa será usado por nuestro submarino para indicar las cosas que debemos buscar y que no olvidemos nada. 

## Conocimiento usado:
1. Variables
2. print
3. while
4. Listas
5. len() 
¡No olvides intentar el challenge cuando hayas acabado el programa! El challenge está al final.

## Actividad:
Recuerda probar tu código depsués de haber completado cada instrucción, para saber si funciona correctamente.
1) Crear una lista con **10** objetos. Estos son los objetos que imaginas que se pueden encontrar en las ruinas submarinas.
>Ponle un nombre diferente a tu lista
~~~python
milista_submarina = ["fósiles", "reliquias", "eculturas"] 
~~~

2) Abajo de tu lista, usa un print para mostrar el primer objeto de la lista.
~~~python
print(milista_submarina[0])
~~~

3) Crea un ciclo while que comience en 0 y cuente hasta 10.  10, porque es la cantidad de objetos en la lista.
> Recuerda poner los espacios debajo del While!!! Justo como lo puse en el i = i+1
~~~python
i = 0

while i <10:

	i = i+1
~~~

4) Pon el print del paso 2, dentro del while que acabas de crear
>No olvides el espacio
~~~python
i = 0

while i <10:
	print(milista_submarina[0])
	i = i+1
~~~

Hasta ahora, nuestro programa imprime 10 veces el primer objeto de la lista, pero nosotros queremos que imprima el objeto siguiente de la lista...¿se te ocurre algo que podemos usar para esta tarea?
>Pista: Debemos cambiar el 0 que está dentro de milista_submarina[0] por otra cosa...

Intenta encontrar la respuesta, antes de ver la solución en el paso siguiente.

5) Cambia el 0 que está dentro de milista_submarina[0] por nuestro iterador i
~~~python
i = 0

while i <10:
	print(milista_submarina[i])
	i = i+1
~~~

¡Con esto ya deberíamos de imprimir todos los objetos de la lista!

6) Ahora le daremos un poco de formarto a nuestro programa. Modifica el print que está dentro del while para que se vea así:
~~~python
print("El objeto número",i,"de la lista es:",milista_submarina[i])
~~~

7) Para terminar, agrega dos prints hasta el final, **Afuera del while** que digan algo parecido a lo siguiente:
~~~python
print("Verificando...[+]...[+]...[+]...")
print("Lista verificada, sistemas verificados, listos para empezar!")
~~~

## Resultado:
El resultado al correr tu código debería verse así:
~~~shell
El objeto número 0 de la lista es: objeto1
El objeto número 1 de la lista es: objeto2
El objeto número 2 de la lista es: objeto3
El objeto número 3 de la lista es: objeto4
El objeto número 4 de la lista es: objeto5
El objeto número 5 de la lista es: objeto6
El objeto número 6 de la lista es: objeto7
El objeto número 7 de la lista es: objeto8
El objeto número 8 de la lista es: objeto9
El objeto número 9 de la lista es: objeto10
Verificando...[+]...[+]...[+]...
Lista verificada, sistemas verificados, listos para empezar!
~~~

## Challenge
Nuestro programa está listo, pero ahora lo mejoraremos. El problema, es que el código sólo funciona cuando la lista tiene 10 objetos. Si agregamos o borramos objetos, el programa va a fallar y en una expedición en las profundidades del océano, no podemos permitir que algo falle.

Para solucionar esto, aprenderemos a usar un comando llamado len(). len viene de lenght que quiere decir longitud en inglés y sirve para obtener la longitud de cosas. 

Por ejemplo si usamos len("hola"), el programa dirá 4, porque la palabra hola, tiene una longitud de 4 letras.

| h   | o   | l   | a   |
| --- | --- | --- | --- |
| 1   | 2   | 3   | 4   |


En len("Python"), será de 6, porque Python tiene 6 letras.

len() también puede ser usado en listas, por ejemplo
~~~python
milista_submarina = ["fósiles", "reliquias", "eculturas"] 
~~~
La longitud de la siguiente lista es de 3, porque contiene 3 objetos.

| fósiles | reliquias | esculturas |
| ------- | --------- | ---------- |
| 1       | 2         | 3          |

Entonces nosotros podemos guardar la longitud (cantidad de objetos que tiene) de un arreglo en un arreglo y sustituir el 10 del ciclo while por esa variable. Vamos a intentarlo

1) Crear una variable que esté arriba del ciclo while y guardar ahí la longitud del arreglo
>Esa variable debe de estar abajo del arreglo y arriba del while
>Recuerda cambiar lista dentro de len, por el nombre de tu lista
~~~python
numero_objetos = len(lista)
~~~

2) Cambiar el 10 del while por nuestra variable
~~~python
while i < numero_objetos:
~~~

Y listo, así tenemos un código a prueba de errores.

3) Por último, para probar esto, borra o agrega 2 objetos de lista y ve si todo funciona como debería

_Innovaland 2021, creado por: Salvador Rodríguez_
