---
title: 'Regletas Wifi'
media_order: iraza.png
published: true
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> Te presentamos algunas de las mejores regletas Wifi del mercado. Controla todos tus aparatos eléctricos desde tu dispositivo móvil de forma sencilla y eficiente.

Aunque de momento no son muchos los fabricantes que se han lanzado a la fabricación de regletas Wifi, desde Regleta Eléctrica estamos seguros de que esta nueva forma de controlar la corriente eléctrica de tu casa va a ganar en adeptos en los próximos años.

Completo control de la regleta vía Wifi Acepta múltiples conexiones Wifi simultáneas Posibilidad de ahorro en el consumo eléctrico Control individual de cada toma AC Comodidad para controlar dispositivos Opción de conexión con Google Home o Amazon Echo Recordar que la mayoría de estas regletas de conexión inalámbrica soportan sobrecargas, altas temperaturas y largas jornadas de trabajo como el resto de regletas de calidad.

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Iraza Enchufe Múltiple Inteligente | Amazon: 28,66€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Iraza Enchufe Múltiple Inteligente...**](https://amzn.to/2J7yf7y)</p><p>Configuración simple y fácil de usar : Siga los pasos<br /> de instalación. Investigación y desarrollo <br />independientes, fácil de operar.<br /> Y la conexión wifi es muy estable.<br />Control de voz de Amazon Alexa, <br />Google Assistant. <br />Puede activar o desactivar las 3 tomas <br />por separado o juntas y los 2 puertos USB <br />a través de Echo o Google Home. <br />NEST y Samsung Smart Things serán <br />compatibles en breve.</p><p> | ![200x200][amzn-iraza][![buy-mzn!][buy-mzn]](https://amzn.to/2J7yf7y)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Nest Learning - Termostato Inteligente | Amazon: 249,00€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Nest Learning - Termostato Inteligente de 3 A Generación, Negro...**](https://amzn.to/2JsD7DA)</p><p>El Nest Learning thermostat de tercera generación es delgado, elegante y refinado. La Grande y claro pantalla y lectura a distancia te permiten ver temperatura, hora y predicción meteorológica incluso cuando te vayas de la otra parte de la habitación. El termostato Nest apprende la temperatura que desees para luego programmarsi de Sé. Conoce el tiempo necesario para calentar tu casa y te lafa cálida encontrar a tu llegada. Cuando vayas por se apaga, para permitirte ahorrar energía. De más, con la aplicación Nest, podrás cambiar la temperatura o controlar la historial de energía dondequiera que vayas.</p> | ![200x200][amzn-BL-RMMINI3] [![buy-mzn!][buy-mzn]](https://amzn.to/2JsD7DA)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-iraza]: user://pages/03.Enchufes+Inteligentes/04.Regletas+Wifi/iraza.png?lightbox=1024&cropResize=200,200
[amzn-Nest]: user://pages/05.termostatos-calefaccion/nest.png?lightbox=1024&cropResize=200,200
[buy-mzn]: https://dabuttonfactory.com/button.png?t=Comprar+en+AMAZON!&f=Roboto-Bold&ts=18&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=037ba2
[buy-aliex]: https://dabuttonfactory.com/button.png?t=Comprar+en+ALIEXPRESS!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=ffae00

---

[/ui-tab]

[ui-tab title="Integración ..."]

La **Integración en Google Home** es muy secilla, solo tienes que añadir la cuenta que creas de la aplicacion del disposivo, en este caso sera IHC,  en la configuración de añadir dispositivos de _Google Home_, en éste caso concreto la aplicación de _Android_ que a mí me funcionó correctamente es la que se descarga de su página oficial, la que se baja de _Google Play_ no me funcionó correctamente, aquí tenéis el enlace para descargarlo:
 * [**IHC android**](http://bit.ly/2VMG34J)
 * [**IHC Iphone**](https://apple.co/2H80XBN)
![](integracion_google_home.gif)

**Para Integrarlo en Home Assitant**

Necesitaras la carpeta de `custom_components` con los archivos para los diferentes componentes, que puedes descargar de aquí: [smartir.zip](smartir.zip), la tienes que poner en el directorio de Home Assistant dentro la carpeta `custom_components`, si no la tienes debes crearla.
![](smartir3.png)


+ Ejemplo `configuration.yaml`:

```text

smartir:

switch:
  - platform: broadlink
    host: 192.168.1.25 _(Ip de tu Broadlink)_
    mac: 78:0f:77:eb:4c:08 _(Mac de tu broadlink)_

media_player:
  - platform: smartir
    name: TV Samsumg
    device_code: 1060
    controller_send_service: switch.broadlink_send_packet_192_168_1_25
    power_sensor: binary_sensor.tv_power

```
---

[/ui-tab]

[/ui-tabs]







