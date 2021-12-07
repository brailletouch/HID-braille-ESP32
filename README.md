# HID-braille-ESP32
to develop HID braille library for ESP32 for brailletouch / para desarrollar librería HID braille para ESP32 para brailletouch

This repository is for developing a hid braille library for ESP32 /  Este repositorio es para desarolar una biblioteca braille hid para ESP32

English

The initial example can be Espressif:
https://github.com/espressif/esp-idf/tree/master/examples/bluetooth/bluedroid/ble/ble_hid_device_demo
In it we have everything you need to get started on a mouse / keyboard project.

Please try to compile and update the sample to ensure a successful development setup.

(introduction to ESP32: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html)

And then you need to change the HID descriptor to the HID braille documentation example.


here are the braille HID references

https://usb.org/sites/default/files/hutrr78_-_creation_of_a_braille_display_usage_page_0.pdf

https://github.com/nvaccess/nvda/blob/00cd67b737bc5b23a6f5e31cf28110b64ebf2fee/devDocs/hidBrailleTechnicalNotes.md


Español

El ejemplo inicial puede ser Espressif:
https://github.com/espressif/esp-idf/tree/master/examples/bluetooth/bluedroid/ble/ble_hid_device_demo
En él tenemos todo lo que necesita para comenzar en base a un proyecto de mouse / teclado.

Intente compilar y actualizar la muestra para garantizar una configuración de desarrollo exitosa.

(introducción a ESP32: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html)

Y luego debe cambiar el descriptor HID al ejemplo de documentación braille HID.


aquí están las referencias HID en braille

https://usb.org/sites/default/files/hutrr78_-_creation_of_a_braille_display_usage_page_0.pdf

https://github.com/nvaccess/nvda/blob/00cd67b737bc5b23a6f5e31cf28110b64ebf2fee/devDocs/hidBrailleTechnicalNotes.md

Marco braille NVDA https://github.com/nvaccess/nvda/wiki/Braille-framework

adición de soporte para una pantalla Braille  en NVDA (pronto ya no tendra soporte usar solo como referencia) https://github.com/nvaccess/nvda/wiki/AddingSupportForABrailleDisplay

HID Usage Tables - Universal Serial Bus (USB) https://usb.org/sites/default/files/hut1_2.pdf

INFORME TÉCNICO brilletouch

Distribución de los controles en los equipos brailletouch 40 

brailletouch 40 contiene la misma distribucion de teclas que  Focus 40 Blue - Freedom Scientific, solo con un teclado adicional corespondiente al equibalente de flechas del teclado de navegacion (isquierda, derecha, arriba, abajo, enter, tabulador, mayuscula + tabulador)



Lado izquierdo del equipo

⦁	(1) Botón de Encendido/Apagado – primer control ubicado al deslizarse desde la parte frontal hacia la parte trasera.
⦁	(2) Puerto micro USB – localizado detrás del botón de encendido/apagado.


Parte superior del equipo

⦁	(3) Celda braille – ubicada hacia la parte frontal derecha del dispositivo.
⦁	(3A) Celdas braille virtuales – ubicadas hacia la parte frontal central del dispositivo.
⦁	(4) Boton de desplazamiento del cursor – localizados arriba de la celda braille.
⦁	(5) Botones dobles de navegación – localizados a ambos lados de la celda braille.
⦁	(6) Botones para cambiar el modo de navegación – localizados arriba de los botones dobles de navegación.
⦁	(7) Teclado braille – localizado arriba de las celdar brailles virtuales. El orden de los puntos del teclado braille es el siguiente: Puntos 1, 2, 3, 7 a la izquierda y los puntos 4, 5, 6, 8 a la derecha.
⦁	(8) Barra de espacio – localizada en el centro, debajo del Teclado braille.
⦁	(9A) Mayúscula izquierda (left shift) al lado izquirdo de la barra espaciadora.
⦁	(9B) Mayúscula derecha (right shift). al lado derecho de la barra espaciadora.
⦁	(10) teclado de navegacion ubicadas hacia la parte izquierda del dispositivo ((10A) isquierda, (10B) derecha, (10C) arriba, (10D) abajo, (10E) enter, (10F) tabulador, (10G) mayuscula + tabulador)

Parte frontal del equipo

En la parte frontal del equipo se encuentran ubicados los siguientes controles, de izquierda a derecha:
⦁	(11A) Botón izquierdo de desplazamiento (pan left).
⦁	(12A) Barra izquierda.
⦁	(13A) Botón izquierdo de selección.
⦁	(13B) Botón derecho de selección.
⦁	(12B) Barra derecha.
⦁	(11B) Botón derecho de desplazamiento (pan right).

Observaciones

Construcción: Brailletouch 40, debe ser un equipo livianos, pero de fuerte construcción y sólida.

Celdas braille: La proyección (altura) de los puntos braille debe ser apropiada y fácil de diferenciar con los dedos. Esto resultara en una rápida identificación de las combinaciones de puntos, facilitando la lectura durante periodos prolongados. El grosor y la consistencia de la celda braille brailletouch debe de calidad.

Teclado braille: La distribución del teclado braille (estilo Perkins) y los controles adicionales en la brailletouch 40, deben ser comodos para su uso y de tamaño adecuado. El diseño del teclado braille en dbe ser ergonómico e intuitivo, facilitando la escritura durante periodos prolongados. La distribución del teclado y su uso debe ser de los más cómodos.

Controles: La función de los controles de la patalla braille brailletouch, está condicionada al lector de pantalla o aplicación que se utilice para manejar el dispositivo. Los botones de desplazamiento, navegación, barras y selectores, entre otros controles, permiten navegar a través de las distintas plataformas y ejecutar variadas funciones. Mediante estos controles es posible moverse entre las aplicaciones de un iPhone, abrir el menú de opciones de Microsoft Word en Windows, abrir el menú de contexto en un teléfono Android, entre otras funciones. 

Duración de la batería: Una de las características que más impresionan de que debe tener bailletouch es la duración de su batería, tanto en tiempo de uso continuo como también en el tiempo de espera (standby).











