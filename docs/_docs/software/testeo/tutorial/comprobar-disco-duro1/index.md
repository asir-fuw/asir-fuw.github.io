---
title: Comprobar el estado y la integridad de un disco duro
---

## Comprobar el estado de un disco duro

### Tecnología S.M.A.R.T.

La tecnología **SMART** *(Self Monitoring Analysis and Reporting Technology)*, consiste en la capacidad de detección de fallos del disco duro.

La detección con anticipación de los fallos en la superficie permite al usuario el poder realizar una copia de su contenido, o reemplazar el disco, antes de que se produzca una pérdida de datos irrecuperable.

Este tipo de tecnología tiene que ser compatible con la *BIOS* del equipo, estar activada y, además, que el propio disco duro sea compatible. 

Monitoriza los diferentes parámetros del disco, como pueden ser la velocidad de los platos del disco, sectores defectuosos, errores de calibración, temperatura del disco, etc...

### CrystalDiskInfo

Es una aplicación para sistemas Windows que se encarga de leer los valores del S.M.A.R.T. que almacenan los discos duros sobre su funcionamiento, y permite conocer el estado de salud de los mismos, pudiendo saber si el disco está funcionando correctamente o si su final se encuentra próximo.

#### 1. Descarga

**Enlace para descargar el programa:** https://crystalmark.info/en/software/crystaldiskinfo

Accedemos a la web para descargar el programa, y tendremos la posibilidad de descargar 3 ediciones distintas del programa: *Standard Edition, Shizuki Edition y Kuro Kei Edition*.

![](imagenes\captura005.PNG)

Básicamente no hay diferencia en cuanto a funcionalidad se refiere, únicamente hay diferencias en la interfaz del programa. Para este tutorial descargaremos la edición estándar

Haciendo click en el botón que se encuentra debajo de la sección *"Quick Download"* nos redirigirá directamente a la descarga del programa, que comenzará automáticamente y guardamos el instalador.

![](imagenes\captura006.PNG)

#### 2. Instalación

Ejecutamos el instalador y comenzamos la instalación con normalidad, seleccionando el idioma, aceptando los términos de licencia, seleccionando la ruta de instalación, si deseamos carpeta en el menú o acceso directo en el escritorio, e instalamos.

![](imagenes\captura007.PNG)

![](imagenes\captura008.PNG)

![](imagenes\captura009.PNG)

![](imagenes\captura010.PNG)

![](imagenes\captura011.PNG)

![](imagenes\captura012.PNG)

#### 3. Uso

Abrimos el programa una vez haya finalizado la instalación, y tendremos la siguiente ventana:

![](imagenes\captura001.PNG)

![](imagenes\captura002.PNG)

El programa es muy sencillo de entender: tenemos una lista de parámetros SMART con una serie de valores. A la izquierda tenemos un círculo que indica el estado de ese parámetro en nuestro disco duro, cuyo color dependerá del estado en el que se encuentre nuestro disco duro:

| Color    | Descripción                                                  |
| -------- | ------------------------------------------------------------ |
| Azul     | Indica un estado óptimo en el parámetro del disco duro       |
| Amarillo | Indica que nuestro disco podría fallar en un momento no muy lejano, por lo que tendríamos que copiar nuestros archivos a otro disco para evitar la pérdida de datos |
| Rojo     | Indica que nuestro disco podría fallar inminentemente, por lo que tenemos que sacar con urgencia los datos del disco |

> Esta leyenda se puede aplicar también a la temperatura y al estado de salud que aparecen en el programa.

## Realizar análisis de superficie del disco para comprobar su integridad

Un análisis de superficie del disco se usa para ver si nuestro disco duro tiene algún problema que nos esté perjudicando en nuestro ordenador, ya sea por pantallazos azules de Windows, que no inicie el sistema, que se quede congelado en cualquier momento, etc.

### SeaTools

Para realizar esta tarea de manera sencilla usaremos el programa **SeaTools**, que nos garantiza total seguridad del sistema. Dicho programa pertenece a la empresa Seagate, marca famosa por vender discos duros.

Nos permite realizar el chequeo del disco de dos maneras: 1) cargando en un pendrive o en un CD/DVD-ROM el programa para que iniciar el equipo, o 2) a través de un programa que podemos instalar en cualquier sistema operativo Windows desde XP hasta Windows 10.

#### Instalación

1. Nos vamos a la página oficial para descargar el software:

   [https://www.seagate.com/es/es/support/downloads/seatools/seatools-win-master/](https://www.seagate.com/es/es/support/downloads/seatools/seatools-win-master/)

2. Bajamos un poco en la página hasta donde dice "Instrucciones" y damos clic en el botón azul que dice "Descargar"

	![](imagenes/imagen1.png)

3. Cuando termine, hacemos clic en la descarga para ejecutar la instalación del programa

	![](imagenes/imagen2.png)

4. En el asistente de instalación pulsamos "Siguiente", aceptamos los términos de licencia y continuamos pulsando "Siguiente" hasta completa la instalación:

	![](imagenes/imagen3.png)

	![](imagenes/imagen4.png)

	![](imagenes/imagen5.png)

#### Pasos para realizar el chequeo de disco

1. Una vez abierto el programa nos habrá chequeado todos los discos que tenemos en el equipo 

	![](imagenes/imagen6.png)

2. Para hacer una acción, tendremos que marcarlo en la casilla y en "Pruebas Básicas" seleccionar Reparar todas > Reparar Larga o Corta. En mi caso como el disco duro de este ordenador está bien, haré la prueba corta. Si tenemos un disco duro que creemos que está mal porque nos ha dado algún fallo o no va como debería haríamos primero la prueba corta para ver si nos da algún fallo, y si nos sigue sin dar fallo realizar la larga, donde lo más probable que en esta prueba sí de con el fallo por ejemplo diciendo que sector del disco duro está dañado.

	![](imagenes/imagen7.png)

3. Una vez dado, a la derecha nos dirá qué plan de chequeo hemos seleccionado y el proceso que le queda para acabar en porcentaje:

   ![](imagenes/imagen8.png)

4. Una vez que acabe nos aparecerá al 100%, y en caso de fallo nos mostraría el error. 

   ![](imagenes/imagen9.png)

Y con estos pasos simples concluye el tutorial de como chequear un disco duro.

> Sistema Operativo: Windows 10 Home 64 bits
> CPU: Intel Core i5 7200U @ 2.50GHz
> RAM: 8,00GB Único-Canal DDR3
> Placa base: Acer Gemini_SK
> Gráfica: Intel HD Graphics 620
> Almacenamiento: 931GB Seagate

## Autores

* Daniel Adán González
* Rubén Pablo Jorge Díaz