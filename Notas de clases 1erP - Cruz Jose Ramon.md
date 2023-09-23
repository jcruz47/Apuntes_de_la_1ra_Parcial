 Apuntes 1er parcial
---
###### Cruz Rodriguez Jose Ramon
-----------------------
## La programacion funcional
La programación funcional es un paradigma de programación que se basa en el concepto de funciones matemáticas y se enfoca en el tratamiento de datos como valores inmutables y en la aplicación de funciones para transformar esos datos.
##### Caracteristicas
-Enfoque Principal: 
Se centra en el uso de funciones como elementos fundamentales.
-Funciones Pura: 
Las funciones son puras, lo que significa que producen el mismo resultado para los mismos argumentos y no tienen efectos secundarios.
-Inmutabilidad: 
Se promueve la inmutabilidad de los datos siempre que sea posible, evitando la modificación de variables y promoviendo la creación de nuevos valores.
-Recursión: 
La recursión se utiliza en lugar de bucles para controlar el flujo del programa.
-----

#### Tipos de datos:
Los tipos de datos son elementos fundamentales ya que te permiten almacenar y manipular diferentes tipos de información. 
###### `Tipos de Datos Numéricos:`

- **int**: Este tipo de dato se utiliza para representar números enteros, como -1, 0, 1, 2, etc. Los enteros en Python no tienen límites de tamaño, lo que significa que pueden ser tan grandes como la memoria lo permita.

- **float**: Los números de punto flotante se utilizan para representar números con decimales, como 3.14 o -0.001. Los números de punto flotante en Python siguen el estándar de punto flotante IEEE 754.

- **complex**: Los números complejos se utilizan para representar números complejos, que tienen una parte real y una parte imaginaria, como 3+2j.

###### `Tipo de Dato Decimal:`

- Python también tiene un tipo de dato decimal (`decimal`) que se utiliza para realizar cálculos de punto flotante con una precisión decimal fija. Es útil cuando se requiere una precisión exacta en cálculos financieros o científicos.

###### `Tipo de Dato Científico:`

- No existe un tipo de dato científico nativo en Python, pero puedes utilizar el tipo `float` para representar números en notación científica. Por ejemplo, `3.14e-10` representa 3.14 multiplicado por 10 elevado a la potencia negativa de 10.

###### `Tipo de Dato Lógico:`

- **bool**: Este tipo de dato se utiliza para representar valores booleanos, que pueden ser `True` (verdadero) o `False` (falso). Los valores booleanos se utilizan en expresiones lógicas y en el control de flujo de un programa para tomar decisiones.

###### `Tipo de Dato Cadena (String):`

- **str**: Las cadenas son secuencias de caracteres, como texto o palabras. Se utilizan para representar y manipular datos de texto. Las cadenas se pueden definir entre comillas simples (' '), comillas dobles (" "), o incluso comillas triples (''' ''' o """ """) para cadenas multilínea.
----------------------------------
#### Operadores:
###### `Operadores Aritméticos:`

- **+**: Suma
- **-**: Resta
- **\***: Multiplicación
- **/**: División
- **//**: División entera (resultado redondeado al número entero más cercano)
- **%**: Módulo (el residuo de la división)
- **\*\***: Potencia (por ejemplo, `2 ** 3` es igual a 2 elevado a la potencia de 3, es decir, 8)

Los operadores aritméticos se utilizan para realizar operaciones matemáticas en Python.

###### `Operadores Lógicos:`

- **and**: Operador lógico "y"
- **or**: Operador lógico "o"
- **not**: Operador lógico "no"

Los operadores lógicos se utilizan para combinar expresiones lógicas y evaluar condiciones en Python.

###### `Operadores Condicionales:`

- **==**: Igual a
- **!=**: No igual a
- **<**: Menor que
- **>**: Mayor que
- **<=**: Menor o igual que
- **>=**: Mayor o igual que
------------------------------------------------
#### Estructuras de datos:

###### `Listas (`list`):`

Las listas en Python son colecciones ordenadas y mutables de elementos. Puedes almacenar una variedad de tipos de datos en una lista y modificarla añadiendo, eliminando o modificando elementos. Las listas se definen utilizando corchetes `[]`.

###### `Diccionarios (`dict`):`

Los diccionarios son colecciones de pares clave-valor que se utilizan para mapear un valor (valor) a una clave (key). Son útiles cuando necesitas buscar un valor basado en una clave. Los diccionarios se definen utilizando llaves `{}`.

###### `Conjuntos (`set`):`

Los conjuntos son colecciones no ordenadas y mutables de elementos únicos. Se utilizan cuando necesitas almacenar elementos únicos y realizar operaciones de conjuntos, como unión e intersección. Los conjuntos se definen utilizando llaves `{}` o la función `set()`.

###### `Tuplas (`tuple`):`
 Las tuplas son colecciones ordenadas e inmutables de elementos. A diferencia de las listas, no se pueden modificar después de su creación. Las tuplas se definen utilizando paréntesis `()`.

-------------------------------------------------------------
#### Estructuras Condicionales:
###### `if:`

La declaración `if` se utiliza para realizar una acción si una condición es verdadera. Por ejemplo:

```python
if condicion:
    # Código a ejecutar si la condición es verdadera
```    
###### `if-else:`
La declaración if-else permite ejecutar un bloque de código si una condición es verdadera y otro bloque de código si la condición es falsa. Por ejemplo:
```python
if condicion:
    # Código a ejecutar si la condición es verdadera
else:
    # Código a ejecutar si la condición es falsa
``` 
###### `if-elif-...-else:` 
La declaración "if-elif-...-else" permite evaluar múltiples condiciones en secuencia y ejecutar el bloque de código del primer if o elif que sea verdadero. Si ninguno es verdadero, se ejecuta el bloque else.

###### `Concordancia de patrones estructurado (structural pattern matching):`
La concordancia de patrones estructurado permite realizar coincidencias en datos complejos, como listas, tuplas, diccionarios y objetos personalizados.
```python
def procesar_datos(datos):
    match datos:
        case 1:
            print("El valor es 1")
        case "texto":
            print("El valor es 'texto'")
        case [1, 2, 3]:
            print("El valor es una lista [1, 2, 3]")
        case _:
            print("El valor no coincide con ninguno de los casos anteriores")

# Llamada a la función con diferentes datos
procesar_datos(1)
procesar_datos("texto")
procesar_datos([1, 2, 3])
procesar_datos(42)
```


------------------------------------------
#### Estructuras para Control de Flujo:

###### `Iterables e Iteradores:`

Los iterables son objetos que se pueden recorrer, como listas y tuplas. Los iteradores son objetos que permiten recorrer un iterable uno a uno, utilizando métodos como `next()`. Puedes crear iteradores personalizados implementando los métodos `__iter__()` y `__next__()`.

###### `Estructura for:`

El bucle `for` se utiliza para iterar sobre elementos en un iterable. Puedes recorrer listas, tuplas, diccionarios, y más utilizando un bucle `for`.

###### `Estructura while:`

El bucle `while` se utiliza para ejecutar un bloque de código repetidamente mientras una condición sea verdadera.

###### `Uso de range, break y continue:`

- `range()`: Se utiliza para generar secuencias de números.

- `break`: Se utiliza para salir de un bucle antes de que se complete.

- `continue`: Se utiliza para pasar a la siguiente iteración de un bucle sin ejecutar el resto del código en ese ciclo.
###### `Estructuras anidadas:`
se refieren a la práctica de incluir una estructura de datos dentro de otra estructura de datos.
- `Listas Anidadas`: Puedes tener listas dentro de listas 
```python
matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```
- `Diccionarios Anidados`: Puedes tener diccionarios dentro de diccionarios
```python
persona = {
    'nombre': 'Juan',
    'edad': 30,
    'direccion': {
        'calle': '123 Main St',
        'ciudad': 'Ciudad A',
        'codigo_postal': '12345'
    }
}
```
- `Listas de Diccionarios`: Se utilizan listas que contienen diccionarios para representar conjuntos de datos relacionados. Cada diccionario en la lista puede representar un elemento individual con sus propias propiedades.
```python
contactos = [
    {'nombre': 'Ana', 'telefono': '123-456-7890'},
    {'nombre': 'Juan', 'telefono': '987-654-3210'},
    {'nombre': 'María', 'telefono': '555-555-5555'}
]
```
