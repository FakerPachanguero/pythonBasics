# Python
Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.


# Basic
Formas de escribir idenfificadores en Python:

    - secuencias de caracteres alfanuméricos del alfabeto inglés
    - Usando ( _ ) underscore - guión bajo
    - No usar espacios
    - No usar caracteres especiales ($, &, *, #)
    - No iniciar con valores numéricos y de preferencia no incorporarlos
    - No ser una palabra reservada del lenguaje.


### lowcase :  

    Es el uso exclusivo de mínusculas.


### UPPERCASE:

    Es el uso exclusivo de mayusculas.

### camelCase:

    Consiste en la capitalización de la inicial de cada palabra compuesta excepto la inicial. El cambio entre minúsculas y mayúsculas se asemeja a las jorobas de un camello.

### Snake_Case

    Consite en el uso de underscore para separar las palabras en una entidad compuesta, la cual estará siempre en minúscula. Las secciones se asemejan a las partes de una serpiente (?.


# <center> Variables </center>


### Definición

    Una variable es un espacio de memoria donde se almacena un dato, un espacio donde se guarda la información necesaria para realizar las acciones que ejecutan los programas.


### Constantes
    A diferencia de C, Java o Javascript, en Python no hay constantes perse, se suele declarar una variable global en snake case mayúsculas para indicar que se trata de un valor persistente.

### Casting
To specify the data type of a variable, this can be done with casting.

```PY
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
```

### Imprimir variables 
La función más importante a la hora de programar, nos permite visualizar en consola: variables, mensajes de texto y el resultado de operaciones, etc.

```PY
print()
```
### Get the Type

    You can get the data type of a variable with the type() function.

### Declarar consiste en nombrar la variable y declarar su tipo, sin especificar un valor inicial.

    Nombre_variable : <tipo_dato>


### Inicializar: Consiste en dar un valor inicial luego de declarar una variable.

```PY
# Declarar variable
x : int
# Inicializar variable
x = 10 
# Declarar e inicializar variable
x : int = 10
```

### Cantidad de bits

```PY
print(x.bit_length)
```

### Representacion binaria 
```PY
print(bin(x)) 
```


### Tipos de datos
    Text Type: 	str
    Numeric Types: 	int, float, complex
    Sequence Types: 	list, tuple, range
    Mapping Type: 	dict
    Set Types: 	set, frozenset
    Boolean Type: 	bool
    Binary Types: 	bytes, bytearray, memoryview
    None Type: 	NoneType

### Boolean
    You can evaluate any expression in Python, and get one of two answers, True or False

```py
x : bool = False
x : bool = True
```


### Numbers
    There are three numeric types in Python:

### Int

    Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.

```py
x : int = 1    
   
```
### Float

    Float, or "floating point number" is a number, positive or negative, containing one or more decimals.
```py
y : float = 2.8  
x = 35e3
y = 12E4
z = -87.7e100
```
### Complex
Complex numbers are written with a "j" as the imaginary part:

```py
8  
z : complex = 1j   
```
### Convertion
```py
#convert to float:
a = float(x)

#convert to int:
b = int(y)

#convert to complex:
c = complex(x) 
```

### Strings
String variables can be declared either by using single '' or double "" quotes:

```py
x = "John"
x = 'John'
```
### Codigo ASCII de un carácter

```py
ord('a')
```

### Carácter de un codigo ASCII
```py
chr('')
```

### Bloque de texto
You can use three single or double quotes
```py
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
```

Get the character at position 1 (remember that the first character has the position 0):


```py
a = "Hello, World!"
print(a[1])
```

### length of a string
To get the length of a string, use the len() function.

```py
a = "Hello, World!"
print(a[1])
```

### Check String

To check if a certain phrase or character is present in a string, we can use the keyword in.


```py
txt = "The best things in life are free!"
print("free" in txt)

# Denial
print("expensive" not in txt)
```



# <center> Operaciones </center>

Es la manera de establecer relaciones (operaciones) entre los tipos de variables.

    Operadores infijos: Se aplican entre los operandos.
    Operadores prefijos: Se aplica antes del operando.
    Operadores sufijos: Se aplica después del operando.

## Operadores aritméticos

Se aplican a los datos de tipo numérico (luego veremos que algunos se pueden sobrecargar a otras estructuras de datos).

### Suma
     Usa el simbolo (+) y obtiene la suma de dos o más valores.
```py
# Suma de dos numeros
4 + 1 # Entero + Entero = Entero
4.0 + 1 # Real + lo que sea = Real 
```


### Resta
    Usa el simbolo (-), representa la sustracción cuando está entre dos operandos (infijo) o la negación (cambio de signo) cuando predece al oeprando (prefijo).


```py
# Sustacción de dos numeros
4 - 1 # Entero - Entero = Entero
-1 # Cambio de signo
```

### Multiplicación
    Usa el simbolo (*) y obtiene el producto entre dos o más valores.

```py
# Producto de dos numeros
4 * 2.0 # Entero * Real = ?
```

### División
    Usa el símbolo (/) y retorna la división exacta.

```py
# División de dos numeros
4 / 2 # Entero / Entero = ?
4.0 / 2 # Real / Entero =?
4.0 / 0 # Tan tan tan
```

### División Entera
    Usa el símbolo (//) y retorna la parte entera de la división exacta.

```py
# División exactas de dos numeros
5 // 2 # Entero / Entero = ?
5.0 // 2 # Real / Entero =?
```


### Módulo
    Usa el símbolo (%) y retorna el residuo de la divisón entre dos números.

```py
# modulo entre dos números
10 % 2 # Entero % Entero = ?
5.0 % 2 # Real / Entero =?
```


### Potencia 
    Usa el símbolo (**) y retorna elevar a una cierta potencia un operando. Importante: NO se usa el símbolo (^) -> Acento circunflejo (Hay gente que le dice el sombrerito...que falta de nivel).

```py
# potencias entre dos números
5**2 # Cuadrados
5**3 # Cubos
81**0.5 # Raíces
```

# <center> Operadores de asignación </center>

    Asignación: Usa el simbolo (=). La parte de la izquierda que debe ser una variable. Sirve para almacenar un dato en una variable. Asigna el valor de evaluar la parte de la derecha a la variable de la parte de la izquierda.

```py

x : int = 1
x += 1 # Equivalente a x = x + 1

x : int = 2
x -= 1 # Equivalente a x = x - 1

x : int = 4
x *= 3 # Equivalente a x = x * 3

x : int = 4
x /= 2 # Equivalente a x = x / 2

x : int = 8
x //= 4 # Equivalente a x = x // 4

x : int = 8
x %= 4 # Equivalente a x = x % 4
```

# <center>Operadores lógicos</center>

    Permiten determinar juicios de valor sobre proposiciones lógicas, su resultando es un booleano.

### Igualdad
    Evalua si dos variables son iguales. Se usa el simbolo
```py
alpha : int = 10
beta : int = 10 
alpha == beta
```

### Diferencia
    Evalua si dos variables son diferentes. Se usa el simbolo (!=). o
```py
alpha : int = 10
beta : int = 11 
alpha != beta
```

### Mayor estricto
    Evalua si la variable de la izquierda es mayor que la de la derecha. Se usa el simbolo (>). 
```py
alpha : int = 10
beta : int = 11 
beta > alpha
```
### Menor estricto
    Evalua si la variable de la izquierda es menor que la de la derecha. Se usa el simbolo (<).
```py
alpha : int = 10
beta : int = 11 
alpha < beta
```
### Mayor igual
    Evalua si la variable de la izquierda es mayor o igual que la de la derecha. Se usa el simbolo (>=).
```py
alpha : int = 10
beta : int = 10 
alpha >= beta
```
### Menor igual
    Evalua si la variable de la izquierda es menor o igual que la de la derecha. Se usa el simbolo (<=). 
```py
alpha : int = 10
beta : int = 10 
alpha >= beta
```
## Operadores relacionales ó lógicas

### Negación/NOT
    Permite evaluar la operación not. Se utiliza la palabra reservada not.

<table cellspacing="1" bgcolor="">
	<tr bgcolor="#252582">
		<th><b>A</b></th>
    <th><b>NOT(A)</b></th>
	</tr>
	<tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">0</td>
    <td style="color:#141414">1</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">1</td>
    <td style="color:#141414">0</td>
	</tr>
</table>



### Conjunción/AND
    Permite evaluar la operación and (y en español). Se utiliza la palabra reservada and.

<table cellspacing="1" bgcolor="">
	<tr bgcolor="#252582">
		<th><b>A</b></th>
    <th><b>B</b></th>
    <th><b>AND(A,B)</b></th>
	</tr>
	<tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">0</td>
    <td style="color:#141414">0</td>
    <td style="color:#141414">0</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">0</td>
    <td style="color:#141414">1</td>
    <td style="color:#141414">0</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">1</td>
    <td style="color:#141414">0</td>
    <td style="color:#141414">0</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">1</td>
    <td style="color:#141414">1</td>
    <td style="color:#141414">1</td>
	</tr>
</table>

### **Disyunción/OR:**
    Permite evaluar la operación *or* (o en español). Se utiliza la palabra reservada *or*.
<table cellspacing="1" bgcolor="">
	<tr bgcolor="#252582">
		<th><b>A</b></th>
    <th><b>B</b></th>
    <th><b>OR(A,B)</b></th>
	</tr>
	<tr tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">0</td>
    <td style="color:#141414">0</td>
    <td style="color:#141414">0</td>
	</tr>
  <tr tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">0</td>
    <td style="color:#141414">1</td>
    <td style="color:#141414">1</td>
	</tr>
  <tr tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">1</td>
    <td style="color:#141414">0</td>
    <td style="color:#141414">1</td>
	</tr>
  <tr tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">1</td>
    <td style="color:#141414">1</td>
    <td style="color:#141414">1</td>
	</tr>
</table>

### Precedencia de opearaciones
En la siguiente tabla se presenta la prioridad de los principales operadores
de Python, la prioridad más alta es la 1 y la más baja es la 9. Si dos operaciones tienen la misma prioridad se resuelve de izquierda a derecha.

<table cellspacing="1" bgcolor="">
	<tr style="text-align: center; vertical-align: middle;" bgcolor="#252582">
		<th><p align=center><b>Operador(es)</b></p></th>
    <th><b>Prioridad</b></th>
	</tr>
	<tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
		<td style="color:#141414">()</td>
    <td style="color:#141414">1</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">not &nbsp &nbsp &nbsp -(signo menos) &nbsp &nbsp &nbsp +(signo más) &nbsp &nbsp &nbsp **(potencia)</td>
    <td style="color:#141414">2</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">* &nbsp &nbsp &nbsp / &nbsp &nbsp &nbsp // &nbsp &nbsp &nbsp %</td>
    <td style="color:#141414">3</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">+ &nbsp &nbsp &nbsp -</td>
    <td style="color:#141414">4</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">< &nbsp &nbsp &nbsp > &nbsp &nbsp &nbsp <= &nbsp &nbsp &nbsp >=</td>
    <td style="color:#141414">5</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">== &nbsp &nbsp &nbsp ~=</td>
    <td style="color:#141414">6</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">and</td>
    <td style="color:#141414">7</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">or</td>
    <td style="color:#141414">8</td>
	</tr>
  <tr style="text-align: center; vertical-align: middle;" bgcolor="#e4e4ed">
    <td style="color:#141414">= &nbsp &nbsp &nbsp += &nbsp &nbsp &nbsp -= &nbsp &nbsp &nbsp *= &nbsp &nbsp &nbsp /= &nbsp &nbsp &nbsp //= &nbsp &nbsp &nbsp %=</td>
    <td style="color:#141414">9</td>
	</tr>
</table>

# <center>CONDICIONALES</center>
