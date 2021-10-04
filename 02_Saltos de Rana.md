# Saltos de Rana
## Objetivo: 

## Conocimiento usado:
1. Identaciones
2. while
3. if
4. else

## Recordando aprendizajes... 
### Un solo espacio
Python cambia el uso de símbolos como  `{};` por el uso de espacios. Los espacios o identaciones funcionan como en el español, pero en vez de separar párrafos u oraciones, separamos bloques de código.

Cuando decimos que algo está adentro de otro bloque, como decir que "la variable va adentro del if", "el break va adentro del else" o "La operación va adentro del if", nos estamos refiriendo a que este código es parte del bloque, entonces en la parte exterior tenemos una estructura como el while o el if y el código que va adentro de este es el que se va aejecutar.
ejemplos:
1) En este caso el print está dentro del while
~~~python
i = 0
while(i<10):
	print("Hello world")
~~~
¿Notas como el while está pegado al borde y el print tiene **un** espacio?

2) En este caso el print está dentro del if
~~~python
numero = 100
if(numero=100):
	print("Hello world")
~~~
¿Notas como el if está pegado al borde y el print tiene **un** espacio?

En todos estos casos, podemos ver que los bloques que están adentro de otro, cuentan con un espacio a la izquierda
#### Apoyo visual
![iamgen1](https://github.com/srodriguez1357/Actividades-Casa/blob/main/images/Pasted%20image%2020211004103128.png)
![[images/Pasted image 20211004103128.png]]
_Fuente: Python for Kids_

### Houston...necesitamos más espacios
¿Qué pasa cuando tenemos varias estructuras? ¡Ponemos más espacios! Por ejemplo, si tenemos un if adentro de un while adentro un while, se vería algo así:
~~~python
i = 0
j = 0
  
while(i<10):
	while(j<15):
		if(j<100): 
			print(j)
		j=j+1
	print(i)
	i=i+1
~~~

![[Pasted image 20211004143046.png]]

Cuenta los espacios que hay en cada nivel. El primer while está pegado, el while que está adentro, tiene un espacio, el if que está adentro del while que está adentro del while, tiene 2 espacios, el print que está adentro del if que está adentro del while que está adentro del while tiene 3 y ya empieza a parecer trabalenguas.

#### Apoyo visual
![[Pasted image 20211004103100.png]]
_Fuente: Python for Kids_

## Actividad:
1) Copia y pega el siguiente código en un nuevo proyecto de replit vacío

~~~python
numerosuerte = eval(input("Ingresa tu número de la suerte: "))

i = 0

while numerosuerte!=1:
if(numerosuerte%2==0):
numerosuerte = numerosuerte/2
print(numerosuerte)
i=i+1

else:
numerosuerte = (numerosuerte*3)+1
print(numerosuerte)
i = i+1
  
print("Tu número mágico es",i)
~~~

2) Una vez pegado tu proyecto debería verse así, verifica que si esté igual que en la imagen. El banner de hasta arriba tú le puedes agregar el que quieras una vez que todo funcione

![[Pasted image 20211004140524.png]]

3)  Agrega todos los espacios/identaciones necesarios para que el código funcione. Lo único que hay que corregir del código son espacios, todo lo demás funciona correctamente. 
>Recuerda que si tienes duda, puedes ver códigos anteriores y volver a leer la sección de recordando aprendizajes


## Resultado:
El resultado al correr tu código debería verse así:
### Prueba 1
~~~shell
Ingresa tu número de la suerte: 7
22
11.0
34.0
17.0
52.0
26.0
13.0
40.0
20.0
10.0
5.0
16.0
8.0
4.0
2.0
1.0
Tu número mágico es 16
~~~
### Prueba 2
~~~shell
Ingresa tu número de la suerte: 12
6.0
3.0
10.0
5.0
16.0
8.0
4.0
2.0
1.0
Tu número mágico es 9
~~~

### Prueba 3
~~~shell
Ingresa tu número de la suerte: 35
106
53.0
160.0
80.0
40.0
20.0
10.0
5.0
16.0
8.0
4.0
2.0
1.0
Tu número mágico es 13
~~~

## Resultado final
Para probar que tu código funcione correctamente, ingresa estos números como tu número de la suerte y ve que obtengas los mismo resultados

| Númerosuerte | Númeromágico |
| ------------ | ------------ |
| 1            | 0            |
| 2            | 1            |
| 3            | 7            |
| 5            | 5            |
| 7            | 16           |
| 8            | 3            |
| 9            | 19           |
| 10           | 6            |
| 12           | 9             |

_Innovaland 2021, creado por: Salvador Rodríguez_
