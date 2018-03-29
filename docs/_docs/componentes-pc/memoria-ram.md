---
title: Memoria RAM
author: Francisco J. Glez Pérez
---

# Memoria.

* Se denomina así a __cualquier dispositivo capaz de almacenar información y permitir recuperarla con posterioridad__.

![lobulos][1]

* Existen varios niveles de memoria en un ordenador:
   - Registros.
     + Pequeños almacenes de pocos bits dentro de la CPU.
   - Memoria caché.
     + Memoria interna a la CPU muy muy rápida pero pequeña.
   - Memoria principal.
     + _La memoria RAM, propiamente dicha_.
   - Memoria secundaria.
     + Discos duros, CD, DVD, Bluray, pendrive, tarjetas de memoria, etc.

![niveles-de-memoria][2]


# Memoria RAM.

* Acrónimo de __Random Access Memory__.
* Por sus _características_, se utiliza como _memoria principal_.
   - Almacena __datos y las instrucciones__ de los programas en ejecución.
* Se utilizan memorias de tipo RAM porque …
   - Se pueden leer y escribir con rapidez.
   - Aunque son __volátiles__, y pierden sus datos al apagar el ordenador.
* Su capacidad se mide en Gigabytes (GB).
* Actualmente se usan las memorias de tipo SDRAM (Synchronous Dynamic RAM).
   – SDR SDRAM, DDR, DDR2, DDR3, …


## Módulo de memoria RAM.

* La memoria RAM se distribuye en forma de __módulos de memoria__.
> Esto es lo que se llama el __encapsulado__.

* Módulo de memoria:
   – Chips rectangulares negros soldados a unas plaquitas.
   – Estos chips contienen componentes electrónicos que forman las “celdas” donde se almacenan los bits (0s y 1s).

   ![Modulo de memoria RAM][3]![Esquema de un chip de memoria][4]


## Controlador de memoria.

* En inglés, MMU (Memory Management Unit).
* Dispositivo que controla __el intercambio de datos entre la memoria y el  microprocesador__.
   – También con otros elementos del PC (dispositivos con DMA, acceso directo a memoria).
* _Antiguamente_:
   – Controlador de memoria en el puente norte (chip de la placa base).
   – El bus que lo comunica con la memoria se llama FSB (bus del sistema o Front Side Bus).

![Esquema de MMU antiguo][5]

* _Actualmente_:
   – Controlador de memoria dentro del microprocesador.
   – Mejora la velocidad de acceso a memoria.
   – El bus que lo comunica con la memoria se llama HyperTransport (AMD) o QPI (Intel).

![Esquema de MMU actual][6]


## Bus de memoria.

![Simil de un bus][7]

* El bus se divide en:
   –  __Bus de direcciones__:
     + Para enviar las direcciones de memoria y localizar los datos.
     + Dependiendo de su ancho de bits:
        – 20 bits hasta 1MB (en CPUs de 16 bits).
        – 32 bits hasta 4GB (en CPUs de 32 bits).
        – 44 bits hasta 16TB = 16384 GB (en CPUs de 64 bits).
        – Según la arquitectura.
        –  __Bus de datos__:
     + Para transferir los datos.
     + Cuanto más ancho de bits, más datos se podrán transmitir en un ciclo de reloj.
        – A más carriles en la autopista, más coches por segundo.
     + Ancho de bits: actualmente de 64 bits.
        – 8 bytes pos ciclo de reloj.
> * Ejemplo: si reloj a 400MHz
	– 400.000.000 ciclos/seg * 8 bytes =
	= 3.200.000.000 bytes/seg = 3,2GB/s aprox.


## Parámetros fundamentales de las RAM.

	* Velocidad de acceso.
	* Latencias.
	* Ancho de banda (Doble Canal / Triple Canal).
	* Voltaje.
	* Buffered y Unbuffered.


### Velocidad de acceso (ns y MHz).
* Ciclo de memoria.
   – Proceso de __acceso a memoria para lectura o escritura__.
   – Éste lleva cierto tiempo.
     + Debido al funcionamiento de los elementos electrónicos de la memoria (cargas y descargas de condensadores, propagación de señales de control, etc.).
* __Tiempo mínimo en realizar un acceso a memoria se mide en nanosegundos__ (1 ns = 10-9 segundos = 0,000000001 segundos).
   – Cuando menos tiempo necesite un ciclo de acceso más rápida será la memoria.
* Las memorias __síncronas__ funcionan a una __cierta velocidad del bus del sistema__ (sincronizadas con el reloj del sistema).
   – La unidad de medida que suele emplearse son los MHz (megahercios), y no los nanosegundos.
   – Podemos calcular los “ns” a partir de los MHz y viceversa.


#### Cómo calcular la velocidad de acceso.

> Ejemplo: Memoria PC-133
	– Memoria de tipo SDRAM.
	– Velocidad de bus a 133MHz (por eso se denomina PC-133).
	– Velocidad de acceso = 1/133.000.000 = 7,5·10-9 segundos = 7,5 ns

> Ejemplo: Memoria DDR-266
	– Memoria de tipo DDR SDRAM (Double Data Rate).
		+ Significa que aprovecha el doble cada ciclo de reloj.
	– Velocidad de bus a 133MHz (la misma de antes).
		+ Ojo, también se le puede denominar PC2100, por su tasa de transferencia de 2133MB/s.
	– Velocidad efectiva de 266 MHz (por eso se denomina DDR-266).
	– Velocidad de acceso = 1/266.000.000 = 3,76 ns

> Ejemplo: Memoria DDR2-1066
	 – Memoria de tipo DDR2 SDRAM (también doble aprovechamiento de cada ciclo, pero funciona a velocidades de bus reales superiores a DDR).
	 – Velocidad de bus a 533MHz
	 – Velocidad efectiva de 1066MHz
	 – Velocidad de acceso = 1/1.066.000.000 = 0,9 ns


### Latencias.

* Son __retardos__ o retrasos que se producen __durante el acceso a la memoria__.
   – Por lo tanto, cuanto _menores_ sean, _mejor_.
* __Designación técnica__ empleada en los módulos de memoria:
   – __CAS-tRCD-tRP-tRAS__, por ejemplo “8-8-7-24”.
*  __Se miden en ciclos de reloj__, y son valores mínimos.
   > Ejemplo: Si CAS=5 (CL=5) significa que hay que darle al menos 5 ciclos de reloj para que funcione bien; menos es arriesgado.

* La latencia más importante es la __latencia CAS (CL = CAS Latency)__.
   – CAS es el acrónimo de “Column Access Strobe”.
   – Único retardo inevitable en todo acceso a memoria.
   – Las otras latencias no siempre se producen en todos los accesos (según la situación).
   – Memoria con menos valores de CAS es más rápida, y más cara.
   – SDRAM y DDR CAS de 3, 2.5 y 2.
   – DDR2 CAS de 5, 4 y 3.
   – DDR3 CAS de 9, 8 y 7 (a más velocidad de bus, más CAS).
* Overclocking.
   – Si aumentamos la velocidad del bus, hay que aumentar la CL para que  funcione correctamente.
   – Se puede hacer mediante la BIOS; esto siempre conlleva riesgos de inestabilidad del sistema.


#### Consultar de latencia con CPU-Z.

![Consulta de latecia CPUZ][8]


### Ancho de banda (MB/s).

* __Máxima cantidad de memoria que puede transferirse por segundo__ (MB/s ó GB/s).
* Cuanto __más, mejor__.
* Cómo se calcula:
   – Ancho de banda = VE x ABD / 8
     + VE = velocidad efectiva de reloj.
     + ABD = ancho del bus de datos en bits.
     + / 8 = para pasarlo a bytes.
> Ejemplo: Memoria DDR2-667
>    - Bus físico de 333MHz
>    - Velocidad de bus efectiva de 667MHz.
>    - Ancho de bus de datos de 64 bits (8 bytes).
>    - AB = 667.000.000 * 64 / 8 = 5.336.000.000 B/s = aprox. 5.300 MB/s
> > Por eso también se la denomina PC-5300.


### Dual-Channel y Triple-Channel.

* **Dual-Channel (Doble canal)**.
   – Tecnología que permite a la CPU acceder a dos módulos de memoria de forma simultánea (2 canales).
   – Se duplica el ancho de banda (tasa de transferencia de datos) .
     + 128 bits por transferencia (64 bits x 2).
         – Son necesarios al menos 2 módulos (o un número par) de memoria __idénticos__.
           – Aparece con las memorias DDR, también lo encontramos en DDR2 y DDR3.
     + DDR3-1066MHz 8500 MB/s x 2 = 17 GB/s
* **Triple-Channel (Triple canal)**.
   – Permite el acceso a tres módulos de memoria de forma simultánea (3 canales).
   – Triplica el ancho de banda.
     + 192 bits por transferencia (64 bits x 3).
         – Necesitamos 3 módulos de memoria (o un nº múltiplo de 3) __idénticos__.
           – Reciente: en los Intel Core i7 (9xx), Triple-Channel DDR3.
     + DDR3-1066MHz 8500 MB/s x 3 = 25.5 GB/s.


### Voltaje.

* Depende del tipo de memoria.
   – Voltaje nominal es el indicado por el fabricante.
* Voltaje superior al nominal, más consumo y más temperatura.
   – Mejora la estabilidad si estamos haciendo overclocking (práctica peligrosa).
* Módulos de alto rendimiento.
   – Ofrecidos por algunos fabricantes.
   – Funcionan a más MHz.
   – Requieren mayor voltaje.
   – Disponen de sistemas de refrigeración mejorados (disipadores).
* Usar con cuidado: Intel avisa que MMU dentro del micro, voltaje 5% superior al nominal puede dañar el microprocesador.


### Voltajes nominales según tipo de memoria.

![Tabla de voltajes nominales][9]

/* Se debería actualizar la imagen por una tabla y añadir las DDR4 */


### Buffered y Unbuffered.

* **Buffered**.
  * También se les denomina Registered.
  * Tienen registros intermedios entre la CPU y la propia memoria.
  * Aumenta la fiabilidad del sistema.
  * Pero retarda los tiempos de transferencia.
  * Se suelen usar en servidores donde es muy importante la integridad de los datos.
* **Unbuffered**.
  * Se comunican directamente con la CPU.
  * Memoria más rápida pero menos segura.


## Tipos de memoria RAM.

	* SRAM.
	* DRAM.
	* SDRAM.
	* DDR.
	* DDR2.
	* DDR3.


### SRAM (Static RAM).

* *Memoria RAM estática*.
* Mantiene la información siempre que no se interrumpa la alimentación eléctrica.
* Con respecto a las DRAM:
   – Son más rápidas.
   – Pero …
     + Son de mayor tamaño (ocupan más espacio físico).
     + Son más caras.
     + Tienen menos capacidad.
* Se suelen utilizar como memoria caché de la CPU, y no como memoria principal.


### DRAM (Dynamic RAM).

* *Memoria RAM dinámica*.
* Su contenido se reescribe (refresca) continuamente porque se va degradando.
* Se utiliza como memoria principal.
* Las primeras fueron asíncronas (iban a su ritmo).
   – FPM (Fast Page Mode).
   – EDO y BEDO RAM.
* Con respecto a las SRAM:
   – Son más lentas.
   – Pero …
     + Son de menor tamaño (ocupan menos espacio físico).
     + Son más baratas.
     + Tienen más capacidad.


### SDRAM (Synchronous DRAM).

* *DRAM síncrona*.
   – Memoria sincronizada con el reloj del sistema (la del FSB).
   – Antes la memoria iba a su ritmo y provocaba esperas a la CPU.
* También se les llama SDR SDRAM.
   – Single Data Rate SDRAM.
* Ancho de banda de 64 bits.
   – En cada Hz (ciclo) envía 64 bits (8 bytes).
* Las encontramos en módulos DIMM de 168 pines.
* Tipos más comunes:
   – __PC100__: 8 bytes/Hz x 100 MHz = aprox. 800 MB/s
   – __PC133__: 8 bytes/Hz x 133 MHz = aprox. 1066 MB/s


### Rambus DRAM.

* Pretendía _remplazar_ a la SDRAM.
* Memoria propietaria, __propiedad de Rambus Inc__.
* Cobraba derechos a quien la fabricara (no era un estándar libre).
* Intel la incorporó con los _Pentium III_.
* Tenía un ancho de banda de menos bits (16 y 32 bits) pero era más rápida (400MHz frente a los 133 de SDRAM).
* Se utilizó en la Playstation 2 y en la Nintendo 64.
* La DDR SDRAM la barrió del mercado.


### DDR.

* SDRAM de doble velocidad de datos.
   – DDR SDRAM (Double Data Rate SDRAM).
* Duplica la velocidad de operación, aprovechando el flanco de subida y el de bajada de la señal de reloj.
* Ancho de bus de datos de 64 bits  --> 8bytes/Hz.
* Suministrados en módulos DIMM de 184 pines.
* Tipos comunes:
   – PC1600 (DDR200): 8 bytes/Hz x 200 MHz = 1600 MB/s
   – PC2100 (DDR266): 8 bytes/Hz x 266 MHz = 2100 MB/s
   – PC2700 (DDR333): 8 bytes/Hz x 333 MHz = 2700 MB/s
   – PC3200 (DDR400): 8 bytes/Hz x 400 MHz = 3200 MB/s


### DDR2.

* Mejora respecto a DDR.
* Más velocidad y menos voltaje (se reduce consumo y calor).
* Se suministran en módulos de 240 pines.
* Capacidades de hasta 2GB por módulo.
* Ancho de bus de datos de 64 bits --> 8bytes/Hz
* Tipos comunes:
   – PC2-3200 (DDR2-400): 8 bytes/Hz x 400MHz = 3200 MB/s
   – PC2-4300 (DDR2-533): 8 bytes/Hz x 533MHz = 4264 MB/s
   – PC2-5400 (DDR2-667): 8 bytes/Hz x 667MHz = 5336 MB/s
   – PC2-6400 (DDR2-800): 8 bytes/Hz x 800MHz = 6400 MB/s


### DDR3.

* Nueva mejora respecto a DDR2.
* Mayor tasa de transferencia y menos consumo.
* Módulos de hasta 16GB.
* Se suministran en módulos de 240 pines.
* Tipos comunes:
   – PC3-6400 (DDR3-800): 8bytes/Hz x 800MHz = 6400 MB/s
   – PC3-8500 (DDR3-1066): 8bytes/Hz x 1066MHz = 8500 MB/s
   – PC3-10600 (DDR3-1333): 8bytes/Hz x 1333 MHz = 10600
   – PC3-12800 (DDR3-1600): 8bytes/Hz x 1600 MHz = 12800

/* DDR4 */


## Los módulos y las ranuras de memoria.

* **Módulo de memoria**: tarjeta de circuito impreso rectangular donde se  sueldan chips de memoria (esto se llama el encapsulado).
* Estos tienen __pines__, que hacen contacto con la placa base.
* **Ranura de memoria (slot)**: es donde se conectan los módulos de memoria, que hacen de memoria principal del ordenador.
> RECUERDA: Llamamos RAM a la memoria principal del ordenador porque es el tipo de memoria que se utiliza.

![modulos y ranuras de memoria][10]


### Ranuras de memoria.

![modulo y zocalos SIMM][11]	![Zocalos DIMM][12]


## Módulos de memoria (encapsulados).

	* SIMM.
	* DIMM.
	* DIMM DDR.
	* RIMM.
	* SO-DIMM.
	* GDDR.


### Tipos de módulos.

![Tipos de modulos de memoria][13]

* Izquierda de arriba a abajo: DIP, SIPP, SIMM 30, SIMM 72.
* Derecha de arriba a abajo: DIMM 168, DIMM 184.


### SIMM.

* Single Inline Memory Module.
   – Módulo de memoria en línea simple.
* Los pines de ambas caras están unidos.
* Los encontramos de 30 y de 72 pines.
* Encapsulado para memorias de tipo DRAM.
* Capacidades de entre 1MB y 128MB.
* Se usaron entre los 80 y los 90.


### DIMM.

* Dual Inline Memory Module.
   – Módulo de memoria en línea doble.
* Físicamente son más largos que SIMM.
* Tiene 168 pines (contactos).
* 1 muesca en cada lado y 2 entre los pines.
* Los encontramos entre 32 MB y 2 GB.
* Se utiliza para la memoria de tipo SDR SDRAM.


### DIMM DDR.

* Han ido sustituyendo a los DIMM de 168 pines.
* 2 muescas en los lados y 1 entre los pines.
* Tipos:
   – DIMM DDR: 184 pines.
   – DIMM DDR2 y DDR3: 240 pines.

![Tipos de memoria DDR][14]

* La muesca entre los pines no coincide entre los módulos (son incompatibles).


### RIMM.

* Rambus Inline Memory Module.
   – Módulo de memoria en línea Rambus.
* Formato propietario de la Rambus Inc.
* Los encontramos con 168 y 232 pines.
* Son más rápidos que los anteriores, ya que encapsulan chips de memoria de tipo RDRAM (Rambus DRAM).
* Su precio es mucho más elevado.
* Vienen con un disipador.

![modulo Rambus][15]


### Módulos de memoria para portátiles.

* **SO-DIMM**.
   – Módulos DIMM para portátiles.
   – Son más pequeñas que las DIMM.
   – Las encontramos de 100, 144 y 200 pines.

![modulo SODIMM][16]

* **SO-RIMM**.
   – Raro caso en que se usó Rambus DRAM en portátiles.

* **Micro-DIMM**.
   – Formato más pequeño que SODIMM.
   – No está muy extendido.

![modulos SO Y Micro DIMM][17]

>> Arriba: SO-DIMM / Abajo: MicroDIMM


### Tabla de módulos de memoria.

![Tabla de mosulos de memoria][18]


### Memoria para tarjetas gráficas.

* GDDR.
   – La encontramos en tarjetas gráficas y videoconsolas.
   – RAM DDR para gráficos.

![Tarjeta gráfica][19]
![Xbox One][20]	
![Play Station 4][21]










[1]: imagenes/memoria-ram/lobulos.png "Partes del cerebro"
[2]: imagenes/memoria-ram/niveles-memoria.png "Niveles de la memoria"
[3]: imagenes/memoria-ram/modulo-ram.png "Modelo de un modulo RAM"
[4]: imagenes/memoria-ram/esquema-ram.png "Esquema de una celda de un modulo"
[5]: imagenes/memoria-ram/mmu-antiguo.png "Esquema MMU antiguo"
[6]: imagenes/memoria-ram/mmu-actual.png "Esquema MMU actual"
[7]: imagenes/memoria-ram/autovia.png "Simil de un bus"
[8]: imagenes/memoria-ram/cpu-z.png "Uso de CPU-Z para consultar Latencia"
[9]: imagenes/memoria-ram/voltajes-nominales-tipos-memorias.png "Tabla de los voltajes nominales"
[10]: imagenes/memoria-ram/modulos-y-ranuras-de-memoria.png "Modulos y ranuras de memoria"
[11]: imagenes/memoria-ram/modulos-zocalos-simm.png "Modulo y zocalos SIMM"
[12]: imagenes/memoria-ram/zocalos-dimm.png "Zocalos DIMM"
[13]: imagenes/memoria-ram/tipos-modulos.png "Tipos de modulos"
[14]: imagenes/memoria-ram/dimm-ddr.png "Tipos de modulos DIMM DDR"
[15]: imagenes/memoria-ram/modulo-rimm.png "Modulo RIMM"
[16]: imagenes/memoria-ram/sodimm-200pines.png "SO-DIMM PC-2700 de 200 pines"
[17]: imagenes/memoria-ram/sodimm-y-microdimm.png "Modulos SODIMM Y MicroDIMM"
[18]: imagenes/memoria-ram/tabla-modulos.png "Tabla de mosulos de memoria"
[19]: imagenes/memoria-ram/tarjeta-grafica.png "Tarjeta gráfica"
[20]: imagenes/memoria-ram/xbox.png "Consola Xbox"
[21]: imagenes/memoria-ram/ps4.png "Consola PS4"