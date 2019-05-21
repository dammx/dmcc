---
title: 'TP-Link HS100 y HS110'
media_order: 'Screenshot_1.png,tp-link-hs-100.png,tp-link-hs-110.png,integracion_google_home.gif,up1_azul1.png'
metadata:
    key(enchufes_wifi): 'Valor(domotizar,casa,enchufes,programar,tp-link,inteligentes,programar,home,assistant,hs100,hs110,regletas,android,iphone,aliexpress,amazon)'
taxonomy:
    category:
        - docs
    tag:
        - domotizar
        - casa
        - enchufes
        - programar
        - tp-link
        - inteligentes
        - home
        - assistant
        - hs100
        - hs110
        - regletas
        - android
        - iphone
        - aliexpress
        - amazon
sitemap:
    changefreq: hourly
    priority: 0.5
process:
    markdown: true
    twig: true
visible: true
---

![win10](image://os-compat.png)

---

<div>
<button type="button" style="color:#fff;background-color:#1694CA;width:200px;height:50px;"><i class="fa fa-amazon fa-lg">mazon!</i></button><br /><br />

<button type="button" style="color:#fff;background-color:#e8a100;width:200px;height:50px;"><i class="fa fa-shopping-cart fa-lg"> AliExpress!</i></button>    
</div>

<div><button type="button" style="color: #fff; background-color: #1694ca; width: 200px; height: 50px;"><i class="fa fa-amazon fa-lg">mazon!><a href="https://amzn.to/2HjWRab" title="amazon-link" target="_blank"></a></i></button>
<br /><br />
<button type="button" style="color: #fff; background-color: #e8a100; width: 200px; height: 50px;"><i class="fa fa-shopping-cart fa-lg"> AliExpress!</i></button></div>





    
    
---

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

TP-Link cuenta con dos modelos con WiFi, el _HS100_ y el _HS110_. Ambos cuentan con las mismas funciones de control mediante la aplicación, programación, modo de simulación de que hay gente en casa... etc. Sin embargo, el _HS110_ también mide el consumo energético de los aparatos que le conectamos, y saca resúmenes semanales y mensuales. Podemos controlarlos con la voz con **Google Home**.
![](Screenshot_1.png)
Para controlar ambos hay que descargar la aplicación Kasa para [iOS](https://apple.co/2WveAlg) o [Android](http://bit.ly/2YgEx8L). El HS100 vale 19,99 euros, y el HS110 vale 27,99 euros. Ambos funcionan por WiFi de 2,4 GHz, se pueden controlar desde fuera de casa, y tienen garantía de 3 años.

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="TP-Link HS100 | Amazon » 19,90€"]
|  |  |
|:-------------|:-------------:|
| <p>[**TP-Link HS100 - Enchufe inteligente para controlar<br /> sus dispositivos desde cualquier lugar...**](https://amzn.to/2Lj7sHB)</p><p>- **Acceso remoto**: Controla dispositivos conectados al Enchufe<br/>Inteligente donde tengas Internet, utilizando la app gratuita<br/>**Kasa** en tu smartphone.</p><p>- **Programación:** Programa el Enchufe Inteligente para que<br/>automáticamente encienda o apague la alimentación de los<br/> electrodomésticos según sea necesario: **Encender la luz al <br/>anochecer o apagarla al amanecer** ...</p> | ![200x200][amzn-TPL-HS100] [![buy-mzn!][buy-mzn]](https://amzn.to/2Lj7sHB)</p> |
[/ui-accordion-item]

[ui-accordion-item title="TP-Link HS110 | Amazon » 27.99€"]
|  |  |
|:-------------|:-------------:|
| <p>[**TP-Link HS110 - Enchufe inteligente para controlar<br /> sus dispositivos desde cualquier lugar...**](https://amzn.to/2HjWRab)</p><p>- **Acceso remoto**: Controla dispositivos conectados al Enchufe<br/>Inteligente donde tengas Internet, utilizando la app gratuita<br/>**Kasa** en tu smartphone.<br />**Programación:** Programa el Enchufe Inteligente para que<br/>automáticamente encienda o apague la alimentación de los<br/> electrodomésticos según sea necesario: **Encender la luz al <br/>anochecer o apagarla al amanecer** ...</p> | ![200x200][amzn-TPL-HS110] [![buy-mzn!][buy-mzn]](https://amzn.to/2HjWRab)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEL ARTÍCULO --->

[amzn-TPL-HS100]: user:/pages/03.enchufes-Inteligentes/01.tp-link-hs100-hs110/tp-link-hs-100.png?lightbox=1024&cropResize=200,200
[amzn-TPL-HS110]: user://pages/03.enchufes-Inteligentes/01.tp-link-hs100-hs110/tp-link-hs-110.png?lightbox=1024&cropResize=200,200
[buy-mzn]: https://dabuttonfactory.com/button.png?t=Comprar+en+AMAZON!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=037ba2

<!--- OCULTO: ![buy-aliex!][buy-aliex] --->
[buy-aliex]: https://dabuttonfactory.com/button.png?t=Comprar+en+ALIEXPRESS!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=ffae00

---

[![](up1_azul1.png)](# "Volver al Inicio")

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