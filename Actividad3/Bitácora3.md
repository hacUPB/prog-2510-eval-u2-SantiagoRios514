# Algoritmos

## Símbolos que se utilizan para representar cada operación de un algoritmo con un diagrama de flujo

![simbolos de diagrama de flujo](images/desktop_32c5e113-9fda-4387-ac19-a648c431b4b7.gif)

## Algoritmo para empresa

![ejercicio 2](images/Ejercicio2.png)

## Ejercicios

### Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo

**Pseudocódigo:**

```pseudo
Inicio
Leer nLapices
Si nLapices >= 1000
    Hacer costo = 85
Si no
    Hacer costo = 90
Fin Si
Hacer valorTotal = nLapices * costo
Escribir "El valor total de los lápices es: ", valorTotal
Fin
```

**Diagrama de flujo:**

![Ejercicio3](images/Diagrama2.png)

**Código:**

```py
nLapices = int(input("Ingresa la cantidad de lápices a comprar: "))

if nLapices >= 1000:
    total = 85 * nLapices
else:
    total = 90 * nLapices
print("El valor de los lápices es: $", total)
```

### Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo

**Pseudocódigo:**

```pseudo
Inicio
Leer valorCompra
Si valorCompra > 250000
    Hacer descuento = valorCompra * 0.15
Si no
    Hacer descuento = valorCompra * 0.08
Hacer valorFinal = valorCompra - descuento
Escribir "El valor final de la compra es: $", valorFinal
Escribir "El descuento fue de: $", descuento
Fin
```

**Diagrama de flujo:**
![alt text](images/Diagrama3.png)

**Código:**

```py
valorCompra = int(input("Ingrese el valor de la compra: "))

if valorCompra > 250000:
    descuento = valorCompra * 0.15
else:
    descuento = valorCompra * 0.08

valorFinal = valorCompra - descuento

print("El valor final de la compra es:", valorFinal, "y el descuento aplicado fue de:", descuento)
```

### El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos

**Pseudocódigo:**

```pseudo
Inicio
Leer nAlumnos
Si nAlumnos < 30
    total = 4000
    precio = total / nAlumnos
Si no
    Si nAlumnos < 50
        precio = 95
    Si no
        Si nAlumnos < 100
            precio = 70
        Si no
            precio = 65
        Fin si
    Fin si
    total = precio * nAlumnos
Fin si
Escribir precio, total
```

## Bucles

### Ejemplo 1

```py
suma = 0
cont = 1 
while cont <= 10:
    valor = int(input("Ingrese el valor: "))
    suma = suma + valor
    cont = cont + 1
print(f"La suma es: {suma}")
```

### Ejemplo 2

```py
suma = 0
for cont in range(1,11,1):
    valor = int(input("Ingrese el valor: "))
    suma = suma + valor
print(f"La suma es: {suma}")
```

### Un profesor tiene un salario inicial de $1500, y recibe un incremento de 10% anual durante 6 años. ¿Cuál es su salario al cabo de 6 años? ¿Qué salario ha recibido en cada uno de los 6 años?

#### Análisis

1. Variables de entrada** No hay

2. Variables de salida

    - `salario` : El salario del profesor en cada año.

3. Constantes

    - `salario_inicial` = 1500
    - `incremento` = 0.1
    - `años` = 6

4. Otras variables

    - `c` : El contador en la función `for`

5. Ecuaciones

    - $\textnormal{salario} = \textnormal{salario} + (\textnormal{salario} \cdot \textnormal{incremento})$

#### Pseudocódigo

```pseudo
Inicio
salario_inicial = 1500
incremento = 0.1
años = 6
Desde c = 0 hasta c = años
    salario = salario_inicial
    Escribir "El salario el año", c, "Es de ", salario
    salario = salario * incremento
Fin desde
Fin
```

#### Código en Python

```py
salario_inicial = 1500
incremento = 0.1
años = 6
salario = salario_inicial + (salario_inicial * incremento) 
for c in range (1,años,1):
    print(f"El salario el año {c} es de {salario}")
    salario = salario + (salario * incremento)
print(f"El salario al cabo de los 6 años es {salario}")
```

### “El náufrago satisfecho” ofrece hamburguesas sencillas (S), dobles (D) y triples (T), las cuales tienen un costo de $20, $25 y $28 respectivamente La empresa acepta tarjetas de crédito con un cargo de 5 % sobre la compra. Suponiendo que los clientes adquieren N hamburguesas, las cuales pueden ser de diferente tipo_hamburguesa, realice un algoritmo para determinar cuánto deben pagar

#### Analisis

1. Variables de entrada

    - `N` : Número de hamburguesas que se van a comprar
    - `tipo_hamburguesa` : El tipo de hamburguesa que se va a comprar
    - `cantidad_hamburguesa` : La cantidad de ese tipo de hamburguesa que se va a comprar

2. Variables de salida

    - `total`

3. Constantes

    - `precio_S` = 20
    - `precio_D` = 25
    - `precio_T` = 28
    - `cargo` = 0.05

4. Otras variables

    - `N`
    - `c` : El contador en la función `Desde`

5. Ecuaciones

    - total = total + (cantidad_hamburguesa * precio_S)
    - total = total + (cantidad_hamburguesa * precio_D)
    - total = total + (cantidad_hamburguesa * precio_T)
    - c = c + cantidad_hamburguesa
    - total = total + (total * cargo)

#### Pseudocodigo

```pseudo
Inicio
precio_S = 20
precio_D = 25
precio_T = 28
cargo = 0.05
total = 0
Leer N
c = 0

Mientras c < N
    Leer tipo_hamburguesa
    Leer cantidad_hamburguesa
        Si tipo_hamburguesa = S
            total = total + (cantidad_hamburguesa * precio_S)
            c = c + cantidad_hamburguesa
        Si no Si tipo_hamburguesa = D
            total = total + (cantidad_hamburguesa * precio_D)
            c = c + cantidad_hamburguesa
        Si no Si tipo_hamburguesa = T
            total = total + (cantidad_hamburguesa * precio_T)
            c = c + cantidad_hamburguesa
        Si no
            Escribir "Tipo de hamburguesa inválido"
        Fin Si
Fin Mientras

Leer pago_con_tarjeta
Si pago_con_tarjeta = 1
    total = total + (total * cargo)
Fin Si

Escribir "El total a pagar es de: $", total
```

## Actividad final

### Identificar Algoritmos

*Responde si los siguientes enunciados representan un algoritmo. Justifica la respuesta:*

1. **Una página web:** No es un algoritmo ya que no necesariamente tiene que tener una forma de resolver un problema en específico.
2. **Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir:** Sí es un algoritmo, ya que resuelve el problema de hacer el pastel a través de una serie de pasos lógicos y estructurados.
3. **"Piensa en un número y multiplícalo por otro":** Sí es un algoritmo ya que te dan una serie de pasos a seguir, con el fin de encontrar un nuevo número.
4. **Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro:** Sí es un algoritmo, ya que te permite armar correctamente el mueble a través de una serie de pasos lógicos.
5. **Una lista de compras organizada en orden alfabético:** No es un algoritmo, ya que aunque tiene un orden establecido, no da pasos lógicos para resolver un problema.

### Variables y Constantes

*Indica si las siguientes afirmaciones describen una variable o una constante:*

1. **El valor de la gravedad en la Tierra, 9.8 m/s:** Es una constante.
2. **La edad de una persona calculada en base al año actual y su año de nacimiento:** Es una variable.
3. **La cantidad de dinero en una cuenta bancaria:** Es una variable.
4. **La velocidad de la luz en el vacío, 299,792,458 m/s:** Es una constante.
5. **El radio de un círculo:** Es una variable.

### Características de los algoritmos

*Responde si los siguientes enunciados cumplen con las características de un algoritmo. Justifica la respuesta:*

1. **Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños:** No cumple con las características de un algoritmo, ya que no se define de manera precisa qué significa "suficientemente pequeño", por lo que no se puede saber cuando terminará el proceso.
2. **Suma los números ingresados y muestra el resultado:** Sí cumple con las características de un algoritmo, ya que especifica de forma precisa los pasos a seguir y el momento a terminar.
3. **Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura:** No cumple con las características de un algoritmo, ya que no se define cuáles son los pasos para calcular el área de este rectángulo, ni cómo se ingresarán esos datos dados.
4. **El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1:** No cumple con las características de los algoritmos, ya que no es claro en cómo se contarán estos votos, ni cómo ni dónde se recopilan los datos de los votos. Además, no es claro cuál es la utilidad del número -1 en este caso.

### Comprensión de Herramientas

*Indica si las siguientes afirmaciones son ciertas o falsas respecto al pseudocódigo y diagramas de flujo:*

1. **El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas:** Falso
2. **Los diagramas de flujo son una representación gráfica de un algoritmo:** Verdadero
3. **El pseudocódigo debe estar escrito en un lenguaje de programación específico:** Falso
4. **Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos:** Verdadero

### Estructuras de Control

*Describe para qué sirven las estructuras de control. Redacta dos ejemplos, uno de tu vida diaria, es decir cuando tienes que tomar decisiones en tus actividades diarias y oto ejemplo en el que se tengan que utilizar cálculos matemáticos para tomar una u otra decisión.*

Las estructuras de control sirven para organizar los algoritmos según la necesidad de los pasos a seguir.

Por ejemplo, en mi vida yo puedo utilizar una estructura de control cuando reviso la hora a la que debo dormir según el horario del siguiente día, si la primera clase es a las 6:00, entonces debo dormirme antes de las 10:00. De lo contrario, puedo quedarme despierto hasta alrededor de las 11:30

Otro ejemplo que involucra cálculos matemáticos al tomar la decisión puede ser un algoritmo que clasifique números según si son pares o impares, en este caso, si el residuo de un número al dividirlo entre 2 es 0, quiere decir que es par, de lo contrario, es impar.
