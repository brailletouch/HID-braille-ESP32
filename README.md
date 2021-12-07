# HID-braille-ESP32
to develop HID braille library for ESP32 for brailletouch / para desarrollar librería HID braille para ESP32 para brailletouch

This repository is for developing a hid braille library for ESP32 /  Este repositorio es para desarolar una biblioteca braille hid para ESP32

English

In order to make it work for a braille display, the InputReport, OutputReport and REPORT_MAP structures need to be considerably adapted. The linked PDF seems to contain the report map. So that's a good starting point for adapting the REPORT_MAP.

The report map describes the data structures of the input and output report. So you will need to understand the details of this complex HID construct in order to figure out how the InputReport and OutputReport look like.

The initial example can be Espressif:
https://github.com/espressif/esp-idf/tree/master/examples/bluetooth/bluedroid/ble/ble_hid_device_demo
In it we have everything you need to get started on a mouse / keyboard project.

Please try to compile and update the sample to ensure a successful development setup.

(introduction to ESP32: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html)

And then you need to change the HID descriptor to the HID braille documentation example.

Ensures that the Hid device is truly a Braille display by verifying that the HIDP_CAPS.UsagePage of the HID device's top-level collection is set to HID_USAGE_PAGE_BRAILLE (0x41).

This document refers to how NVDA reads the HID braille structure https://github.com/nvaccess/nvda/pull/12523




here are the braille HID references

https://usb.org/sites/default/files/hutrr78_-_creation_of_a_braille_display_usage_page_0.pdf

https://github.com/nvaccess/nvda/blob/00cd67b737bc5b23a6f5e31cf28110b64ebf2fee/devDocs/hidBrailleTechnicalNotes.md

NVDA braille framework https://github.com/nvaccess/nvda/wiki/Braille-framework

adding support for a Braille display in NVDA (soon no longer support use for reference only) https://github.com/nvaccess/nvda/wiki/AddingSupportForABrailleDisplay

HID Usage Tables - Universal Serial Bus (USB) https://usb.org/sites/default/files/hut1_2.pdf


TECHNICAL REPORT brilletouch

Distribution control on brailletouch device 40

brailletouch 40 contains the same key layout as Focus 40 Blue - Freedom Scientific, only with an additional keyboard corresponding to the equivalent of arrows on the navigation keyboard (left, right, up, down, enter, tab, uppercase + tab)



Left side of the device

⦁ (1) On / off button: first control located by sliding it from front to back.
⦁ (2) Micro USB port: located behind the on / off button.


top of device

⦁ (3) Braille cell: located towards the right front of the device.
⦁ (3A) Virtual braille cells: located towards the front center of the device.
⦁ (4) Cursor scroll button: located above the braille cell.
⦁ (5) Double navigation buttons: located on both sides of the braille cell.
⦁ (6) Buttons to change the navigation mode, located above the dual navigation buttons.
⦁ (7) Braille keyboard: located above the virtual braille cells. The order of the dots on the braille keyboard is as follows: dots 1, 2, 3, 7 on the left and dots 4, 5, 6, 8 on the right.
⦁ (8) Space bar: located in the center, below the Braille keyboard.
⦁ (9A) Scroll left to the left side of the space bar.
⦁ (9B) Scroll to the right. to the right side of the space bar.
⦁ (10) navigation keyboard located on the left of the device ((10A) left, (10B) right, (10C) up, (10D) down, (10E) enter, (10F) tab, (10G) uppercase + tab )

Front of device

The following controls are located on the front of the device, from left to right:
⦁ (11A) Scroll left (pan left) button.
⦁ (12A) Left bar.
⦁ (13A) Left selection button.
⦁ (13B) Right selection button.
⦁ (12B) Right bar.
⦁ (11B) Scroll right (pan right) button.

Observations

Construction: Brailletouch 40, it should be a lightweight device, but with a strong and solid construction.

Braille cells: The projection (height) of the braille dots should be appropriate and easy to differentiate with the fingers. This will result in quick identification of point combinations, making it easier to read over extended periods. The thickness and consistency of the braille cell must be of good quality.

Braille keyboard: The braille keyboard layout (Perkins style) and the additional controls on the brailleouch 40 should be comfortable to use and sized appropriately. The dbe braille keyboard design is ergonomic and intuitive, making it easy to type over long periods of time. The keyboard layout and its use should be the most comfortable.

Controls: The function of the controls on the braille touch screen depends on the screen reader or application used to operate the device. The scroll buttons, navigation, bars and selectors, among other controls, allow you to navigate through the different platforms and perform various functions. Through these controls it is possible to move between the applications of an iPhone, open the Microsoft Word options menu in Windows, open the context menu on an Android phone, among other functions.

Battery life: One of the most impressive features bailletouch must have is its battery life, both in continuous use time and in standby time.


Español

Para que funcione para una pantalla braille, las InputReport , OutputReport y REPORT_MAP deben adaptarse considerablemente. El PDF vinculado parece contener el mapa del informe. Así que ese es un buen punto de partida para adaptar REPORT_MAP .

El mapa de informes describe las estructuras de datos del informe de entrada y salida. Por lo tanto, deberá comprender los detalles de esta compleja construcción HID para descubrir cómo se InputReport y OutputReport .


El ejemplo inicial puede ser Espressif:
https://github.com/espressif/esp-idf/tree/master/examples/bluetooth/bluedroid/ble/ble_hid_device_demo
En él tenemos todo lo que necesita para comenzar en base a un proyecto de mouse / teclado.

Intente compilar y actualizar la muestra para garantizar una configuración de desarrollo exitosa.

(introducción a ESP32: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html)

Y luego debe cambiar el descriptor HID al ejemplo de documentación braille HID.

Asegura que el dispositivo Hid sea verdaderamente una pantalla Braille al verificar que el HIDP_CAPS.UsagePagede la colección de nivel superior del dispositivo HID esté configurado en HID_USAGE_PAGE_BRAILLE( 0x41).

este documeto hace refrecia a como lee NVDA la estructura HID braille https://github.com/nvaccess/nvda/pull/12523



the Braille HID specification.




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











