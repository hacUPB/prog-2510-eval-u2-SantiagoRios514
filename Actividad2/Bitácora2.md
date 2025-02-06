# Actividad 2: Bitácora

## Ejercicio 1

1 bit de información puede representar 2 estados, `0` y `1`

2 bits de información pueden representar 4 estados, `00`, `01`, `10` y `11`

3 bits de información pueden representar 8 estados, `000`, `001`, `010`, `011`, `100`, `101`, `110` y `111`

Siguiendo con esta secuencia, usando $n$ bits de información se pueden representar $2^{n}$ estados totales.

## 📤 Para la bitácora

### ¿Cómo se representan los datos en una computadora?

Los datos en un computador se representan usando bytes según una codificación definida. Por ejemplo, con la tabla `ASCII` se pueden representar todos los números y letras posibles almacenándolos según los códigos de la tabla.

### ¿Cuáles son las unidades de almacenamiento de datos que se utilizan en computación?

|Unidad|Tamaño|
|------|------|
|Bit||
|Byte (B)|8 Bits|
|Kilobyte (KB)|1024 B|
|Megabyte (MB)|1024 KB|
|Gigabyte (GB)|1024 MB|
|Terabyte (TB)|1024 GB|

### La importancia del trabajo de George Bool en este tópico

El trabajo de George Bool permitió usar fácilmente los valores binarios en computación. Gracias a él, se hacen operaciones entre valores binarios en computación.

## 📤 Ejercicio 2 - Convertir a sistema `Decimal` los siguientes valores binarios

- $1010101010_2$

  $2^{1}+2^{3}+2^{5}+2^{7}+2^{9}=512+128+32+8+2=682_{10}$

- $11111_2$

  $2^{0}+2^{1}+2^{2}+2^{3}+2^{4}+2^{5}=1+2+4+8+16+32=63_{10}$

- $10000000_2$
- $100100100_2$
- $111000_2$

## 📤 Ejercicio 3 - Convertir a sistema `Binario` los siguientes valores decimales

- $127_{10}$

  |128|64|32|16|8|4|2|1|
  |---|--|--|--|-|-|-|-|
  |0|1|1|1|1|1|1|1|
  
  $127_{10}=1111111_2$

- $246_{10}$

  |128|64|32|16|8|4|2|1|
  |---|--|--|--|-|-|-|-|
  |1|1|1|1|0|1|1|0|
  
  $246_{10}=11110110_{2}$

- $1025_{10}$

  |1024|256|128|64|32|16|8|4|2|1|
  |----|---|---|--|--|--|-|-|-|-|
  |1|0|0|0|0|0|0|0|0|1|

  $1025_{10}=1000000001_{2}$

- $354_{10}$

  |256|128|64|32|16|8|4|2|1|
  |---|---|--|--|--|-|-|-|-|
  |1|0|1|1|0|0|0|1|0|

  $354_{10}=101100010_{2}$

- $187_{10}$

  |128|64|32|16|8|4|2|1|
  |---|--|--|--|-|-|-|-|
  |1|0|1|1|1|0|1|1|


## Tipos de Datos

### Diferentes tipos de datos que se utilizan en varios lenguajes de programación

||Enteros|Punto Flotante|String|Booleano|Char|
|-|------|--------------|------|--------|----|
|Python|SI|
|C y C++|SI|
|Java|SI|
|JavaScript|SI|
|C#|SI|
|Swift|SI|
|Ruby|SI|
|PHP|SI|
