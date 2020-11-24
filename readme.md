####imprimir un string

print("hola mundo")

****salto de linea 
\n

---------------
4- tipos de variables
/*/*/*tres tipos de datos: 
numericos, booleanos, textos

***Asignacion de variables
numero = 10

***Mostrar por pantalla variable:
print(numero)

***imprimir el tipo de variable
print(type(nombrevariable))

/*/*/* Si ponemos un valor entero (int) ej 10 , un valor flotante (float) 10.5
ingresar comillas simples dentro de comillas dobles
variable = "la verdad o 'la verdad'"

****Datos booleanos
Valor = True
Valor = False



***concatener
print ("el resultado es: ",resultado)
colcamos unca coma para concatenar

***tipado dinamico
podemos almacenar diferentes tipos de variables
valor = 20
print(valor)
valor = "Sato"
print (valor)


--------------------------
5- comentarios
#comentario 
# esto es un comentario 
''' comentario multilinea
esto es un comentario multiiinea ***

------------------------
6- operadores aritmeticos
suma +
resta -
multiplicar *
dividir /
division entero (redondeado para abajo // 
modulo (que vamos a divir el resto de la division) %
exponenciacion  **

ejemplo:
2**3 * (5/2 + (6*5))

/*/*/*prioridad de los operadores aritmeticos
parentesis ()
exponenciacion **
multiplicacion, division, modulo *, / , %
suma y resta +, -


7- oepradores relacionales
*se utilizan para establecer una relacion entre 2 valores
*compara estos valores entre si y esta comparacion produce 
un resultado de certeza o falsedad (verdaderos o falsos)
*tienen el mismo nivel de su evaluacion
*los operadores relacionales tienen menor prioridad que los aritmeticos
> mayor que
< menor que
>= mayor o igual que
<= menor o igual que
!= diferente (distinto que)
== igual 

resultado = 10 < 20
print (resultado)

nos mostrarà verdero o falso.

----------------------------------------
8- operadores logicos
*permuitenb construir expreciones logicas y se obtiene como resultados booleanos
and && (perador de multiplicacion logica)
or  || (oeperador de suma logica)
not

/*/*/*operando AND
true and true = true
true and false = false
false and true = false
false and false = false
Donde sea 2 verderos hay verdadero, sin todo es falso

/*/*/*operando OR
true and true = true
true and false = true
false and true = true
false and false = false
Solo basta tener 1 solo verdadero para tener todos verdaderos 

***Operador de NOT negacion.
not(true) = false
not(false) = true 

/*/*/Prioridad de los operadores logicos
1. NOT
2- AND
3- OR 

Ejemplo 
((a>b) or (a<c))and((a==c) or (a>=b))

aqui tenemos que pensarlo 
Es muy bueno para hacer matematica discreta.


/*/*/*Pririedades de operadores en general
1. ()
2. **
3 *,/,mod %,not
4. +,-,and 
5. >, <, ==, >=, <=, !=, or 

-------------------------------- Operadores de asignacion
a = 5 
a += 5 #suma en asignaciòn.
a -= 2 #resta en asignacion
a *= 8 #multiplacion en asignacion
a /= 9 #division en asignacion 
a **=8 #potencia en asignicacion
a %=6 #modulo de la asignicion 
valores que sirven para acortar el código.

-----------------------------10 salidas de datos
print("hola",nombre,"tienes: ",edad,"años")
con funciones
print("hola {} tienes {} años".format(nombre,edad)
otra forma desde las ultimas actualizaciones de python:
print(f"Hola {nombre} tienes {edad} años")

-----------------------------11 entrada de datos 
#entrada de datos
nombre = input("mensaje al usuario")
##el input te lo guarda como cadena
##entonces podemos asingnar el tipo antes de poner el input
numero = int(input("ingresar un numero"))

----------------------------12 funciones integradas
#sirven para hacer conversiones entre tipos de datos
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

----------------------------13 


//////////////////
----------------------------prints
print("contenido",variable)
----------------------------input de usuario
variable=input(float("Ingrese numero: "))
cambiar el float por el tipo de variable, int, float string o boolean
----------------------------If, else
if resultado == 0:
contenido
else:
contenido del else

////////// podemos haer los valores aparte
ej:

vota=edad>=18 and edad<=70 and distancia<=500
if vota:
sasasa
else:


----------------------------Else if
elif resultado:
contenido



----------------------------While
while(i<=n):
    suma=suma+i
    #print(i,suma)
    i=i+1

----------------------------do while

----------------------------cadenas

-----------------------------import math
import math
math.sqr(numero) #raiz cuadrada
math.exp(1) #exponente
math.pi #pi
math.log(2) #logaritmo

"*"*10 ##multiplica por 10 el contenido de una cadena

-------------------------for
FOR
for i in range (1,11,1):
#El range(min_value, max_value) función range(min_value, max_value) genera una secuencia con números min_value , min_value + 1 , ..., max_value - 1 . El último número no está incluido. 


#Hay una forma reducida de range () - range(max_value) , en cuyo caso min_value se establece implícitamente en cero:
for i in range(3):
    print(i)
# 0
# 1
# 2

#De esta manera, podemos repetir algunas acciones varias veces:
for i in range(2 ** 2):
    print('Hello, world!')

#secuencia vacia
for i in range(-5):
    print('Hello, world!')

for character in 'hello':
    print(character)
#separa caracter a caracter

#Para iterar sobre una secuencia decreciente, podemos usar una forma extendida de range () con tres argumentos: range(start_value, end_value, step) . Cuando se omite, el paso es implícitamente igual a 1. Sin embargo, puede ser cualquier valor distinto de cero. El ciclo siempre incluye start_value y excluye end_value durante la iteración:

for i in range(10, 0, -2):
    print(i)
# 10
# 8
# 6
# 4
# 2

-----------------------print
Por defecto, la función print() imprime todos sus argumentos separándolos por un espacio y pone un símbolo de línea nueva después de él. Este comportamiento se puede cambiar usando los argumentos de palabras clave sep (separator) y end .

print(1, 2, 3)
print(4, 5, 6)
print(1, 2, 3, sep=', ', end='. ')
print(4, 5, 6, sep=', ', end='. ')
print()
print(1, 2, 3, sep='', end=' -- ')
print(4, 5, 6, sep=' * ', end='.')
