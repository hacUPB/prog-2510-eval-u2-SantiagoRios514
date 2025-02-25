# Problemas

## Se requiere obtener la distancia entre dos puntos en el plano cartesiano, tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo que representen el algoritmo para obtener la distancia entre esos puntos.

![Figura 1](<images/Figura1.webp>)

### Análisis

1. Variables de entrada

    - `x_1` : Coordenada en x del punto 1
    - `y_1` : Coordenada en y del punto 1
    - `x_2` : Coordenada en x del punto 2
    - `y_2` : Coordenada en y del punto 2

2. Variables de salida

    - `D` : Distancia entre el punto 1 y 2

3. Constantes no hay

4. Otras variables no hay

5. Ecuaciones

    - `D = sqrt((x_2 - x_1)^2+(y_2 - y_1)^2)`

### Pseudocódigo

```
Inicio
Leer x_1, x_2, y_1, y_2
D = sqrt((x_2 - x_1)^2+(y_2 - y_1)^2)
Imprimir D
Fin
```

### Diagrama de flujo

![Diagrama 1](images/Reto1.png)

## Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero. Para cada pedido, tiene que proporcionar las medidas de la tela en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo para ayudar a resolver el problema, determinando cuántas pulgadas debe pedir con base en los metros que requiere. Represéntelo mediante un diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).

### Análisis

1. Variables de entrada

    - `medida` : medida de la tela en metros

2. Variables de salida

    - `medida_in` : medida de la tela en pulgadas

3. Constantes

    - `m_in = 0.0254` : factor de conversión de metros a pulgadas

4. Otras variables no hay

5. Ecuaciones

    - `medida_in = medida * m_in`

### Pseudocódigo

```
Inicio
Leer medida 
m_in = 0.0254
medida_in = medida * m_in
Imprimir medida_in
Fin
```

### Diagrama de flujo

![Diagrama 2](images/Reto2.png)

## Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla?

### Análisis

1. Variables de entrada

    - `c1` : medida del cateto 1
    - `c2` : medida del cateto 2

2. Variables de salida

    - `h` : medida de la hipotenusa del triángulo

3. Constantes no hay

4. Otras variables no hay

5. Ecuaciones

    - `h = sqrt((c1)^2+(c2)^2)`

### Pseudocódigo

```
Inicio
Leer c1, c2
h = sqrt((c1)^2+(c2)^2)
Imprimir h
Fin
```

### Diagrama de flujo

![Diagrama 3](images/Reto3.png)

## Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.

- Diseñe un algoritmo que permita calcular la edad de la persona.

- Dentro de la solución, determine si la persona ya celebró su cumpleaños este año o si aún no lo ha hecho.

- Verifique si la fecha actual corresponde al día de su cumpleaños. De ser así, imprima el mensaje “Feliz Cumpleaños”.

### Análisis

1. Variables de entrada

    - `dia_h` : Día de la fecha actual
    - `mes_h` : Mes de la fecha actual
    - `ano_h` : Año de la fecha actual
    - `dia_c` : Día de la fecha del cumpleaños
    - `mes_c` : Mes de la fecha del cumpleaños
    - `ano_c` : Año de la fecha del cumpleaños

2. Variables de salida

    - `edad` : Edad calculada del usuario

3. Constantes no hay

4. Otras variables

    - `celebro` : Es un valor que dice si es verdadero o falso que el usuario ya celebró su cumpleaños este año

5. Ecuaciones

    - `edad = ano_h - ano_c`
    - `edad = edad - 1`

### Pseudocódigo

```
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
    Imprimir "El usuario ya celebró su cumpleaños este año"
Fin si
Fin
```

### Diagrama de flujo

![alt text](images/Reto4.png)
