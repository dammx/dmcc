---
title: 'Bombillas Wifi'
media_order: 'bombilla_teckin.png,up1_azul1.png'
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

Te presentamos varias opciones que pueden ser de tu utilidad

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Iraza Enchufe Múltiple Inteligente | Amazon » 28,66€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Iraza Enchufe Múltiple Inteligente ...**](https://amzn.to/2J7yf7y)</p><p>Configuración simple y fácil de usar : Simplemente, siga los<br />pasos de instalación.</p><p>- Investigación y desarrollo independientes, fácil de operar. La conexión wifi es muy estable. Control de voz vía _Amazon Alexa_ y _Google Assistant.</p><p>Puede activar o desactivar las 3 tomas por separado o juntas y los 2 puertos USB a través de _Echo_, _Google Home_, NEST y _Samsung Smart Things_ serán compatibles en breve.</p> | <div> ![img-500crop][amzn-iraza] </div> <div> <a href="https://amzn.to/2J7yf7y" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="Konesky Smart Power Strips | Amazon » 29.99€"]

|  |  |
|:------|:-----------------------:|
| <p>[**Konesky Smart Power Strips Wifi ...**](https://amzn.to/2Valrih)</p> Protector contra sobretensiones con 4 salidas 4 puertos USB.</p><p>La regleta de alimentación inalámbrica Timmer es compatible con los puertos USB, ahorra espacio y dinero, no necesita comprar muchos enchufes ni banco de energía, la regleta multifuncional le permite cargar muchos dispositivos al mismo tiempo.</p><p>El control de voz de la toma de corriente inteligente WIFI, puede controlar sus aplicaciones a través de los dispositivos  _Alexa_, _Google Home_ e _IFTTT_. Conveniente y fácil de usar.</p> | <div> ![img-500crop][amzn-Konesky] </div> <div> <a href="https://amzn.to/2Valrih" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="TECKIN Bombilla LED inteligente WiFi  | Amazon » 15,99€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Smart Wifi Plug Power Strip ...**](https://amzn.to/2I844dL)</p><p>Bombilla RGBW de 7.5W WiFi de la marca Teckin que se integra en _**Smart Life**_.</p><p>Compatible con Alexa y con Google Home además de que deberíamos poder integrarlas en Home Assistant.</p> | <div> ![img-500crop][amzn-b.teckin] </div> <div> <a href="https://amzn.to/2I844dL" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-iraza]: user://pages/03.enchufes-Inteligentes/02.regletas-wifi/iraza.png?lightbox=1024&cropResize=500,500
[amzn-Konesky]: user://pages/03.enchufes-Inteligentes/02.regletas-wifi/Konesky.png?lightbox=1024&cropResize=500,500
[amzn-b.teckin]: user://pages/09.iluminacion/bombillas-wifi/bombilla_teckin.png?lightbox=1024&cropResize=500,500

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
![](integracion_google_home.gif)

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

[/ui-tab]

[/ui-tabs]