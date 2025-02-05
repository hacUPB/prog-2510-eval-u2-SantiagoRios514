# Actividad 1: El computador digital moderno

![alt text](images/4b601ced50579e329d3b39908fa0fdf6.jpg)

## ¿Qué es un computador?

Un computador es una máquina programable que puede ejecutar una serie de comandos dados, con el fin de procesar los datos de entrada. A través de estos comandos, un computador puede ejecutar órdenes dadas por el usuario y a través de estas órdenes, el computador puede llegar a resultados que resuelvan muchas tareas distintas. 🖥️💻

[**Fuente 1**](https://concepto.de/computador/), [**Fuente 2**](https://definicion.de/computadora/#google_vignette)

## Arquitecturas de un computador

### Arquitectura CISC

El enfoque del procesador `CISC` es minimizar el número de instrucciones por programa. Los procesadores que usan esta arquitectura están diseñados para disminuir el costo de la memoria, porque los grandes programas necesitan más memoria, así necesitando que la memoria sea lo más barata posible.

Para abaratar el costo de la memoria, se reduce el número de instrucciones por programa, incrustando varias operaciones en una sola instrucción, haciendo que usen menos memoria, pero volviéndolas más complejas.

### Arquitectuar RISC

El enfoque del procesador `RISC` es la optimización, este se usa principalmente en dispositivos portátiles como los celulares, debido a su eficiencia energética.

`RISC` intenta reducir los ciclos por instrucción aumentando el número de instrucciones del programa. Para ejecutar programas, estos utilizan el *Pipelining*, este se realiza sobreponiendo varias intrucciones en su ejecución, así teniendo una ventaja de rendimiento sobre `CISC`

[**Fuente**](https://mefics.org/es/qu%C3%A9-es-la-arquitectura-risc-y-cisc-con-sus-ventajas-y-desventajas/)

## ¿Qué es el hardware?

El hardware son los componentes físicos que usa el usuario para interactuar con un computador. Estos son necesarios para hacer que el equipo funcione.

![Hardware](images/hardware-computadora_80590-1785.avif)

### CPU: Unidad Central de Procesamiento

El CPU proporciona la capacidad de programación y procesamiento. El CPU tiene algunas funciones básicas, como recolectar información, decodificarla en pedazos más pequeños y ejecutar instrucciones.

Las partes del CPU son:

#### Núcleo

Es la unidad base del CPU, interpreta y ejecuta acciones. Hoy en día, los procesadores tienen como mínimo dos núcleos.

#### Unidad de control

Es un circuito que extrae intrucciones de la memoria, la descifra y la ejecuta

#### Unidad aritmética lógica

Es un circuito que ejecuta las operaciones lógicas y matemáticas entre datos.

#### Unidad de coma flotante

Es un componente especializado para calcular operaciones con coma flotante.

#### Memoria caché

Es la memoria en la que se almacenan datos que el usuario usa frecuentemente.

#### Registros

Es una memoria de alta velocidad, que permite controlar las instrucciones que se están ejecutando

#### Controlador de memoria

Es un circuito integrado al procesador que regula el flujo de datos entre el procesador y la memoria

#### Buses

Son sistemas digitales que envían y reciben datos entre los componentes de hardware.

[**Fuente**](https://concepto.de/cpu/)

### GPU: Unidad de procesamiento de gráficos

Es un tipo de procesador que maneja y acelera la representación de gráficos. Especialmente en tareas como renderizado y modelado 3D y reproducción de gráficos de juegos en 3D.

[**Fuente**](https://es.digitaltrends.com/computadoras/que-es-la-gpu)

### Memoria

La memoria es el lugar de almacenamineto electrónico de las instrucciones y datos que se necesita acceder rápidamente.

#### Principal (RAM)

La `RAM`, o Memoria de Acceso Aleatorio, es el lugar donde se almacenan los datos que necesita el procesador en el momento, estos sólo se almacenan durante un breve periodo de tiempo. Esta memoria no se conserva cuando se apaga el computador.

#### Secundaria (HDD, SSD)

Es conocido como almacenamiento auxiliar, estos almacenan y crean copias de seguridad de datos a largo plazo, con capacidades de almacenamiento más altas y costos más bajos en comparación con la memoria principal.

#### Virtual

Es una sección de la memoria caché creada temporalmente en la unidad de almacenamiento secundaria, se utiliza cuando la `RAM` está llena.

[**Fuente**](https://www.purestorage.com/la/knowledge/what-is-computer-memory.html)

### Dispositivos de entrada o salida

También conocidos como periféricos, son dispositivos independientes al computador que permiten realizar una función extra. Sirven como complemento para las operaciones del computador

#### De entrada

Son aquellos que permiten el ingreso de datos desde el exterior, por ejemplo: mouse, teclado, micrófono, lector de CDs.

#### De salida

Son aquellos que reflejan la información desde el interior hacia el exterior, por ejemplo: monitor, altavoz, impresora.

[**Fuente**](https://www.ceupe.com/blog/periferico.html)

### Buses de datos

Los buses de datos son líneas de comunicación entre dos componentes. Los tres más importantes son: la interfaz `PCIe`, el bus `SATA` y el `USB`.

El `PCIe`, se utiliza principalmente para comunicar componentes que requieren de un ancho de banda muy grande. Principalmente se utiliza para tarjetas gráficas y unidades de almacenamiento `SSD M.2`.

El bus `SATA` se utiliza para comunicar todo tipo de unidades de almacenamiento. Y finalmente, el `USB` es el bus universal para comunicar dispositivos externos de todo tipo.

[**Fuente**](https://hardzone.es/reportajes/que-es/bus-datos-pc-cuales)

## ¿Qué es el software?

`Software` es todo componente no físico que forma parte de dispositivos digitales y que permite su funcionamiento. Pueden ser diversos tipos de programas y aplicaciones diseñados para cumplir un rol específico dentro del sistema. Los programas del `software` le dicen al `hardware` que pasos seguir para ejecutar una función.

### Software de sistema

Son los programas que dan la forma de controlar el hardware. Ofrece soporte para otros programas dentro de él, por ejemplo: sistemas operativos o servidores.

### Software de programación o desarrollo

Son programas diseñados para desarrollar programas informáticos. Permiten fácilmente desarrollar aplicaciones con un lenguaje de programación específico, por ejemplo: compíladores o editores de texto.

### Software de aplicación

Son programas diseñados para realizar una o más tareas específicas. Son casi todos los programas descargados en un computador, por ejemplo: `Microsoft Word`, `Adobe Photoshop`, `Google Chrome`.

[**Fuente**](https://concepto.de/software/)

## Funcionamiento del computador

### ¿Qué procesos se llevan a cabo cuando enciendes un computador?

Cuando se enciende un computador se llevan a cabo una serie de pasos:

1. Se inicializa la fuente de poder
2. Se inicializa el procesador
3. Se arranca la placa base
4. Se comprueba la memoria RAM
5. Se arrancan todos los buses primarios y secundarios
6. Se arranca la tarjeta gráfica
7. Se arrancan y monitorean las unidades de almacenamiento secundarias
8. Se comprueban las tarjetas de expansión conectadas
9. Se inicia la BIOS de la placa base
10. Se carga el sistema operativo

[**Fuente**](https://hardzone.es/tutoriales/montaje/arrancar-ordenador/)

### ¿Qué sucede desde que ingreso un dato a través del teclado, hasta que veo el resultado de la operación en la pantalla?

El teclado de un computador tiene un microcontrolador que tiene instalado un programa para su funcionamiento, este revisa si se está pulsando una tecla y si es el caso, envía un código de identificación al sistema operativo a través del bus, el cual lo identifica como una tecla pulsada.

[**Fuente**](https://www.etsist.upm.es/estaticos/ingeniatic/index.php/tecnologias/item/615-teclado.html)

### ¿Cómo se codifican los datos internamente en el computador?

Para optimizar y facilitar los procesos con los datos para el computador, toda la información se codifica internamente en el sistema numérico **binario**, osea, mediante dos caracteres: `1` y `0`.

Internamente, el `1` indica la presencia de corriente eléctrica y el `0` indica la ausencia de corriente eléctrica.

[**Fuente**](https://www.oposinet.com/temario-de-informatica/temario-3-informatica/tema-10-representacin-interna-de-los-datos-2/)

### ¿Cuáles son las unidades de medida de datos en un computador?

Para medir el almacenamiento de información en un computador, se utiliza la unidad base de información: el `Bit`.

Así, para seguir aumentando la cantidad, se emplea el siguiente sistema:

|Unidad|Tamaño|
|------|------|
|Bit||
|Byte (B)|8 Bits|
|Kilobyte (KB)|1024 B|
|Megabyte (MB)|1024 KB|
|Gigabyte (GB)|1024 MB|
|Terabyte (TB)|1024 GB|

[**Fuente**](https://edu.gcfglobal.org/es/cultura-tecnologica/medidas-de-almacenamiento-de-informacion/1/)


## Mapa Conceptual Resumen

![Mapa conceptual](images/Mapa_Conceptual.png)
