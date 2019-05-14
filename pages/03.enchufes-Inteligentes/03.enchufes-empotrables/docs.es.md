---
title: 'Enchufes Empotrables'
media_order: Kaifire.png
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

Toma de contacto de protección con 2 conectores USB tipo A. Conexiones hasta cable de 2,5 mm².<br/>
Toma de contacto de protección con protección infantil integrada. Uso simultáneo de todos los puertos,USB a 2.4A.<br/>
Para la carga sin complicaciones de todos los dispositivos móviles que tienen una interfaz USB, como por ejemplo iPhones, iPads y teléfonos inteligentes.<br/>
Girado alrededor por la descripción simple.La carga máxima de los dos puertos USB es de 2.4A.<br/>
El zócalo está protegido por una protección electrónica contra cortocircuitos, una protección contra sobrecargas y una función de filtro de línea.
![](Kaifire.png)

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Kaifire USB Enchufe Pared 2.4A Schuko | Amazon » 13,99€"]
|  |  |
|:-------------|:-------------:|
| <p>[**Kaifire USB Enchufe Pared 2.4A Schuko Toma de Corriente Estándar con 2 USB Conectores...**](https://amzn.to/2HqTtKl)</p><p>- **Acceso remoto**: Controla dispositivos conectados al Enchufe<br/>Inteligente donde tengas Internet, utilizando la app gratuita<br/>**SmartLife** en tu smartphone.</p><p>- **Programación:** Programa el Enchufe Inteligente para que<br/>automáticamente encienda o apague la alimentación de los<br/> electrodomésticos según sea necesario: **Encender cualquier electroméstico en cualquier lugar y/o momento** ...</p> | ![200x200][amzn-TPL-HS100] [![buy-mzn!][buy-mzn]](https://amzn.to/2HqTtKl)</p> |
[/ui-accordion-item]

[ui-accordion-item title="TP-Link HS110 | Amazon » 27.99€"]
|  |  |
|:-------------|:-------------:|
| <p>[**TP-Link HS110 - Enchufe inteligente para controlar<br /> sus dispositivos desde cualquier lugar...**](https://amzn.to/2HjWRab)</p><p>- **Acceso remoto**: Controla dispositivos conectados al Enchufe<br/>Inteligente donde tengas Internet, utilizando la app gratuita<br/>**Kasa** en tu smartphone.<br />**Programación:** Programa el Enchufe Inteligente para que<br/>automáticamente encienda o apague la alimentación de los<br/> electrodomésticos según sea necesario: **Encender la luz al <br/>anochecer o apagarla al amanecer** ...</p> | ![200x200][amzn-TPL-HS110] [![buy-mzn!][buy-mzn]](https://amzn.to/2HjWRab)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-TPL-HS100]: user:/pages/03.enchufes-Inteligentes/03.enchufes-empotrables/Kaifire.png?lightbox=1024&cropResize=200,200
[amzn-TPL-HS110]: user://pages/03.enchufes-Inteligentes/01.tp-link-hs100-hs110/tp-link-hs-110.png?lightbox=1024&cropResize=200,200
[buy-mzn]: https://dabuttonfactory.com/button.png?t=Comprar+en+AMAZON!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=037ba2

<!--- OCULTO: ![buy-aliex!][buy-aliex] --->
[buy-aliex]: https://dabuttonfactory.com/button.png?t=Comprar+en+ALIEXPRESS!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=ffae00

---

[/ui-tab]

[ui-tab title="Integración ..."]

La **Integración en Google Home** es muy secilla, solo tienes que añadir la cuenta que creas de la aplicacion del disposivo en la configuracion de añadir dispositivos de Google Home:
![](integracion_google_home.gif)
**Para Integrarlo en Home Assitant**


+ Ejemplo `configuration.yaml` entradas con IP's específicas:

```text
tplink:
  discovery: false
  light:
    - host: 192.168.200.1
    - host: 192.168.200.2
  switch:
    - host: 192.168.200.3
    - host: 192.168.200.4
```
---

[/ui-tab]

[/ui-tabs]