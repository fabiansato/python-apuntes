# Cheatsheet Python🐍

## Instalar herramientas
cmder

------------------------------
## Tipos de variables
#### tres tipos de datos: 
```python
numericos, booleanos, textos
```

#### Asignacion de variables
```python
numero = 10
```


#### Datos booleanos
```python
Valor = True
Valor = False
```

### Entrada de datos 
```python
nombre = input("mensaje al usuario")
```
el input te lo guarda como cadena
entonces podemos asingnar el tipo antes de poner el input
```python
numero = int(input("ingresar un numero"))
```
cambiar el float por el tipo de variable, int, float string o boolean
ejemplo:

```python
numero = str(input("ingresar un numero"))
```

------------------------------
## Mostrar datos por pantalla
#### Imprimir un string
```python
print("hola mundo")
```

#### salto de linea 
```python
\n
```

### Triple comillas dobles
Se puede mostrar un string largo ejemplo:
```python
menu = """ 
Bienvenido al conversor de monedas😊
"""
```
#### imprimir el tipo de variable
```python
print(type(nombrevariable))
```

#### mostrar int o float
Si ponemos un valor entero (int) ej 10 , un valor flotante (float) 10.5
ingresar comillas simples dentro de comillas dobles:
```python
variable = "la verdad o 'la verdad'"
```


### Separadores en print
Podemos separar internamente datos con la palabra clave "sep=" y terminar con "end="
```python
print(1, 2, 3, sep=', ', end='. ')
print(4, 5, 6, sep=' * ', end='.')
```


#### concatener
```python
print ("el resultado es: ",resultado)
colcamos unca coma para concatenar
```

#### tipado dinamico
podemos almacenar diferentes tipos de variables
```python
valor = 20
print(valor)
valor = "Sato"
print (valor)
```

#### comentarios

```python
# esto es un comentario 
''' comentario multilinea
esto es un comentario multinea ***
```
----------------------------------------
### operadores aritmeticos

```python
suma +
resta -
multiplicar *
dividir /
division entero (redondeado para abajo // 
modulo (que vamos a divir el resto de la division) %
exponenciacion  **
```

ejemplo:
```python
2**3 * (5/2 + (6*5))
```

#### prioridad de los operadores aritmeticos
```python
1. parentesis ()
2. exponenciacion **
3. multiplicacion, division, modulo *, / , %, NOT
4. suma y resta +, -, AND
5.  >, <, ==, >=, <=, !=, or 
```

----------------------------------------
### Operadores relacionales
se utilizan para establecer una relacion entre 2 valores
compara estos valores entre si y esta comparacion produce 
un resultado de certeza o falsedad (verdaderos o falsos)
tienen el mismo nivel de su evaluacion
los operadores relacionales tienen menor prioridad que los aritmeticos
```python
> mayor que
< menor que
>= mayor o igual que
<= menor o igual que
!= diferente (distinto que)
== igual 
```
ejemplo:
```python
resultado = 10 < 20
print (resultado)
```
nos mostrarà verdero o falso.

----------------------------------------
### operadores logicos
*permiten construir expreciones logicas y se obtiene como resultados booleanos
and && (perador de multiplicacion logica)
or  || (oeperador de suma logica)
not

#### Operador AND

valor1 | AND | valor2  | Resultado
------------ | ------------- |------------- |------------- |
TRUE | AND | TRUE  | TRUE
TRUE | AND | FALSE  | FALSE
FALSE | AND | TRUE  | FALSE
FALSE | AND | FALSE  | FALSE


_Solamente basta un false para que el resultado sea false_

#### Operador OR

valor1 | AND | valor2  | Resultado
------------ | ------------- |------------- |------------- |
TRUE | AND | TRUE  | TRUE
TRUE | AND | FALSE  |  TRUE
FALSE | AND | TRUE  | TRUE
FALSE | AND | FALSE  | FALSE

_Solamente es falso cuando ambos son false false (0 y 0)_


#### Operador de NOT negacion.
```python
not(true) = false
not(false) = true 
```

#### Prioridad de los operadores logicos

1. NOT
2. AND
3. OR 


Ejemplo:
```python
((a>b) or (a<c))and((a==c) or (a>=b))
```

aqui tenemos que pensarlo 
Es muy bueno para hacer matematica discreta.


--------------------------------
## Operadores de asignacion
a = 5 
a += 5 #suma en asignaciòn.
a -= 2 #resta en asignacion
a *= 8 #multiplacion en asignacion
a /= 9 #division en asignacion 
a **=8 #potencia en asignicacion
a %=6 #modulo de la asignicion 
valores que sirven para acortar el código.

-----------------------------
### salidas de datos
```python
print("hola",nombre,"tienes: ",edad,"años")
```
con funciones:
```python
print("hola {} tienes {} años".format(nombre,edad)
```

otra forma desde las ultimas actualizaciones de python:
```python
print(f"Hola {nombre} tienes {edad} años")
```

lo mismo para convetir variables ya ingresadas usamos
```python
int();
str();
float();
```
----------------------------
### CONDICIONALES
#### Condicionales (If, else)
```python
if resultado == 0:
	contenido
else:
	contenido del else
```

_podemos haer los valores aparte_
ej:

```python
vota=edad>=18 and edad<=70 and distancia<=500
if vota:
sasasa
else:
```



#### Condicionales (While)
```python
while(i<=n):
    suma=suma+i
    print(i,suma)
    i=i+1
```


#### Condicionales (FOR)
Se coloca for _variable_ in range (_valor minimo_,_valor maximo_,_sumadevariable_)

```python
for i in range (1,11,2):
```
El antarior codigo es for variable _i_ en el rango de iniciacion en 1, hasta 11 con salteos de 2. El último numero no se incluye.

### Condicional for range(min_value, max_value)
función range(min_value, max_value) genera una secuencia con números min_value , min_value + 1 , ..., max_value - 1 . El último número no está incluido. 


### Forma reducida de range () 
Se realiza de la siguiente manera range(max_value) , en cuyo caso min_value se establece implícitamente en cero:
```python
for i in range(3):
    print(i)
# 0
# 1
# 2
```

### De esta manera, podemos repetir algunas acciones varias veces:
```python
for i in range(2 ** 2):
    print('Hello, world!')
```

#### Ejemplo de secuencia vacia
```python
for i in range(-5):
    print('Hello, world!')
```


#### Secuencia decreciente
Para iterar sobre una secuencia decreciente, podemos usar una forma extendida de range () con tres argumentos: range(start_value, end_value, step) . Cuando se omite, el paso es implícitamente igual a 1. Sin embargo, puede ser cualquier valor distinto de cero. El ciclo siempre incluye start_value y excluye end_value durante la iteración:
```python
for i in range(10, 0, -2):
    print(i)
# 10
# 8
# 6
# 4
# 2
```
----------------------------
###  MANEJO DE ARCHIVOS

Abrir archivo de lectura : 
```python
f = open("fichero.txt") 
```
Abrir archivo de lectura : 
```python
f = open("fichero.txt", "r") 
```

Abrir archivo para escribir desde cero : 
```python
f = open ("fichero.txt", "w") 

Abrir archivo para añadir al final :
```python
f = open ("fichero.txt", "a") 
```
⚠️ Recordar siempre al terminar de utilizar un archivo tanto para lectura o escritura cerrarlo.
 No hacerlo puede traer problemas para poder utilizarlo luego.

Simplemente basta llamar a 
```python
f.close() 
```
Donde f es la variable en donde se almacenó el archivo 
```python
(ejemplo, f = open("fichero.txt", "r") )
```

#### Leer de un archivo
Para leer del archivo, podemos usar las funciones f.readlines() y f.readline() 
Lectura de todo el archivo de golpe : 
```python
datos = f.readlines() 
(datos es una lista con todos los elementos del archivo)
```
Lectura de una línea completa : 
```python
dato = f.readline() 
```
(dato es una cadena con la primer línea del archivo)

#### Funciones para conocer donde está el cursor en
el archivo y para ubicarlo en otro lugar
```python
archivo.tell() 
archivo.seek() 
```

#### Funciones con write
```python
función f.write(“texto”)
f = open("arch.txt","w")
f.write("Esto es un archivo de texto\n");
f.write("Generado con python\n");
f.write("no es hermoso?\n")
f.close()
```

-----------------------------
### BIBLOTECAS
#### biblioteca import math
```python
import math
math.sqr(numero) #raiz cuadrada
math.exp(1) #exponente
math.pi #pi
math.log(2) #logaritmo

"*"*10 ##multiplica por 10 el contenido de una cadena
```

----------------------------
### Biblioteca Random
Debemos importar la biblioteca para utilizar sus funciones de trabajos aleatorios.
```python
import random
```
uso de biblioteca:
```python
random.randrange(inico,fin,paso)
random.randint(inicio,fin)

```
ejemplo
```python
import random
w=random.randrange(1,100,2)
print("w es:",w)

```
ejemplo con for range
```python
for i in range(3):
	w=random.randrange(1,100,2)
	print("w es:",w)
    # Por cada iteración obtiene un numero impar  aleatorio entre 1 y 99 .
Eventualmente podrían llegar a repetirse los números

```
```python
import random
w=random.randint(inicio,fin)
# Devuelve un entero aleatorio entre inicio y fin incluyendo los extremos.

```

----------------------------
### FUNCIONES
#### Funciones integradas
sirven para hacer conversiones entre tipos de datos
```python
n = int(10)
n = float(10)
n = str("10")
n = bin(1)
n = hex(10F)
n = int("010",2) #convierte un binario a entero
n = int("0xa",16) #convierte un numero hexa en base 16 a int
n = abs(-8) #devuelve un balor absoluto de -8
n = round (5.6) #lo redondea al numero entero mas cercano
n = len("fabian") #muestra cuantas caracteres tiene el string
```

## Metodos array

```python
# transforma en mayuscula todo el string
nombre.upper()
# transforma en minúscula todo el string
nombre.lower()

# transforma la primera letra en mayuscula del string
nombre.capitalize()

# elimina espacios vacios adelante y atras del string
nombre.strip()

# remplaza una letra o caracter seleccionado por otro seleccionado en un string
nombre.replace('o', 'a')

# Tamaño del string
len("mostrara el tamaño del texto")


```

# Arrays Slices
```python
nombre = "Fabian"
print(nombre)



print(nombre[0 : 3])
# Fab

 #Va desde el principio hasta antes de llegar del 3° índice. Cómo no hay ningún parámetro en el primer lugar, se interpreta que arranca desde el principio.
print(nombre[:3])
# Fab

#Arranca desde el índice 1 hasta llegar antes del 7.
print(nombre[1:7])
# abian


 #Arranca desde el índice 1 hasta llegar antes del 7, pero pasos de 2 en 2, ya que eso es lo que nos indica el 3! parámetro, el cual es 2.
print(nombre[1:7:2])
# ain


 #Arranca desde el índice 1 hasta el final del string (al no haber ningún 2° parámetro, significa que va hasta el final), pero en pasos de 3 en 3.
print(nombre[1::3])
# aa


  #Al no haber parámetro en los 2 primeros lugares, se interpreta que se arranca desde el inicio hasta el final, pero en pasos de 1 en 1 con la palabra al revés, porque es -1.
print(nombre[::-1])
# naibaF


```

---------------------------------
### Strings de caracteres
#### separa caracter a caracter
```python
for character in 'hello':
    print(character)

```
tamaño del caracter:
```python
a="Hola Mundo"
len(a)
```

Recorrer una cadena:
```python
a="mi cadena"

for caracter in a:
    print(caracter)

```
otra forma:
a="mi cadena"
```python
for caracter in a:
    print(caracter, end="")
```


-----------------------------
### FUNCIONES
```python
def funcion(parametro):
```

```python
def NOMBRE(LISTA_DE_PARAMETROS):
    """DOCSTRING_DE_FUNCION"""
    SENTENCIAS
    RETURN [EXPRESION]
```
Refs:
- NOMBRE, es el nombre de la función.
- LISTA_DE_PARAMETROS, es la lista de parámetros que puede recibir una función.
- DOCSTRING_DE_FUNCION, es la cadena de caracteres usada para documentar la función.
- SENTENCIAS, es el bloque de sentencias en código fuente Python que realizar cierta operación dada.
- RETURN, es la sentencia return en código Python.
- EXPRESION, es la expresión o variable que devuelve la sentencia return.

ejemplo s/ retornar:
```python
def mostrarGuion ( ) :
    print ( "-" , end="" )
```

Ejemplo c/ retorno
```python
def resta(a, b):
    return a - b
```  

Pasar variables por argumentos:
```python
argumento = "Nunca digas nunca."
imprimirDosVeces ( argumento )
```

## Tupla
```python
mi_tupla = ()
mi_tupla = (1,2,3)
```

### generar una tupla de un solo valor
`mi_tupla = (1,)`

### Acceder a un índice de la tupla

```python
mi_tupla = (1,2,3)
mi_tupla[0] #1
mi_tupla[1] #2
mi_tupla[2] #3
```

### Reasignar una tupla

```python
mi_tupla = (1,2,3)
mi_otra_tupla = (4,5,6)
mi_tupla =+ mi_otra_tupla
```

### Métodos para trabajar con tuplas

Usando el ejemplo:

`mi_tupla = (1,1,1,2,2,3)`

### Encontraremos los siguientes métodos:

`mi_tupla.count(1)`
    Devolverá 3, ya que el número 1 aparece 3 veces en la tupla.
	
`mi_tupla.index(3)`
    Devolverá 5, índice de la primera instancia donde se encuentra un elemento.
	
`mi_tupla.index(1)`
    Devolverá 0
`mi_tupla.index(2)`
    Devolverá 3.

-----------------------------
### LISTAS (Arrays)
### declaración de listas:
```python
my_lista = []
my_lista = list()
```
### creacion de listas:
```python
lista = [7; 3; 4; 6; 10]
```

### unir lista
```python
my_lista = [1]
my_lista2 = [2,3,4]
my_lista3 = my_lista + my_lista2
my_lista3 # [1,2,3,4]
```
otra forma
```python
my_lista = [1]
my_lista2 = [2,3,4]
my_lista.extend(my_lista2) # [1,2,3,4]
```
### partir listas con slice
```python
my_lista = [1,2,3]
my_lista[1:] = [2,3]
```

### multiplicar lista:
```python
my_lista = ['a']
my_lista2 = my_lista * 5
my_lista2 # ['a','a','a','a','a']
```

### longitud de lista:
```python
len(lista)
```
agregar un elemento al final de la lista:
```python
lista:append(2)
```
### Eliminar elementos de la lista:
```python
lista.pop(3)
#quita el tercer elemento de la lista empezando por 0
```
mostrar toda la lista por pantalla:
```python
print(lista)
```

### Recorrer listas:
codigo base para todos
```python
animales = [''gato'', ''perro'', ''raton'']
i = 0
```
#forma 1
```python
while (i < len(animales)):
	print(animales[i])
i = i + 1
```

#forma 2
```python
for i in range(len(animales)):
	print (animales[i])
```

#forma 3
```python
for elemento in animales:
	print (elemento)
```

### ordenar lista
```python
my_lista = [2,1,5,4,3]
my_lista = my_lista.sort()
my_lista # [1,2,3,4,5]
```

## eliminar un elemento especifico en la lista
```python
my_lista = [1,2,3,4,5]
del my_lista[0]
my_lista # [2,3,4,5]
```

### eliminar si conocemos su valor
```python
my_lista = [1,2,3,4,5]
my_lista.remove(3)
my_lista #[1,2,4,5]
```
## saber que metodos hay dentro de un elemento en la lista
```python
my_lista = [1,2,3,4,5]
dir(my_lista) # ['__add__', '__class__', '__contains__', ...
```

### modificar un elemento en la lista
```python
my_lista = [1,2,3,4,5]
my_lista[0] = 100
my_lista # [100,2,3,4,5]
```

### agregar un elemento al final de la lista
```python
my_lista = [1,2,3,4,5]
my_lista.append(6)
my_lista # [1,2,3,4,5,6]
```

### ordenar una lista
```python
my_lista = [2,5,1,3,4]
my_lista.sort() #[1,2,3,4,5]
```
-------------

### Métodos adicionales para listas
`.sorted()`
    También ordena como sort() pero modifica la lista inicial

`clear()`
    Vacía la lista

`.count()`
    Cuenta las veces que esta un elemento en lista

`.index()`
    Indica la posición donde esta un elemento de la lista
	
`.insert()`
    Inserta un elemento en una posición dada ej: lista.insert(posición,item)
	
`.reverse()`
    Le da la vuelta a una lista

## Diccionarios (son como objetos)
Los diccionarios en Python son una estructura de datos mutable las cuales almacenan diferentes tipos de valores sin darle importancia a su orden. Identifican a cada elemento por una clave (Key). Se escriben entre {}.

Operaciones en diccionarios

`.keys():` Retorna la clave de nuestro elemento.

`.values():` Retorna una lista de elementos (valores del diccionario).

`.items():` Devuelve lista de tuplas (primero la clave y luego el valor).

`.clear():` Elimina todos los items del diccionario.

`.pop(“n”):` Elimina el elemento ingresado.

Cómo trabajar con diccionarios

    Definir función principal

```python
def run():
    # Defino el diccionario, agrego los valores.
    mi_diccionario = {
      'llave1' : 1,
      'llave2' : 2,
      'llave3' : 3,
    }
```

    Imprimir las llaves del diccionario utilizando un bucle for. Con .keys()’ estamos llamando a imprimir las llaves, no los valores.

```python
for llave in mi_diccionario.keys():
        print(llave)
```

    Imprimir los valores del diccionario empleando un bucle for. Con ’.values()’ estoy llamando a imprimir los valores.

```python
for valores in mi_diccionario.values():
        print(valores)
```

    Imprimir las llaves y los valores usando ‘.items()’. Para esto, coloco las variables llave e items.

```python
for llave, items in 			mi_diccionario.items():
        print("La llave: '" + llave + "' contiene el item: " + str(items))

if __name__ == '__main__':
    run()
```

Aporte creado por: Rusbel Bermúdez, Ignacio Escudero.


### MATRICES (Matrix)
Las matrices en Python son listas de listas.
se escriben así:
```python
[lista0, lista1,...,listaN]
```
ejemplo:
```python
numeros = [[1,2,4],[4,3,2],[9,8,7],[6,4,3],[5,6,8]]
	print(numeros[0][2]) # imprime 4
	print(numeros[3][0]) # imprime 6
	print(numeros[4][3]) # error
```

### También podemos imprimir la matriz entera:
```python
print(numeros)
print(numeros[2])
```

### Saber la longitud de una variable
```python
longitud = len(numeros)
print (longitud) #imprime 5
print(len(numeros[2])) #imprime 3
```

### Agregar datos a un array
```python
#por ejemplo
numeros[2].append(5) 
agrega un 5 al final de la lista 2
```

### Quitar datos en un array:
```python
numeros[3].pop(1) 
elimina la posición 1 de la lista 3
```
