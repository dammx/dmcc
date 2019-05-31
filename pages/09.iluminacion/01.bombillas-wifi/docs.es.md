---
title: 'Bombillas Wifi'
media_order: 'up1_azul1.png,hue.png,utorch.png,bombilla_teckin.png'
published: true
metadata:
    Key(bombillas_wifi): 'Valor((bombillas,wifi,hub,phillips,utorch,teckin,home,assistant)'
taxonomy:
    category:
        - docs
    tag:
        - domotica
        - bombillas
        - wifi
        - hub
        - phillips
        - utorch
        - teckin
        - home
        - assistant
        - google
sitemap:
    changefreq: hourly
    priority: 0.5
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> Uno de los elementos conectados a Internet más fáciles de incluir en nuestros hogares inteligentes son las bombillas Wifi. Hay una gran variedad de marcas y modelos, es una opcion de las más interesantes por su precio y sencillez de funcionamiento.

!! El funcionamiento de las bombillas inteligentes depende del modelo que se compre: existen modelos que necesitan un _“ hub”_ o centralita y otros que no lo requieren, con los que sólo hay que conectar las bombillas por wifi.

**¿En qué debemos fijarnos a la hora de comprar una lámpara inteligente?**
+ Si la luz que emitirá será sólo blanca o también permite elegir colores.
+ La temperatura de color.
+ Desde el punto de vista técnico, la temperatura de color se mide en grados Kelvin (K). Cuanto menos grados tenga, más cálida (amarilla) será la luz y, por lo contrario, cuantos menos grados, más fría.
Las bombillas inteligentes pueden ofrecer distintas temperaturas de color. Hay que tener en cuenta que la luz cálida es la ideal para el salón y las habitaciones -ya que es más agradable para atardecer y la noche- mientras que la luz fría produce una sensación de mayor luminosidad, por lo que se emplea con más frecuencia en cocinas y baños.
+ La vida útil de las lámparas, es decir, su tiempo de vida esperado.
+ La conectividad: si es mediante wifi o por Bluetooth.
+ Si admiten o no control por voz.
+ Debemos evaluar se tienen la posibilidad de conectarse con otros electrodomésticos de la casa.
+ El precio. Hay diferencias considerables entre unas marcas y otras.

!!! _**Te presentamos varias opciones que pueden ser de tu interés...**_

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Bombilla LED RGB 9.5W Philips Hue  | Amazon » 47,99€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Bombilla LED RGB 9.5W Philips Hue ...**](https://amzn.to/2I6OCyu)</p><p>Bombilla RGB de Philps Hue con casquillo E27. Poseen una potencia de 9.5W y nos permite su uso por medio de Alexa, Google Assistant o HomeKit. 16 millones de colores.</p><p>Para usar en el sistema de Philips es necesario el bridge.</p><p> Para la integración de _**Home Assistant**_ tienes que integrarlo directamente desde integraciones.</p> | <div> ![img-500crop][amzn-hue] </div> <div> <a href="https://amzn.to/2I6OCyu" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="Utorch Bombilla LED 7W RGB | Aliexpress » 11,78€"]

|  |  |
|:------|:-----------------------:|
| <p>[**Utorch Bombilla LED 7W RGB...**](http://s.click.aliexpress.com/e/bkqswhgU)</p><p>Bombilla Utorch RGB WiFi que nos permiten la iluminación de una habitación.</p><p> Es RGBW y funciona con Google Assistant, Alexa e IFTTT.</p><p>Se integra en _**SmartLife**_, por lo que deberíamos poder integrarlo en _**Home Assistant**_.</p> | <div> ![img-350crop][ali-utorch] </div> <div> <a href="http://s.click.aliexpress.com/e/bkqswhgU" alt="AlieExpress-link" target="_blank"> <button type="button" style="color:#fff;background-color:#e8a100;width:80%;height:35px;"><i class="fa fa-shopping-cart  fa-lg"> AliExpress</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="Teckin Bombilla LED inteligente WiFi  | Amazon » 15,99€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Teckin Bombilla LED inteligente WiFi...**](https://amzn.to/2I844dL)</p><p>Bombilla RGBW de 7.5W WiFi de la marca Teckin que se integra en _**Smart Life**_.</p><p>Compatible con Alexa y con Google Home además de que deberíamos poder integrarlas en **_Home Assistant_**.</p> | <div> ![img-500crop][amzn-b.teckin] </div> <div> <a href="https://amzn.to/2I844dL" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-hue]: user://pages/09.iluminacion/01.bombillas-wifi/hue.png?lightbox=1024&cropResize=500,500
[ali-utorch]: user://pages/09.iluminacion/01.bombillas-wifi/utorch.png?lightbox=1024&cropResize=500,500
[amzn-b.teckin]: user://pages/09.iluminacion/01.bombillas-wifi/bombilla_teckin.png?lightbox=1024&cropResize=500,500
[int-ghome]: user://pages/02.interruptores/integracion_google_home.gif
---

[![](up1_azul1.png)](# "Volver al Inicio")

[/ui-tab]

[ui-tab title="Integración ..."]

La **Integración en Google Home** es muy secilla, solo tienes que añadir la cuenta que creas de la aplicacion del disposivo, en este caso sera **_Smart Life_**  o  **_Tuya_**,  en la configuración de añadir dispositivos de _Google Home_, aquí tenéis el enlace para descargarlo:
 * [**Smart Life android**](http://bit.ly/2JnEUtN)
 * [**Smart Life Iphone**](https://apple.co/2DVyRsK)
 * [**Tuya Android**](http://bit.ly/2ZYql5T)
 * [**Tuya iphone**](https://apple.co/2vIrNeD)

###### **_(Aúnque en el Ejemplo usamos la aplicación Kasa, el procedimiento para la integración és el mismo, utilizando la aplicación correcta del componente, arriba indicada, según proceda)._**.###### 
![int-ghome]

**Para Integrarlo en Home Assitant**
Solo necesitaras anadir a tu `configuration.yaml` los siguientes datos:

+ Ejemplo  App Tuya `configuration.yaml`:

```text

tuya:
  username: nuestro@correo.es
  password: contraseñaquepusimos
  country_code: 34 

```
+ Ejemplo  App Smart Life `configuration.yaml`:

```text
​
tuya:
  username: nuestro@correo.es
  password: contraseñaquepusimos
  country_code: 34
  platform: smart_life
​
```
---
[![](up1_azul1.png)](# "Volver al Inicio")

[/ui-tab]

[/ui-tabs]