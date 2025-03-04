# Bitácora 4

## Reto Final

### Se requiere obtener la distancia entre dos puntos en el plano cartesiano

```pseudo
Inicio
Leer x_1, x_2, y_1, y_2
D = sqrt((x_2 - x_1)^2+(y_2 - y_1)^2)
Imprimir D
Fin
```

```py
import math # Se importa el módulo de matemáticas para usar la función raíz cuadrada

# Se pide al usuario los puntos a los que se le calculará la distancia
x_1 = int(input("Ingrese la coordenada en x del primer punto: "))
y_1 = int(input("Ingrese la coordenada en y del primer punto: "))
x_2 = int(input("Ingrese la coordenada en x del segundo punto: "))
y_2 = int(input("Ingrese la coordenada en y del segundo punto: "))

D = math.sqrt((x_2 - x_1)**2+(y_2 - y_1)**2) # Se calcula la distancia entre los dos puntos
print(f"La distancia entre los dos puntos es: {D}") # Se imprime el resultado
```

### Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero. Para cada pedido, tiene que proporcionar las medidas de la tela en pulgadas, pero ella generalmente las tiene en metros. (1 pulgada = 0.0254 m)

```pseudo
Inicio
m_in = 0.0254
Leer medida
medida_in = medida * m_in
Imprimir medida_in
Fin
```

```py
m_in = 0.0254 # Se fija la constante del factor de conversión
medida = int(input("Ingrese la medida de la tela en metros: ")) #Se pide la medida en metros
medida_in = medida / m_in # Se calcula la distancia en pulgadas
print(f"La medida ingresada en pulgadas es: {medida_in}") # Se imprime el resultado
```

### Se requiere determinar la hipotenusa de un triángulo rectángulo

```pseudo
Inicio
Leer c1, c2
h = sqrt((c1)^2+(c2)^2)
Imprimir h
Fin
```

```py
import math #Se importa el módulo de matemáticas para usar la función raíz cuadrada

# Se pide al usuario dar las medidas de los dos catetos del triángulo
c1 = int(input("Ingrese la medida del primer cateto: "))
c2 = int(input("Ingrese la medida del segundo cateto: "))

h = math.sqrt(c1**2 + c2**2) # Se calcula la medida de la hipotenusa
print(f"La medida de la hipotenusa del triángulo es: {h}") # Se imprime el resultado
```

### Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año

- Diseñe un algoritmo que permita calcular la edad de la persona.

- Dentro de la solución, determine si la persona ya celebró su cumpleaños este año o si aún no lo ha hecho.

- Verifique si la fecha actual corresponde al día de su cumpleaños. De ser así, imprima el mensaje “Feliz Cumpleaños”.

```pseudo
Inicio
Leer dia_h, mes_h, ano_h, dia_c, mes_c, ano_c
celebro = 0
edad = ano_h - ano_c
Si mes_h < mes_c
    edad = edad - 1
Si no Si mes_h = mes_c
    Si dia_h < dia_c
        edad = edad - 1
    Si no Si dia_h = dia_c
        Imprimir "Feliz cumpleaños!🥳🎉"
    Si no
        celebro = 1
    Fin Si
Si no
    celebro = 1
Fin si
Imprimir edad
Si celebro = 1
    Imprimir "El usuario ya cumplió años este año"
Fin si
Fin
```

```py
# Se pide al usuario que ingrese la fecha de hoy
dia_h = int(input("Ingrese el día que es hoy: "))
mes_h = int(input("Ingrese el mes que es hoy: "))
ano_h = int(input("Ingrese el año que es hoy: "))

# Se pide al usuario que ingrese la fecha en la que nació
dia_c = int(input("Ingrese el día en el que nació: "))
mes_c = int(input("Ingrese el mes en el que nació: "))
ano_c = int(input("Ingrese el año en el que nació: "))

celebro = 0 # Se fija la variable que indica si ya se celebró el cumpleaños en cero
edad = ano_h - ano_c # Se calcula un aproximado inicial para la edad del usuario

# Se inicia el ciclo en el que se revisa que la edad sea correcta
if mes_h < mes_c: # El mes del cumpleaños no ha ocurrido, la edad está errada por un año
    edad = edad - 1 
elif mes_h == mes_c: # El mes del cumpleaños es este mismo mes
    if dia_h < dia_c: # El día del cumpleaños no ha ocurrido, la edad está errada por un año
        edad = edad - 1
    elif dia_h == dia_c: # El día del cumpleaños es hoy, el usuario está cumpliendo años
        print("Feliz cumpleaños!🥳🎉")
    else: # El día del cumpleaños ya ocurrió
        celebro = 1
else: # El mes del cumpleaños ya ocurrió
    celebro = 1

print(f"El usuario tiene {edad} años") # Se imprime la edad real del usuario

# En el caso que el cumpleaños ya haya ocurrido, se indica
if celebro == 1: 
    print("El usuario ya cumplió años este año")
```

### Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar más de 50 horas no está permitido

```pseudo
Inicio
horas_normal = 0
horas_doble = 0
horas_triple = 0
Leer horas, sueldoH
Si 47 <= horas <= 50
    horas_normal = 45
    horas_doble = 5
    horas_triple = horas - 45
Si no si 41 <= horas <= 45
    horas_normal = 45
    horas_doble = horas - 40
Si no si horas <= 40
    horas_normal = horas
Si no
    Imprimir "Número de horas inválido"
sueldoS = (horas_normal * sueldoH) + (horas_doble * sueldoH * 2) + (horas_triple * sueldoH * 3)
Si horas <= 50
    Imprimir sueldoS
Fin
```

```py
# Se pide al usuario la cantidad de horas trabajadas y cuánto es el pago habitual por hora
horas = int(input("Ingrese la cantidad de horas trabajadas: "))
pago_hora = int(input("Ingrese el pago por hora: "))

# Se inician las horas por cada tipo de pago en cero
horas_normal = 0
horas_doble = 0
horas_triple = 0

# Se inicia el ciclo en el que, dependiendo de la cantidad de horas, se da un valor al sueldo
if 46 <= horas <= 50: # Si la cantidad de horas está entre 46 y 50, se calcula la cantidad de horas pagadas al triple
  horas_normal = 45
  horas_doble = 5
  horas_triple = horas - 45
elif 41 <= horas <= 45: # Si la cantidad de horas está entre 41 y 45 se calcula la cantidad de horas pagadas al doble
  horas_normal = 40
  horas_doble = horas - 40
elif horas <= 40: # Si la cantidad de horas es menor a 40, todas las horas se pagan normal
  horas_normal = horas
else:
  print("Número de horas inválido") # Si la cantidad de horas excede las 50, este es un  número inválido
sueldoS = (horas_normal * pago_hora) + (horas_doble * pago_hora * 2) + (horas_triple * pago_hora * 3) # Se calcula el pago semanal

if horas <= 50: # Se imprime el valor sólo si el valor de horas era válido
  print(f"El sueldo semanal del trabajador es de {sueldoS}")
```
