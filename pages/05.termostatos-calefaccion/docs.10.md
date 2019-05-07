---
title: 'Termostatos Wifi'
media_order: netnamo.png
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> Comprar un termostato WiFi es una de las mejores cosas que puedes hacer para ahorrar en la factura de la luz, en el caso que tengas calefacción en casa. Lejos de ser una pijada para geeks y techies, los termostatos inteligentes han demostrado ser, como mínimo,  **un 24% más eficientes que los termostatos analógicos**. Y tal y como está el precio de la luz, no es cosa menor.

Pero instalar un termostato WiFi en casa no solo es buena idea por el ahorro energético, sino por confort. La regulación automática de la temperatura, el control a distancia desde tu propio móvil allí donde estés, y la posibilidad de monitorizar el consumo son prestaciones que los termostatos inteligentes ofrecen, mientras que los termostatos normales no.

Los termostatos WiFi son también una herramienta más para domotizar tu hogar y hacerlo inteligente.

Tenemos modelos cono los _Nest_, _Netnamo_, _Tado_ ... Son termostatos de alta gama que funcionan perfectamente, pero son bastante caros! Dispones de modelos mas asequibles que también realizan su función perfectamente como: _Fluoreon_, _Beok_ y _Walmeech_ y están disponibles en _Amazon_ y _Aliexpress_.

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Broadlink RM pro | Amazon: 39,89€   Aliexpress: 34,33€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Netatmo.Termostato Inteligente para caldera individual...**](https://amzn.to/2H27FcP)</p><p>Termostato Inteligente Netatmo te permite<br />ahorrar una media de 37% de energÍa para<br /> calentar tu casa. El ahorro se consigue gracias <br />a una programa de la calefacción adaptada <br />a tu ritmo de vida, al control<br /> fácil de la calefacción desde tu smartphone<br /> y a los consejos personalizados<br /> de tu Balance de Ahorro Energético.</p><p> | ![200x200][amzn-netnamo][![buy-mzn!][buy-mzn]](https://amzn.to/2H27FcP)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Broadlink RM Mini3 | Amazon: 19.99€  Aliexpress: 17,12€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Broadlink RM Mini3...**](https://amzn.to/2WtK7DW)</p><p>-Wi-Fi Universal Remote integra todos tus<br />dispositivos controlados IR-<br />En comparación con RMPRO,<br />no dispone la función de RF 433 Mhz.<br /> Con la aplicación IHC en tu<br />teléfono inteligente puedes controlar<br />todos los dispositivos,<br /> usa un cable USB para conectar con la<br />energía.<br /> Fácil configuración.</p> | ![200x200][amzn-BL-RMMINI3] [![buy-mzn!][buy-mzn]](https://amzn.to/2WtK7DW)</p>[![buy-aliex][buy-aliex]](http://bit.ly/2V1LpVr)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-netnamo]: user://pages/05.termostatos-calefaccion/netnamo.png?lightbox=1024&cropResize=200,200
[amzn-BL-RMMINI3]: user://pages/04.broadlink+rm+pro/rm_mini_3.png?lightbox=1024&cropResize=200,200
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