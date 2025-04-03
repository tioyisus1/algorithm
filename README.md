# **Conceptos Fundamentales de Programación**

En la programación, existen ciertos conceptos fundamentales que son esenciales para escribir código eficiente y bien estructurado. Entre ellos, encontramos:  

1. Variables  
2. Operadores Matemáticos (Math)  
3. Operadores Lógicos  
4. Ciclo For  
5. if/else/elif  
6. Funciones y Parámetros  

A continuación, explicaremos cada uno de estos en detalle, proporcionando ejemplos prácticos y casos de uso en la vida real.  


---

## **1. Variables: Almacenamiento de Datos en Memoria** 📝  

### **¿Qué es una variable?**  
Una variable representa un contenedor o un espacio en la memoria física o virtual de una computadora, donde se almacenan distintos tipos de datos (valores) durante la ejecución de un programa. A cada variable se le asigna un nombre descriptivo o un identificador que se refiere al valor guardado. Los datos almacenados pueden cambiar de valor o ser constantes.

Las variables sirven para guardar y recuperar datos, representar valores existentes y asignar unos nuevos. Las variables permiten que los programadores se refieran a un valor con un nombre representativo en vez de tener que recordar este valor, lo que facilita muchas tareas complejas.

Así, puedes usar valores almacenados en cálculos, operaciones de entrada y salida, comparaciones y otros tipos de procesamiento de datos. Por ejemplo, en un programa de contabilidad, una variable puede almacenar el saldo de una cuenta, y otra variable representa el monto de una transacción. A través de las variables, puedes realizar fácilmente operaciones matemáticas para actualizar el saldo de la cuenta.

### **Caracteristicas de una variable**
Una variable en programación se caracteriza por:

El nombre único que la identifica dentro del programa
El valor guardado que puede cambiar durante la ejecución del programa
El tipo de datos que se almacena, como números, textos, estados booleanos, etc.
El alcance, que puede ser global, si se puede acceder desde cualquier parte del programa, o local, si solo se puede acceder dentro de un bloque de código.

### **Tipos de variables en programación**  
Los tipos de variables dependen del lenguaje de programación. Cada lenguaje tiene sus propios tipos de datos y formas de definir variables. El tipado puede ser estático, cuando los tipos de variables se establecen a la hora que se declaren, o dinámico, cuando el tipo se determina y se asigna durante la ejecución del programa.

Algunos de los tipos de variables más comunes son:

Variables numéricas que almacenan números enteros.

Variable de punto flotante que guardan números con decimales.

Variables de caracteres que representan símbolos o caracteres.

Variables de cadena de caracteres que contienen palabras y textos.

Variables lógicas o booleanas que sirven para almacenar valores lógicos (verdadero o falso).

### **Ejemplo básico de variables en Python:**  
```python
nombre = "David"
edad = 30
altura = 1.75

print(f"Hola, mi nombre es {nombre}, tengo {edad} años y mido {altura} metros.")
```
Aquí, la variable `nombre` almacena una cadena de texto, `edad` almacena un número entero y `altura` almacena un número decimal.  

### **Ejemplo práctico en una aplicación real:**  
Imagina que estás desarrollando un sistema para una tienda en línea. Puedes usar variables para almacenar el precio de un producto y calcular su precio con impuestos:  

```python
precio = 50000  # Precio en pesos colombianos
impuesto = 0.19  # 19% de IVA
precio_final = precio + (precio * impuesto)

print(f"El precio final del producto es: {precio_final} COP")
```
Aquí usamos una variable para almacenar el precio y otra para el impuesto, lo que nos permite calcular fácilmente el valor total sin necesidad de modificar manualmente los números.  

---

## **2. Operadores Matemáticos (Math) ➕➖✖️➗**  

Los operadores matemáticos nos permiten realizar cálculos en nuestros programas.  

### **Tipos de operadores matemáticos en Python:**  
| Operador | Descripción | Ejemplo |
|----------|-------------|---------|
| `+` | Suma | `a + b` |
| `-` | Resta | `a - b` |
| `*` | Multiplicación | `a * b` |
| `/` | División | `a / b` |
| `//` | División entera | `a // b` |
| `%` | Módulo (resto de división) | `a % b` |
| `**` | Potencia | `a ** b` |

### **Ejemplo en la vida real: cálculo de sueldo con bonificaciones**  
```python
sueldo_base = 2000000
bonificacion = 500000
sueldo_total = sueldo_base + bonificacion

print(f"El sueldo total del empleado es: {sueldo_total} COP")
```
Aquí usamos la suma para calcular el sueldo total de un empleado.  

---

## **3. Operadores Lógicos (and, or, not) 🤔**  

Los operadores lógicos permiten evaluar condiciones en los programas. Son muy útiles para la toma de decisiones.  

### **Tipos de operadores lógicos:**  
| Operador | Descripción | Ejemplo |
|----------|-------------|---------|
| `and` | Verdadero si ambas condiciones son verdaderas | `a > 10 and b < 5` |
| `or` | Verdadero si al menos una condición es verdadera | `a > 10 or b < 5` |
| `not` | Invierte el valor lógico | `not(a > 10)` |

### **Ejemplo práctico: Validación de acceso en un sistema**  
```python
usuario = "admin"
contraseña = "1234"

if usuario == "admin" and contraseña == "1234":
    print("Acceso concedido")
else:
    print("Acceso denegado")
```
Aquí usamos `and` para asegurarnos de que **tanto** el usuario como la contraseña sean correctos antes de conceder acceso.  

---

## **4. Ciclo For: Iteración sobre Elementos 🔄**  

Los ciclos `for` permiten repetir instrucciones múltiples veces sin necesidad de escribirlas una por una.  

### **Ejemplo básico: Imprimir los números del 1 al 10**  
```python
for i in range(1, 11):
    print(i)
```
En este caso, `range(1, 11)` genera los números del 1 al 10 y `for` los imprime uno por uno.  

### **Ejemplo avanzado: Listar los productos de una tienda**  
```python
productos = ["Laptop", "Celular", "Tablet", "Auriculares"]

for producto in productos:
    print(f"Producto disponible: {producto}")
```
Aquí, `for` recorre la lista de productos y los muestra en pantalla.  

---

## **5. if/else/elif: Toma de Decisiones en un Programa ⚡**  

La estructura `if/else/elif` permite ejecutar diferentes bloques de código según las condiciones.  

### **Ejemplo básico: Determinar si un número es positivo, negativo o cero**  
```python
numero = -5

if numero > 0:
    print("El número es positivo")
elif numero < 0:
    print("El número es negativo")
else:
    print("El número es cero")
```
Aquí, el programa evalúa si `numero` es mayor que 0, menor que 0 o igual a 0 y responde en consecuencia.  

---

## **6. Funciones y Parámetros: Modularidad en el Código 🎭**  

Las funciones permiten agrupar código en bloques reutilizables.  

### **Ejemplo básico: Función para calcular el área de un triángulo**  
```python
def calcular_area_triangulo(base, altura):
    return (base * altura) / 2

print(calcular_area_triangulo(5, 10))  # 25.0
```
Aquí definimos una función `calcular_area_triangulo` que recibe dos parámetros y devuelve el área del triángulo.  

### **Ejemplo en la vida real: Sistema de facturación**  
```python
def calcular_precio_total(precio_unitario, cantidad):
    return precio_unitario * cantidad

producto = "Zapatos"
precio = 120000
cantidad = 3
total = calcular_precio_total(precio, cantidad)

print(f"Producto: {producto}")
print(f"Cantidad: {cantidad}")
print(f"Precio Total: {total} COP")
```
Aquí la función `calcular_precio_total` nos ayuda a calcular fácilmente el precio total de una compra.  

---

