# servocorte

Servocorte es un dispositivo de corte de precisión. Su actuador principal es una cuchilla adherida a un servomotor. Posee un sensor optico para detectar el tamaño del objeto a cortar.

## Motor

Se utiliza un motor paso a paso nema 17HS2408 de 0.6A para realizar los cortes. El motor se controlará con el dispositivo [EasyDriver v4.4](https://articulo.mercadolibre.cl/MLC-438559609-easydriver-v44-a3967-controlador-de-motores-de-paso-a-paso-_JM) basado en el integrado [A3967 de Allegro] (https://www.allegromicro.com/en/Products/Motor-Driver-And-Interface-ICs/Bipolar-Stepper-Motor-Drivers/A3967.aspx). El driver soporta hasta 750mA, por lo que no deberiamos tener problemas

## Sensor Optico

El sensor Optico se compone de un [led laser](http://electr3s.com/buscar?controller=search&orderby=position&orderway=desc&search_query=laser&submit_search=) y de un [foto receptor o fotodiodo](https://articulo.mercadolibre.cl/MLC-449727845-foto-diodo-sensor-luminosidad-arduino-_JM).

El  fotodiodo posee una salida digital y analógica.

Ambos dispositivos fueron escogidos para su facil integración electrica y mecánica.


## Controlador

El controlador central será un [arduino Uno R3] (https://afel.cl/producto/arduino-uno-r3/).

## Alimentación 

Tanto el arduino como los sensores pueden operar a 5V. Por su parte, el controlador del motor puede requerir un voltaje mayor para su correcta operación (por determinarse). Quizas la mejor estrategia es poner una fuente de [12 o 24 V](https://articulo.mercadolibre.cl/MLC-452759543-fuente-de-poder-12v-2a-24w-_JM) para alimentar al motor, y poner un [regulador step down](https://articulo.mercadolibre.cl/MLC-434594643-regulador-de-voltaje-step-down-dc-dc-lm2596-_JM) a 5V para el resto de la electrónica.

## Montaje y cables

Se utilizará una caja estanca, con prensa estopa todas saliendo por el mismo lado para:

* motor
* laser
* sensor optico
* alimentación

Hay que pensar en el soporte de la caja. Como se va a integrar con el equipo.
Hay que pensar en el soporte de los cables. Como se van a sujetar al equipo? con amarras plasticas?.




[bornera](https://articulo.mercadolibre.cl/MLC-444932023-par-de-borneras-atornillables-screw-para-arduino-uno-_JM)