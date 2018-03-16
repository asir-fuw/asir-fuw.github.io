---
title: Microprocesador
---



## Introducción

- Muchas veces se da nombre al PC en función de este componente:
  - <u>Decimos</u>: este ordenador es "*un Core 2 Duo*", "*un Phenom*" o "*un i7*", o incluso "*un AMD*".
  - Es como decir que un coche es "*un Renault Clio*" o "*un Ford*".


- Coloquialmente lo llamamos el "**micro**".
- Técnicamente, la "**CPU**".
  - Central Processing Unit, Unidad Central de Proceso.


- Es un dispositivo electronico imprescindible en todo un ordenador
  - Es el "*cerebro del PC*"







## ¿Qué es el microprocesador?

- Componente principal del ordenador.
- Millones de minúsculos componentes electrónicos en un solo "chip".
  - Casi todos **transistores**
  - Tamaño del transistor
    - Hasta hace poco: 45nm
    - Muy recientemente: 25nm
  - 1nm = 1 millonésima parte de un mm
- **Se encarga de**
  - Dirigir y controlar todos los componentes
  - Realizar las operaciones aritméticas y lógicas
  - Ejecuta las instrucciones de los programas
- El primero fue fabricado por Intel, y se llamó el 4004.







## Fabricación de un micro

- Se emplean materiales **semiconductoresen** su fabricación
  - El más común es el **silicio**
  - De ahí el nombre del famoso valle californiano de Silicon Valley
    - Ahí se ubican muchas empresas de la industria de los semiconductores
- Un lingote cilíndrico de silicio puro se corta en finos discos llamados **obleas** (wafers) 
- Sobre la oblea se graba el circuito electrónico del chip mediante **fotolitografía**
  - Sobre una oblea se graban muchos micros
  - Se proyecta luz ultravioleta sobre la oblea y se "esculpe" el diseño del chip (como pintar con spray sobre una plantilla)
- Luego se depositan pequeñas impurezas (**dopado**) sobre la oblea completando el circuito
  - Esto se repite, realizando varias capas superpuestas
- Se cortan los chips individuales de la oblea, denominados "die" (o "core")
- Luego se realiza el **encapsulado**, fijándolo a una base cerámica con los conectores y colocando encima una superficie disipadora (para distribuir el calor generado por el "die")







## Encapsulado del microprocesador

- Es la **estructura externa del microprocesador**.
- <u>Protege</u> el chip (<u>die</u>) que es muy delicado.
- Evolución de los encapsulados del micro:
  - **DIP (Dual Inline Package)**
    - Clásica “cucaracha” negra, de cerámica o plástico
    - Conectores como patas rectas en sus laterales
    - Se insertan o sueldan en zócalos
    - Es el caso de Intel 8088 y 8086
  - **PGA (Pin Grid Array)**
    - Matriz de pines, colocados en la superficie inferior
    - Actualmente ocupan toda la superficie inferior
    - Es el caso del Intel 286 (80286)
  - **LGA (Land Grid Array)**
    - Los pines ahora están en el zócalo de la placa base (socket)
    - El microprocesador tiene los contactos planos
    - Polémico: fácil doblar los pines de la placa base
  - Otros: QFP, PLCC, LCC, Slot,…







## Refrigeración del microprocesador

- El procesador, cuanto más trabajo realiza, más se calienta:
  - A mayor calor…
    - Fallos e inestabilidad del sistema.
    - Se puede quemar.
  - Puede llegar a soportar unos 60°.
- Es necesario disipar este calor de la forma más eficaz posible
- Sistemas de refrigeración:
  - Refrigeración **por aire** o **aircooling**
  - Refrigeración **líquida** o **watercooling**







## Refrigeración por aire o aircooling

- Componentes:
  - Disipador  (refrigeración pasiva)
  - Ventilador (refrigeración activa)
- El encapsulado del micro también ayuda a disipar el calor.
- Pasta termoconductora:
  - Mejora el flujo del calor se emplea (térmica) entre procesador y disipador







## Refrigeración por aire

- ¿Cómo debe fluir el aire dentro de la caja?
  - Ventiladores frontales y laterales:
    - **<u>introduciendo aire</u>**
  - Ventiladores traseros y superiores:
    - **<u>extrayendo aire</u>**






## Refrigeración por aire

- CFM (pies cúbicos por minuto; cubic feet per minute)
  - Unidad para medir el flujo de gas o líquido
  - Volumen en pies cúbicos que pasa a través de un punto fijo en un minuto
- dBA (decibelios A)
  - Indicador del riesgo auditivo de una señal sonora.
  - Indican la cantidad de ruido que genera el sistema de refrigeración.
  - Indican la cantidad de ruido que genera el sistema de refrigeración.
  - 26 dBA, se oyen; a partir de 35 dBA molestan.
  - NOTA: 25 dBA = 1 sone
- PWM
  - Modulación por ancho de pulsos.
  - Tecnología que permite controlar la velocidad del ventilador.
  - Se ajusta la velocidad de acuerdo al calor generado por la CPU.





## Refrigeración por aire (Ejemplo)

| Fabricante                   | Arctic                        |
| :--------------------------- | ----------------------------- |
| **Modelo**                   | Alpine 64 GT AMD              |
| **Compatibilidad (sockets)** | AMD: 754, 939, 940, AM2, AM2+ |
| **Potencia**                 | 70W                           |
| **Flujo de aire**            | 25.6 CFM                      |
| **Velocidad**                | 500-2000 RPM                  |
| **Regulación**               | Función PWM                   |
| **Nivel de ruido**           | 7.5 dbA                       |
| **Precio**                   | ~10€                          |





## Refrigeración líquida o watercooling

- Se utiliza agua o líquido refrigerante 
  - Conducen mejor el calor que el aire
- Se trata de un circuito cerrado de líquido que extrae el calor
- Componentes básicos:
  - Depósito
  - Circuito de líquido (tubos)
  - Bomba  (para que circule el líquido)
  - Radiador  (tubos muy finos entre los que pasa el aire)
  - Ventilador (para enfriar el líquido en el radiador)
- Los hay internos o externos a la carcasa
- Algunos vienen sellados (sealed) de fábrica, no requieren mantenimiento.





Refrigeración líquida (Ejemplo)




Refrigeración por aire
Ejemplo
FabricanteCollerMaster
ModeloHyperTX3 EVO
Compatibilidad INTEL: LGA 1366 / 1156 / 1155 / 
13
Compatibilidad (sockets)
INTEL: LGA 1366 / 1156 / 1155 / 775 / 1150 AMD: FM1 / FM2 / AM3+ / AM3 / AM2+ / AM2 Flujo de aire15.7-43.1 CFM
Velocidad800-2200 RPM(PWM)
RegulaciónFunción PWM
Nivel de ruido17-30 dBA
Precio~20€



Heatpipe
•Consiste en un tubo hueco sellado que contiene líquido refrigerante –Suele ser de cobre •Al calentarse el fluido en la parte del microprocesador, se evapora y se desplaza al otro extremo, donde se desplaza al otro extremo, donde se vuelve a condensar •Lo encontramos mucho en los portátiles •No es tan eficiente como el sistema anterior.





## Partes lógicas de un microprocesador

- Registros
  - En inglés, registers
- Unidad aritmético lógica
  - En inglés, Arithmetic Logic Unit (ALU)
- Unidad de coma flotante
  - En inglés, Floating Point Unit (FPU)
- Unidad de control
  - En inglés, Control Unit (CU)




Registros

Pequeñas memorias internas al micro muy rápidas

Almacenan datos, direcciones, instrucciones, …

El tamaño de estos registros determina en parte la arquitectura del microprocesador:

Intel 4004: 4 bits

Intel 8088: 8 bits

Intel 8086-286: 16 bits

Intel 386 ó Pentium, entre otros: 32 bits

Intel Corei3-i7: 64 bits

NOTA:

Bit = unidad mínima de información en informática

Su nombre proviene de “BinarydigIT” (dígito binario)

Puede valer 0 ó 1





Unidad aritmético lógica

Se encarga de ejecutar operaciones aritméticas y lógicassobre números enteros.

Los ordenadores actuales son “superescalares”.

Tienen unidades de ejecución repetidas

Esto implica que los microprocesadores actuales tienen más de una UAL.





Unidad de coma flotante

Realiza operaciones con números en coma flotante (números decimales).

LA FPU se incluyó en el micro a partir del Intel 486.

Los primeros microprocesadores:

Microprocesador Intel 386

Los primeros microprocesadores:

Del 8086 al 386 no incluían esta unidad

Había dos alternativas:

“Emular” los cálculos por software, lo que era muy lento

Incluir un coprocesador matemático

Chip (muy caro) denominado comúnmente el “copro”

Las placas tenían un zócalo para su colocación

Para el i286 era el i287, para el i386 el i387, …





Unidad de control

Como su nombre indica, es la unidad que lleva el control.

Dirige al resto de unidades del microprocesador. microprocesador.

Recupera las instrucciones de la memoria, las descodifica  y las ejecuta.

Ciclo de ejecución de cada instrucción

En función de la instrucción, da las órdenes oportunas al resto de componentes





Arquitectura x86

Todo empezó con el Intel 8086

Y continuó con el 80186, el 80286, el 80386, el 80486, Pentium, etc.

Se dice que todos pertenecen a la familia “x86” porque sus arquitecturas son compatibles

¿Qué significa?

Que un programa escrito para el 8086 funcionará en sus predecesores.

¿Cómo es posible?

Manteniendo el juego de instrucciones, entre otras cosas.

NOTA:

Lo único que entiende el microprocesador es el código máquina(lenguaje de más bajo nivel, 0s y 1s).

Los programas para ejecutarlos tienen que estar en código máquina.

Cada microprocesador tiene su juego de instrucciones, y ese conjunto de instrucciones forman los elementos del lenguaje máquina

La arquitectura se ha mejorado, manteniendo la compatibilidad básica





Nuevas instrucciones x86 (I)

MMX

En 1996, Intel añadió nuevas instrucciones con el Pentium MMX.

Este nuevo conjunto de instrucciones se llamó MMX.

Eran para agilizar operaciones multimediapara vídeo o sonido.

También se incluyeron 8 nuevos registros de 64 bits.

Aquí empezó la carrera. 





Nuevas instrucciones x86 (II)

3DNow!

AMD no quiso quedarse atrás.

Añadió también nuevas instrucciones a su microprocesador AMD K6-2.

Este conjunto de instrucciones se llamó 3DNow!.

Su objetivo era mejorar el rendimiento en los cálculos para gráficos 3D.

Más tarde se ampliaron las instrucciones: Enhanced 3DNow!(Athlon) y 3DNow! Professional (Athlon XP)



Nuevas instrucciones x86 (II)

Intel siguió y siguió añadiendo nuevas instrucciones a los microprocesadores de la familia x86:

SSE(Streaming SIMD Extensions) en el Pentium III (AMD las incorporó más tarde a su Athlon XP)

SSE2en el Pentium 4 (AMD las soporta en su Athlon 64)

SSE2en el Pentium 4 (AMD las soporta en su Athlon 64)

SSE3en la última revisión del Pentium 4 (Prescott)

SSSE3y SSE4en el Core 2.

AMD, por su parte, no se ha interesado por SSSE3 y SSE4:

Incorpora SSE128 ó SSE4a.





Aclaraciones

a)Intely AMDson actualmente los principales fabricantes de microprocesadorespara PC

Hubo otros fabricantes, como Cyrix.

b)Los microprocesadores que fabrica b)Los microprocesadores que fabrica AMD también pertenecen a la familia x86.

c)Para sacar provecho a las nuevas instruccionesañadidas al juego de instrucciones del microprocesador, los programadores (o más bien los compiladores)  las tienen que tener en cuenta.





El mundo de los 64 bits (I)

Desde el 386 (año 1986) el tamaño de la mayoría de los registros seguían siendo de 32 bits

Por lo tanto, direccionamiento de memoria con 32

Por lo tanto, direccionamiento de memoria con 32 bits.

Así, sólo es posible acceder hasta 4GB de memoria.

Era el momento de actualizar a los 64 bits.





El mundo de los 64 bits (II)

Intel tomó la iniciativa:

Decidió abandonar la arquitectura IA-32 (x86 de 32 bits).

Pasó directamente a los 64 bits con la nueva arquitectura IA-64.

Esto se plasmó en los microprocesadores Itanium (2001) e Itanium2 (2002), muy avanzados.

Necesita software específico para estos microprocesadores, y eso lleva tiempo.

Incluyeron un modo de compatibilidad con IA32,

Para utilizar el software de 32 bits existente.

Pero la “emulación” era muy lenta.

Fue un fracaso comercial.





El mundo de los 64 bits (III)

AMD tomó la dirección contraria:

Complementarla arquitectura IA-32.

Surge así la llamada arquitectura x86-64

AMD la denominó AMD64

También se denomina x64.

Surgen así los microprocesadores Opteron (2003), Athlon 64 (2003) y Phenom (2007).

Sigue funcionando el software creado para micros x86 a alta velocidad.

Y además soporta nuevo software de 64 bits.

En las direcciones de memoria no se llegó aún a los 64 bits pero sí a los 44 bits

¡Hasta 16 TB de RAM!

¡Éxito rotundo!

Intel adoptó esta nueva arquitectura y la retocó para denominarla Intel64 (antes IA-32e y EM64T = Extended Memory Technology).





Parámetros de funcionamiento de un microprocesador
•Velocidad de reloj (MHz o GHz) •Velocidad de bus (ancho de bits y MHz) •Memoria caché •Tecnología de fabricación (nm) •Tecnología de fabricación (nm) •El voltaje del microprocesador •Tipos de núcleo •Múltiples núcleos (dual core, quad core, …) •Marca (¿Intel o AMD?) •Mejoras de rendimiento



Velocidad de reloj (MHz o GHz)
•El ordenador funciona de forma síncrona marcada por una señal de reloj. •Los pulsos por segundo que genera el reloj se llama frecuenciay se mide en “hercios” (Hz). •Es lo que se conoce como “velocidad de reloj” o “frecuencia del microprocesador”. •Megahercio = MHz = 1.000.000 Hz •Megahercio = MHz = 1.000.000 Hz •Gigahercio = GHz = 1.000.000.000 Hz •Ejemplo: 1 procesador a 2000MHz (2GHz) podrá realizar 2.000.000.000 de ciclos por segundo •¡No se debe emplear como medida para comparar micros distintos! •La CPU puede ejecutar una instrucción en 1 o más ciclos de reloj –Dependerá de la instrucción de que se trate



Velocidad de bus (bytes / segundo)
•Los microprocesadores tienen un bus de datos para comunicarse con el resto del sistema –Normalmente está conectado al northbridge (puente norte). –A su vez el Northbridge lo comunica con la RAM y los otros componentes. •Éste bus de datos se denomina el bus frontal (FSB, Front Side Bus) o bus del sistema –AMD lo denomina HyperTransport. –El de Intel ahora es QPI (Quick Path Interconnection).
Bus frontal
DMI – El de Intel ahora es QPI (Quick Path Interconnection). •Ancho de bits del bus –Número de bits que puede transmitir en cada pulso. –Suele ser de 64 bits •Frecuencia del bus –Suele ser muy inferior a la velocidad interna del micro. –Ejemplo: Pentium III a 733MHz tenía bus a 133MHz. •Tasa de transferencia (Velocidad de bus) –TT = Ancho de bits del bus * Velocidad reloj del bus –Cuanto mayor sea el caudal de datos del bus mejor irá la comunicación –Ejemplo: Ancho de 64 bits y velocidad 133MHz = 1014MB/s 



Cálculo de la velocidad del micro
•Esta velocidad se mide en Hz (frecuencia) •Esta frecuencia se obtiene de multiplicar dos factores: –La frecuencia del bus frontal (FSB) •FSB = es la “autopista” que conecta la CPU con el resto de componentes (a través del northbridge) través del northbridge) –El multiplicador •Indica el número de veces que es más rápido la CPU que el FSB •Internamente la CPU va a una velocidad y el FSB va a otra •El Pentium III tenía un multiplicador de 5,5; esto es, iba 5,5 veces más rápido que el FSB Frecuencia CPU = Frecuencia FSB * multiplicador –Ejemplo: FSB a 400MHz y un procesador con un multiplicador de 5x  2000MHz = 2GHz



¿Cuánto de bueno es un micro?
•Unidades para medir la eficacia de un procesador: –MIPS •Millones de instrucciones por segundo –MegaFLOPS •Millones de instrucciones en coma flotante por segundo •Lo mejor es hacer comparativas (benckmarking) •Lo mejor es hacer comparativas (benckmarking) –Ejecutar un software de testeo sobre los micros a comprobar –Suelen medir el tiempo que tardan en realizar una serie de cálculos intensivos (calcular fractales) –Ejemplos: Sandra, Everest, … –Enlace: http://www.cpubenchmark.net/



Conocer los detalles de mi CPU



La memoria caché (MB)
•Memoria muy rápida y de pequeño tamaño. •Usada por la CPU para reducir el tiempo necesario para acceder a memoria principal(la RAM). •Guarda una copia de los datos e instrucciones de la memoria RAM utilizados más frecuentemente •Se usan memorias de semiconductores de tipo SRAM (Static RAM). •Actualmente hay hasta 3 niveles: L1, L2 y L3 •Actualmente hay hasta 3 niveles: L1, L2 y L3 –La L1 es la más próxima a la CPU y L3 la más alejada –Cuanto más cerca de la CPU más pequeña y rápida es la memoria –L1 dentro del núcleo; L2 y L3 conectadas al núcleo mediante el BSB(Back Side Bus) –L1se divide en dos: una sólo para datosy otra sólo para instrucciones. •Ejemplo: Intel Core 2 Quad Q6600 –L1: 64Kb + 64Kb (64Kb para instrucciones + 64Kb para datos) –L2: 2 x 4 Mb (4 Mb por pareja de núcleos) –Total de caché: 8’128 Mb de caché



La memoria caché (MB)
Ejemplo •CPU con 3 niveles de caché: L1, L2 y L3. •L3 es compartida por los núcleos. •L1 y L2 son dedicadas para cada núcleo.



Conocer detalles de mi caché de CPU



Tecnología de fabricación (nm)
•También se denomina “litografía”. •Lo avanzado de una tecnología se indica mediante el tamaño del elemento más pequeño del chip (normalmente el transistor). •Se trata de elementos microscópicos (millones en menos de un centímetro cuadrado) •Por eso se miden en nanometros (nm) •Intel actualmente fabrica a 32nm •Recientemente anunció los 25nm •Al reducir el tamaño: –Más chips por oblea (se reducen costes) –Mayores velocidades de reloj (GHz) –Disminuye el voltaje necesario para funcionar y así el calor generado –Queda espacio para más elementos (p.ej. cachés de mayor capacidad) •Se está llegando al límite del silicio



Potencia de diseño térmico (W)
•En inglés, Thermal Design Power (TDP). •Máxima cantidad de potencia requerida por el sistema de refrigeración de un ordenador para disipar el calor generado ordenador para disipar el calor generado por el microprocesador. •Se mide en vatios (W).



El voltaje del microprocesador
•Cuanto menor sea menos calor se genera. •Aumentar el voltaje es peligroso (freír el chip). •Puede ser necesario al realizar “overclocking”. •Actualmente suele haber dos voltajes en el •Actualmente suele haber dos voltajes en el microprocesador: –Externo al chip –Voltaje de E/S •Suele ser 3,3 v (voltios) –Interno al chip (núcleo) –Vcore o core voltage •Este es el interesante para el overclocking •Suele ser 1.2 v o menos (menos temperatura)



Tipos de núcleo
•Durante el tiempo que se emplea una determinada marca comercial el microprocesador evoluciona –Se fabrican diversas versiones del núcleo –Se identifican mediante un nombre clave •Ejemplo: –Nombres clave de las distintas versiones de núcleo de Pentium 4:Pentium 4 Willamette de Pentium 4: •Willamette •Northwood •Prescott •Prescott 2M (2MB de caché L2) •Cedar Mill (ya con tecnología de 65nm) •Pueden cambiar tanto a nivel físico(encapsulado, voltaje, caché,…) como interno(nuevas instrucciones, monitorización térmica,…).



Microprocesadores con núcleo múltiple
•Aumentar la velocidad de reloj tiene un límite •Nuevas formas de mejorar el rendimiento •Emplear varios microprocesadores en lugar de uno –Soporte multiprocesador es molesto y caro •Placa base con dos o más zócalos, circuitería compleja compleja •Duplicar requisitos de refrigeración •Solución: –Varios núcleos en un único encapsulado –De ahí, dual core, quad core, … •Actualmente: –Todos de doble núcleo, como mínimo. –Excepto Atom, para netbooks, de 1 solo núcleo (aunque hay modelos de doble núcleo)



¿Intel o AMD?
•Al principio: –AMD fabricaba bajo licencia de Intel, igual que otras empresas. –Por lo tanto, sus micros eran idénticos a los de Intel. •Intel, al sacar su 386, decidió retirar la licencia de fabricación –AMD e Intel estuvieron peleando durante años en los tribunales •Durante este tiempo, AMD se las ingenió para sacar microprocesadores •Durante este tiempo, AMD se las ingenió para sacar microprocesadores compatibles con los de Intel –Mediante ingeniería inversa –A AMD le fue muy bien, a otras empresas no tanto •Los diseños se han ido separando con el tiempo, hasta ser absolutamente diferentes •Para algunas tareas unos procesadores son mejores que los del otro –Pentium 4 era bueno procesando vídeo –Athlon 64 no era tan bueno en eso, pero si para los juegos •Sin duda, la compatibilidad a nivel de software está garantizada. 



Overclocking

Forzar al procesador a que trabaje a un frecuencia superior (+MHz) para las que ha sido diseñado

¿Cómo?

–Aumentar el multiplicador o la frecuencia del FSB desde el “BIOS Setup”

–No todos los micros de Intel permiten hacerlo •Gama “K” o “Extreme” permiten cambiar multiplicador.

Gama “K” o “Extreme” permiten cambiar multiplicador.

Otros modelos vienen bloqueados.

Ventajas

–Podemos mejorar el rendimiento del equipo sin gastar dinero.

Desventajas

–Acortan la vida útil del microprocesador.

–Pérdida de garantía.

–Puede ser necesario mejorar la refrigeración del micro.

–Alto riesgo de quemar el micro.





Hyperthreading

Tecnología de los micros de Intel

En qué consiste:

–A veces la CPU no necesita un ciclo completo para ejecutar una instrucción

–Puede ejecutar las instrucciones de otro hilo (thread)

–Puede ejecutar las instrucciones de otro hilo (thread) en el tiempo sobrante

Intel asegura una mejora de 15-30% en el rendimiento de los micros

Sólo en sistemas operativos multihilo

Disponible desde el Pentium 4 (2000-2008)





VT-x y AMD-V

Son extensiones incluidas por los microprocesadores para favorecer la virtualización.

Estas extensiones se denominan:

–VT-x, en los microprocesadores de Intel

–VT-x, en los microprocesadores de Intel

Primera vez en modelos 662 y 672 de Pentium 4 (2005)

–AMD-V, en los microprocesadores de AMD

Primera vez en Athlon 64 (Orleans), Athlon 64 x2 y Anthlon 64 FX (Windsor) (2006) .

Permiten que una máquina huésped (host) pueda ejecutar una máquina virtual (guest) sin recurrir a la emulación.





Intel Smart Cache

Tecnología de los micros de Intel

Consiste en la arquitectura que permite a los núcleos compartir dinámicamente el último nivel de caché (L2 ó L3) último nivel de caché (L2 ó L3)

Por ejemplo: si un núcleo la necesita, puede usar toda la caché L2 ó L3 
46





Intel Turbo Boost

Tecnología de los micros de Intel

Consiste en un overclocking automático

El microprocesador aumenta su rendimiento cuando es necesario. es necesario.

Se activan en función del número de núcleos activos y temperatura del microprocesador, entre otros factores.

–Por ejemplo: si hay núcleos inactivos (infrautilizados), se “overclockean” los núcleos activos.





Physical Address Extension (PAE)

Característica de los micros de 32 bits (x86).

Por su limitación, físicamente sólo pueden acceder a 4GB de memoria física.

PAE les permite utilizar hasta 64GB.

El micro puede manejar direcciones de memoria de hasta 36

El micro puede manejar direcciones de memoria de hasta 36 bits.

–Hasta 64GB de memoria física.

Disponible desde el Intel Pentium Pro y AMD Athlon (año 1995).

Se solía activar desde el S.O. para resolver problemas del mapeo de dispositivos E/S (MMIO)





Microarquitecturas de Intel

El conjunto de instrucciones de la arquitectura (denominado ISA) es el mismo para todos.

Una microarquitectura es como un micro implementa el ISA.

Intel les da unos nombres en clave (codename).

Por ejemplo:

Por ejemplo:

–Broadwell (2014): 14 nm

–Haswell (2013): 22 nm, socket LGA 1150

–Ivy Bridge (2012): 22 nm, socket LGA2011, LGA1155

–Sandy Bridge (2011): 32 nm, socket LGA2011, LGA1155

–Westmere (2010): 32 nm, socket LGA 1156

–Nehalem (2008): 45nm


