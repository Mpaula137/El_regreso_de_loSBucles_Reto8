# El_regreso_de_loSBucles_Reto8
La segunda parte de bucles, son ejemplos de como entendimos el bucle for
## Punto 1:
- Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
Explicación: Utilizams el ciclo for y luego colocamos la intencion de cada iteación en la impresión
```
#Este programa imprime el cuadrado de los numero desde el 1 al 100

#vamos a utilizar un ciclo for pra iterar los numeros del 1 al 100
for n in range(1, 101): #colocamos el rango hasta 101 ya que este va de forma (n-1)
  # imprimiremos el numero i y con una separación de ":" y colocamos el cuadrado con el signo **
 print(n, ":", n**2)
 ```
 ## Punto 2:
 - Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
 Explicación: Use el ciclo for ajustando el rango y la forma en la que aun¿menta para crear una lista de pares e impares
 ```
 #Imprime los numeros de 1 a 999 usando un ciclo for(sabiendo que cuando aunmenta ( muestra los numeros impares)
for i in range(1,1000, 2):
    print(i)

#Imprimer los numeros de 2 a 1000 usando ciclo for(sabiendo que cuando aumenta mostrara los numeros pares
for i in range(2, 1001, 2):
    print(i)
 ```
 ## Punto 3:
 - Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado.
 Explicación: Primero investigue para poder guiarme luego encontre que el usuario debe ingresar el numero despues se agrega la condición donde i debe ser mayor o igual  a 2, ponemos en rango y el descenso dentro del ranfo luego colocamos la condicion que debe cumplir el numero al que se descendio para imprimirse. 
 ```
 #se le pide al usuario que ingrese un numero mayor o igual a 2 con la funcion imput
i =int(input("Ingrese un numero mayor o igual a 2:"))

# la condicion nos permitira verificar que el numero se mayor o igual a 2
if i>=2:
    for n in range(i, 1, -1): #ponemos el for para que recorra el rango hacia atras 
        if n % 2 == 0: #Ponemos otra condicion la cual nos dice que si el numero n tiene modulo de 2 para que queden numeros pares
            print(n)
else:
    print("el numero ingresado no es mayor o igual a 2")

 ```
 ## Punto 4:
 -  Imprimir los números de 1 hasta un número natural n dado, cada uno con su respectivo factorial.
 Explicación: tenemos que llamar a la funcion factorial, en esta misma entablamos las condiciones adecuadas. Luego usamos la funcion name, interactuamos con el usuario y colocamos el condicional el cual dice que n debe ser mayor a 0 y se pone el buble for para decir que va desde 1 hasta n+1 y se imprime. 
 ```
 def factorial(n):
    """
    Esta función calcula el factorial de un número n
    """
    if n==0:
        return 1
    else:   
        return n* factorial(n-1)

if __name__ == "__main__": #Llamo la funcion name ya que utilizare un funcion anteriormente impuesta
    n= int(input("Ingrese un numero natural:"))
if n>=0:#se crea la condicion para usar el factorial
    for i in range(1, n+1): #ponemos n+1 para que el rango nos quede en n
        print(i, ":", factorial(i))
else:
    print("NO es un nuemro natural")
 ```
 ## Punto 5:
 -  Calcular el valor de 2 elevado a la potencia n usando ciclos for.
 Explicación: inicializamos una variable con el valor que de el usuario otra la inicializamos en 1 luego declaramos el for para el rango n es decir que lo que queramos realizar pase3 por todo ese rango, luego decimos que la variable igual mientras aunmente sera multiplicado 2.
 ```
 #Este programa se creo para obtener a 2 elevado n veces
n = int (input("Ingrese un numero natural :"))#declaramos la variable num la cual el usuario va a ingresar
igual= 1 #declaramos igual ya que cualquier numero elevado a 0 da 1

for i in range(n):  #declaramos el ciclo for para que 2 se multiplique po si mismo n veces
    igual *=2 # quiere decir que se multiplica dos segun n veces
print("el resultado de 2 elevado a la portencia", n, "es:", igual)

 ```
 ## Punto 6:
 - Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for.
 Explicación: inicalizamod dos variables segun el valor que coloque el usuario usamos el mismo procedimiento que en el anterior punto solo que esta vez las dos las colocara el usuario el for lo colocamos para una variabe i en el rango de n allí dice que resultado que la inicalizamos en 1 y aumenta segun el valor de n se expresa para que```
 x se multiplique esas veces.
 ```
 #Este programa permite obtener a x elevado n veces
n = int(input("Ingrese un numero natural:")) # Declaramos la variable n el cual va a seer el exponente
x = float(input("Ingre un numero real:"))# Declaramos la variable  x la cual va a ser la base

resultado= 1 #inicializamos la varibale resultado en uno

for i in range(n):#declaramos en ciclo for para que pase por todo el rango de n 
    resultado*=x #resultado que se inicalizo en uno se multiplicara en x
print(x,"Elevado a potencia", n, "es:", resultado)
 ```
 ## Punto 7:
 - Diseñe un programa que muestre las tablas de multiplicar del 1 al 9.
 Explicación: En el ejemplo de abajo solo coloque la de la primera tabla ya que la metodología es la misma para todas las tablas, yo empece inializando una variable en o para tener el valor de las iteraciones liego cree el rango en donde se pone el primer multiplo y el multiplo de la multiplicación del numero por 11 luego se suma la cantidad de ves que sea necesario para crear la tabla como a continuación.
 ```
 #Este programa permite identificar todas las tablas del 2 al 9 
iteracion=0 #esto permite crear el numero de iteracion
for i in range(2,22,2): # Creo el ciclo for para que se recorran los en el rango sumando de a dos
    iteracion+=1 # en esta se declara que en cada ciclo se le sume uno a la iteracion para tener mejor claridad al momento del resultado
    print("iteracion numero",iteracion, "de la tabla del 2:", i)

 ```
 
