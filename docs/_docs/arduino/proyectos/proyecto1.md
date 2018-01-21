---
title: Proyecto 1 - Encender un led
---

El proyecto consiste en encender un led conectado al pin 12 de la Arduino UNO. 

Esquema físico del proyecto:

![Esquema del proyecto](imagenes/proyecto1-esquema.png)

Programa en ensamblador AVR:

```asm
;
; EncenderLed.asm
;

.cseg

	; configura el pin 4 del puerto B (pin 12 Arduino) como salida
	ldi		r16, 0b00010000
	out		DDRB, r16
	
	; activa el pin 4 del puerto B (se enciende el led)
	sbi		PORTB, 4

loop:
	jmp		loop
```
