# Leyendo la mente de la computadora
## Objetivo: 
Hacer un juego usando valores aleatorios :game_die:
## Requisito:
Antes de hacer esta actividad, debes haber completado: https://github.com/srodriguez1357/Actividades-Casa/blob/main/random.md
## Conocimiento usado:
1. random
2. Variables
3. if - else
4. input
5. eval

## Antes de empezar: 
En esta actividad crearemos un juego que funcionará de la siguiente manera
* La computadora escogerá un número al azar entre 1 y 6, esto simula el tirar un dado
* El programa nos va a pedir un número
* Si el número que escribimos es igual al que escogió la computadora, ganamos
* Si no logramos adivinar el número, la computadora nos dirá algo como Game Over o mejor suerte para la próxima
## Actividad:
1. Importa el módulo random
* ```import random```
2. Crea una variable que guarde el resultado de usar *randint*
3. Crea una variable que guarde la respuesta del jugador cuando escriba su respuesta
4. Pedirle al jugador que ingrese el número que cree que la computadora escogió
> No olvides el eval
5. Comparar la variable de la computadora y la del jugador
> Recuerda que para saber si dos variables son iguales usamos dos símbolos de igual (==)
6. Si ambas variables son iguales, decirle al jugador que ganó
7. Si no son iguales, decirle que perdió
