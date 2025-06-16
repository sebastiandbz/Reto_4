# Reto_4

## Resolucion de los problemas del reto.

### 1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.

```python
n : int
n = int(input("Ingrese un número entero: "))

if n == 97 or n == 101 or n == 105 or n == 111 or n == 117:
    print("El número corresponde al código ASCII de una vocal minúscula.")
else:
    print("El número no corresponde al código ASCII de una vocal minúscula.")
```

### 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.

```python
cadena: str
cadena = input("Ingrese una cadena de longitud 1: ")

codigo_ascii: int = ord(cadena[0])

if codigo_ascii % 2 == 0:
    print("El código ASCII de la primera letra es par.")
else:
    print("El código ASCII de la primera letra es impar.")
```

### 3.Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.

```python
n = (input("Ingrese un caracter: "))

if n == '1' or n == '2' or n == '3' or n == '4' or n == '5' or n == '6' or n == '7' or n == '8' or n == '9' or n == '0':
  print("El caracter es un digito")
else:
  print("El caracter no es un digito")
```

### 4. Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.

```python 
numero1: float
numero1 = float(input("Ingrese el primer número: "))
numero2: float
numero2 = float(input("Ingrese el segundo número: "))

if numero1 % numero2 == 0:
  print("El primer número es múltiplo del segundo.")
else:
  print("El primer número no es múltiplo del segundo.")
```

### 5. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

Positivo: "El número x es positivo"

Negativo: "El número x es negativo"

Cero (0): "El número x es el neutro para la suma"

```python 
x: float
x = float(input("Ingrese un número real: "))

if x > 0:
    print(f"El número {x} es positivo")
elif x < 0:
    print(f"El número {x} es negativo")
else:
    print(f"El número {x} es el neutro para la suma")
```

### 6. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.

```python 
x_centro: float = float(input("Ingrese x del centro del círculo: "))
y_centro: float = float(input("Ingrese y del centro del círculo: "))
radio: float = float(input("Ingrese el radio del círculo: "))

x_punto: float = float(input("Ingrese x del punto: "))
y_punto: float = float(input("Ingrese y del punto: "))

distancia_al_cuadrado: float = (x_punto - x_centro)**2 + (y_punto - y_centro)**2

if distancia_al_cuadrado < radio**2:
    print("El punto está dentro del círculo.")
else:
    print("El punto NO está dentro del círculo.")
```

### 7. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.

```python 
a: float = float(input("Ingrese la primera longitud: "))
b: float = float(input("Ingrese la segunda longitud: "))
c: float = float(input("Ingrese la tercera longitud: "))

if a + b > c and a + c > b and b + c > a:
    print("Las longitudes SÍ pueden formar un triángulo.")
else:
    print("Las longitudes NO pueden formar un triángulo.")
```

### 8. Escriba un programa que reciba el nombre en minúsculas de un país de America y retorne la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado (Utilice match-case).

```python 
pais: str = input("Ingrese el nombre del país: ")

match pais:
    case "argentina":
        print("La capital es Buenos Aires.")
    case "brasil":
        print("La capital es Brasilia.")
    case "chile":
        print("La capital es Santiago.")
    case "colombia":
        print("La capital es Bogotá.")
    case "peru":
        print("La capital es Lima.")
    case "mexico":
        print("La capital es Ciudad de México.")
    case "canada":
        print("La capital es Ottawa.")
    case "estados unidos":
        print("La capital es Washington D.C.")
    case "uruguay":
        print("La capital es Montevideo.")
    case "paraguay":
        print("La capital es Asunción.")
    case _:
        print("País no identificado.")
```

## Todos los codigos fueron ejecutados desde google colab.
## Muchas gracias x la atencion prestada.
