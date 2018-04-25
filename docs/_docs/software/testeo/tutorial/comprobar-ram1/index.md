---
title: Comprobar el estado de la memoria RAM
---

1. Descarga del software desde la [página del fabricante](https://www.memtest86.com/download.htm):

   ![](imagenes\Screenshot_1.png)

   Y seguir las instrucciones del fabricante que están dentro del archivo descargado anteriormente (PDF):

   En nuestro caso, al no disponer de CD, lo haremos a través de un USB Booteable.

   ![](imagenes\Screenshot_2.png)

2. Abrir la aplicación **imageUSB** para bootear el USB con la ISO de MemTest86:

![](imagenes\Screenshot_7.png)

3. Como dicen las instrucciones, habrá que marcar todas las opciones que aparecen indicadas con una flecha, y finalmente, hacer clic en Write:

![](imagenes\Screenshot_3.png)

​	



![](imagenes\Screenshot_5.png)

![](imagenes\Screenshot_6.png)

4. Una vez completado el proceso anterior, habrá que iniciar la máquina y configurar la BIOS para bootear desde el USB:

![](imagenes\foto1.jpg)

5. Una vez configurado, ejecutamos el programa que aparecerá en la lista de particiones del GRUB (en nuestro caso):

![](imagenes\foto3.jpg)



6. Simplemente, sería iniciar la aplicación y como no soporta UEFI la máquina, se iniciará la versión 4.20 (7.5 en máquinas con UEFI), y empezará el diagnóstico automáticamente:

   Se realizarán varios test.

![](imagenes\foto4.jpg)

Podemos observar que nos aparece:

- Procesador (Intel Core 2).


- Niveles de caché (L1, L2).


- Memoria RAM (4 GB).


- Chipset (Intel Q35).


- Configuraciones de la RAM (DDR2-332MHz, latencia CAS y el modo en el que están puestas (Dual Channel)).

## Autores

* Eduardo Reyes Peraza
* Daniel de la Torre Bueno

