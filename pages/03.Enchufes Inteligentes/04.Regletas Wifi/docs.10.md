---
title: 'Regletas Wifi'
media_order: 'iraza.png,Konesky.png,integracion_google_home.gif'
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

[ui-accordion-item title="Iraza Enchufe Múltiple Inteligente | Amazon » 29,99€ "]
|  |  |
|:-------------|:-------------:|
| <p>[**Iraza Enchufe Múltiple Inteligente...**](https://amzn.to/2J7yf7y)</p><p>Configuración simple y fácil de usar : <br />Siga los pasos de instalación.<br /> Investigación y desarrollo independientes,<br /> fácil de operar. <br />Y la conexión wifi es muy estable.<br />Control de voz de Amazon Alexa,<br /> Google Assistant.<br /> Puede activar o desactivar las 3 tomas<br /> por separado o juntas y<br /> los 2 puertos USB a través de <br />Echo o Google Home. NEST<br /> y Samsung Smart Things serán compatibles<br /> en breve.</p><p> | ![200x200][amzn-iraza][![buy-mzn!][buy-mzn]](https://amzn.to/2J7yf7y)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Konesky Smart Power Strips | Amazon » 29.99 "]
|  |  |
|:-------------|:-------------:|
| <p>[**Konesky Smart Power Strips Wifi<br /> Protector contra sobretensiones con <br />4 salidas 4 puertos USB...**](https://amzn.to/2Valrih)</p><p>La regleta de alimentación inalámbrica<br /> Timmer es compatible con los puertos USB,<br /> ahorra espacio y dinero, no necesita<br /> comprar muchos enchufes ni<br /> banco de energía, la regleta multifuncional <br />le permite cargar muchos dispositivos<br /> al mismo tiempo. <br />El control de voz de la toma<br /> de corriente inteligente wifi,<br /> puede controlar sus aplicaciones a través de<br /> los dispositivos<br /> Alexa / Google Home / IFTTT,<br /> conveniente y fácil de usar.</p> | ![200x200][amzn-Konesky][![buy-mzn!][buy-mzn]](https://https://amzn.to/2Valrih)</p> |
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

La **Integración en Google Home** es muy secilla, solo tienes que añadir la cuenta que creas de la aplicacion del disposivo, en este caso sera _Smart Life_ o _Tuya_,  en la configuración de añadir dispositivos de _Google Home_, aquí tenéis el enlace para descargarlo:
 * [**Smart Life android**](http://bit.ly/2JnEUtN)
 * [**Smart Life Iphone**](https://apple.co/2DVyRsK)
 * [**Tuya Android](http://bit.ly/2ZYql5T)
 * [**Tuya iphone](https://apple.co/2vIrNeD)
![](integracion_google_home.gif)

**Para Integrarlo en Home Assitant**
Solo necesitaras anadir a tu `configuration.yaml` los siguientes datos:

+ Ejemplo  App Tuya `configuration.yaml`:

```text

tuya:
  username: dmunoz.info@gmail.com
  password: abb40lsot
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







