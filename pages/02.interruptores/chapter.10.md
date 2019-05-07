---
title: 'Interruptores Wifi'
metadata:
    Key(domotizar_mi_casa): 'Valor(blog,grav)'
    Key(domotizar): 'Valor(blog,grav)'
taxonomy:
    category: docs
child_type: docs
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> ¿Qué es un interruptor inteligente?
Los interruptores WiFi al igual que los tradicionales se instalan conectándolos a la red eléctrica del interruptor convencional, pero a diferencia de los tradicionales te permiten instalar una aplicación de control en tu smartphone y con la que manejar a distancia este interruptor. Puedes establecer un horario, apagarlo o encenderlo de forma remota.


Interruptores de luz inteligentes: cosas a considerar:
A diferencia de las luces inteligentes , los interruptores requieren un poco más de consideración. Puede parecer un caso de simplemente sacar tu interruptor existente e intercambiarlo por uno nuevo, pero hay cosas que debes considerar como el cableado, medidas, compatibilidad.
Lo primero que tienes que tener en cuentas es que si quieres que todo sea una red, tienes que comprarlos de la misma marca. Así podrás manejarlos desde una app de forma unitaria y no tendrás que andar cambiando de una a otra.
Los interruptores WiFi tienen un problema actualmente y es que a diferencia de otros productos de domótica son bastantes caros y aún no hay muchas opciones diferentes en el mercado. A pesar de eso los productos que e destacado son muy buenas compras para tu hogar.
---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Netatmo | Amazon » 164,95€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Iraza Enchufe Múltiple Inteligente...**](https://amzn.to/2J7yf7y)</p><p>Configuración simple y fácil de usar : Siga los pasos de instalación. Investigación y desarrollo independientes, fácil de operar. Y la conexión wifi es muy estable.Control de voz de Amazon Alexa, Google Assistant. Puede activar o desactivar las 3 tomas por separado o juntas y los 2 puertos USB a través de Echo o Google Home. NEST y Samsung Smart Things serán compatibles en breve.</p><p> | ![200x200][amzn-iraza][![buy-mzn!][buy-mzn]](https://amzn.to/2J7yf7y)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Konesky Smart Power Strips | Amazon » 29.99 "]
|  |  |
|:-------------|:-------------:|
| <p>[**Konesky Smart Power Strips Wifi Protector contra sobretensiones con 4 salidas 4 puertos USB...**](https://amzn.to/2Valrih)</p><p>La regleta de alimentación inalámbrica Timmer es compatible con los puertos USB y USB, ahorra espacio y dinero, no necesita comprar muchos enchufes ni banco de energía, la regleta multifuncional le permite cargar muchos dispositivos al mismo tiempo. El control de voz de la toma de corriente inteligente wifi, puede controlar sus aplicaciones a través de los dispositivos Alexa / Google Home / IFTTT, conveniente y fácil de usar.</p> | ![200x200][amzn-BL-RMMINI3] [![buy-mzn!][buy-mzn]](https://https://amzn.to/2Valrih)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-iraza]: user://pages/03.Enchufes+Inteligentes/04.Regletas+Wifi/iraza.png?lightbox=1024&cropResize=200,200
[amzn-Konesky]: user://pages/03.Enchufes+Inteligentes/04.Regletas+Wifi/Konesky.png?lightbox=1024&cropResize=200,200
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