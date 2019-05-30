---
title: 'Tiras de Led'
media_order: tira_led_5m.png
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> Las tiras LED son un tipo de iluminación increíblemente versátil, con una amplia variedad de usos que pueden ir desde decorativos hasta usos más funcionales y profesionales. Esta versatilidad se refleja principalmente en su facilidad de instalación y las múltiples características que presentan los diferentes tipos de tiras de luces ...

Son un tipo de iluminación cada vez más utilizadas por las personas que buscan conseguir el máximo ahorro posible. **Pueden consumir hasta un 80% menos de energía que las bombillas tradicionales**, además de tener una duración claramente superior.

!!! Otra de las grandes ventajas de una tira led es que **es autoadhesiva** por lo que es muy sencilla adaptarla a cualquier tipo de superficie. Además, su iluminación es muy nítida, no causará ningún tipo de reflejo y será capaz de adaptarse a nuestra vista sin cansarla de ninguna manera.
Tienen  múltiples funciones son como perfecto acompañamiento de luz para espacios fijos que necesitas alumbrar, como un hueco en un cabecero, una guardilla en el pasillo, en el baño... 

!!! Convierte la iluminación de tu casa en una experiencia extraordinaria propia de una casa inteligente!

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Tira LED Tira Iluminación Inteligente RGB   | Amazon » 29,99€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Tira LED Tira Iluminación Inteligente RGB ...**](https://amzn.to/2Wvcghj)</p><p>WIFI Tira LED Tira Iluminación Inteligente RGB 5M</p><p> Bawoo 150 LED Smart Strip LED Impermeable ALEXA Google Home IFTTT. Teléfono Control Remoto 24 Teclas.</p><p> Puede controlar la tira de LED utilizando la aplicación "Magic Home" para encenderla, apagarla, cambiar de color, agregar un programa, crear un escenario, (Can 10m).</p> | <div> ![img-500crop][amzn-led5m] </div> <div> <a href="https://amzn.to/2Wvcghj" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="Utorch Bombilla LED 7W RGB | Aliexpress » 11,78€"]

|  |  |
|:------|:-----------------------:|
| <p>[**Utorch Bombilla LED 7W RGB...**](http://s.click.aliexpress.com/e/bkqswhgU)</p> Bombilla Utorch RGB WiFi que nos permiten la iluminación de una habitación.</p><p> Es RGBW y funciona con Google Assistant, Alexa e IFTTT.</p><p> Se integra en _**SmartLife**_, por lo que deberíamos poder integrarlo en _**Home Assistant**_.</p> | <div> ![img-500crop][ali-utorch] </div> <div> <a href="http://s.click.aliexpress.com/e/bkqswhgU" alt="AlieExpress-link" target="_blank"> <button type="button" style="color:#fff;background-color:#e8a100;width:100%;height:35px;"><i class="fa fa-shopping-cart  fa-lg"> AliExpress</i></button></a> </div> |

[/ui-accordion-item]

[ui-accordion-item title="Teckin Bombilla LED inteligente WiFi  | Amazon » 15,99€ "]

|  |  |
|:------|:-----------------------:|
| <p>[**Teckin Bombilla LED inteligente WiFi...**](https://amzn.to/2I844dL)</p><p>Bombilla RGBW de 7.5W WiFi de la marca Teckin que se integra en _**Smart Life**_.</p><p>Compatible con Alexa y con Google Home además de que deberíamos poder integrarlas en **_Home Assistant_**.</p> | <div> ![img-500crop][amzn-led5m] </div> <div> <a href="https://amzn.to/2I844dL" alt="amazon-link" target="_blank"><button type="button" style="color:#fff;background-color:#1694CA;width:100%;height:35px;margin:5px;"><i class="fa fa-amazon fa-lg">mazon</i></button></a> </div> |

[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-led5m]: user://pages/09.iluminacion/02.tiras-de-led/tira_led_5m.png?lightbox=1024&cropResize=500,500
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