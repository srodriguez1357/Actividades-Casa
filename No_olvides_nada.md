# ¡No olvides Nada!
## Objetivo: 
En tu familia se han estado quejando mucho últimamente sobre que cuando van al súper, olvidan algunas cosas de lo que hay que comprar. El día de hoy bajaste a prepararte unos deliciosos hotcakes pero cuando ya habías servido la harina, te diste cuenta que habían olvidado comprar la leche y los huevos, en ese momento decidiste ponerle un alto a este problema de memoria y decidiste crear una solución al respecto. Después de pensar mucho en una solución, has decidido crear una aplicación en Python, que sirva para crear una lista para el Súper. 

## Conocimiento usado:
1. Variables
2. print
3. while
4. Listas
5. append

## Actividad:
1) Crear un arreglo llamado lista de super
~~~python
listasuper = []
~~~
2) Crear una variable llamada objeto y asignarle el valor de a
~~~python
objeto = "a"
~~~
3) Crear una variable llamada contador y asignarle el valor de 0
~~~python
contador = 0
~~~
4) Crear un ciclo while que la condición sea objeto != ""
Esto quiere decir que el programa se va a ejecutar hasta que el usuario deje el input vacío, una vez que presionemos enter sin haber agregado un objeto, se sale del ciclo y se cierra la aplicación
~~~python
while objeto != "" :
~~~
5) Agrega un input dentro del while(cuidar los espacios) que nos pregunte cuál es el objeto que queremos guardar y lo almacene en la variable objeto
>El código de abajo solamente es un ejemplo, no es como se hace, si lo copias igual, no va a funcionar
~~~python
variable = input("")
~~~
6) Agregar un if que su condición sea objeto!=""
~~~python
if(objeto!=""):
~~~
7) Adentro del if usar el comando append para agregar el objeto a la lista
~~~python
listasuper.append(objeto)
~~~
8) Sumarle uno a la variable contador
>El código de abajo solamente es un ejemplo, no es como se hace, si lo copias igual, no va a funcionar
~~~python
i = i + 1
~~~
9) Agregar un else afuera del if
~~~python
if():
	bla
	bla
	bla
else:
	<aquí estamos>
~~~
10) Agregar un break adentro del else
11) Agregar un print que diga. numeroobjetos siempre será distinto y usará los datos de la variable contador para mostrar el número de objetos
~~~text
Tu lista tiene <numeroobjetos> objetos
~~~
12) Agregar un print que diga. listasuper, será nuestro arreglo, imprimirá todo el arreglo
~~~text
Tu lsita de super: <listasuper>
~~~
## Resultado:
El resultado al correr tu código debería verse así:
### Prueba 1
~~~shell
¿Qué objeto quieres agregar? manzana
¿Qué objeto quieres agregar? jugo
¿Qué objeto quieres agregar? pan de muerto
¿Qué objeto quieres agregar? dulces
¿Qué objeto quieres agregar? hamster
¿Qué objeto quieres agregar? 
Tu lista tiene 5 objetos
Tu lista: ['manzana', 'jugo', 'pan de muerto', 'dulces', 'hamster']
~~~
### Prueba 2
~~~shell
¿Qué objeto quieres agregar? zanahoria
¿Qué objeto quieres agregar? 
Tu lista tiene 1 objetos
Tu lista: ['zanahoria']
~~~

## Resultado final
Tu resultado final debe verse algo como esto, cuida de usar los nombres de varibales y espacios correctos.
>Los objetos que tienen un * al lado, quiere decir que se deben modificar, ejemplo variable1* quiere decir que ese no es el nombre correcto de la variable
~~~python
objeto = "a"
contador = 0
  
while objeto != "" :
	variable* = input("¿Qué objeto quieres agregar? ")

	if(objeto!=""):
		listasuper.append(objeto)
		i* = i* + 1
	else:	
		break

print("Tu lista tiene",variable*,"objetos")
print("Tu lista:",lista*)
~~~
