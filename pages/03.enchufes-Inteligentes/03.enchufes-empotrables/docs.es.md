---
title: 'Enchufes Empotrables'
media_order: 'Kaifire.png,Jindia.png,shukowifi.png'
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
| <p>[**Kaifire USB Enchufe Pared 2.4A Schuko<br/> Toma de Corriente Estándar<br/> con 2 USB Conectores...**](https://amzn.to/2HqTtKl)</p><p>- **Acceso remoto**: Controla dispositivos<br/> conectados al Enchufe<br/> Inteligente donde tengas Internet,<br/> utilizando la app gratuita<br/> **SmartLife** en tu smartphone.<br/>- **Programación:** Programa el Enchufe Inteligente<br/> para que automáticamente encienda<br/> o apague la alimentación de los<br/> electrodomésticos según sea necesario:...</p> | ![200x200][amzn-Kaifire] [![buy-mzn!][buy-mzn]](https://amzn.to/2HqTtKl)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Jindia 2.4A Schuko Enchufe Pared | Amazon » 13,49€"]
|  |  |
|:-------------|:-------------:|
| <p>[**Jindia 2.4A Schuko Enchufe para la pared<br/> 2 puertos de carga USB,<br/> Blanco/Gris...**](https://amzn.to/2LIBu7T)</p><p>- **Acceso remoto**: Toma de contacto<br/> con protección infantil integrada.<br/> Uso simultáneo de todos los puertos,<br/> USB a 2.4A.<br/>Para la carga sin complicaciones de todos<br/> los dispositivos móviles que tienen una interfaz<br/> USB, como por ejemplo iPhones,<br/> iPads y teléfonos inteligentes.<br/>La carga máxima de los dos puertos USB<br/> es de 2.4A...</p> | ![200x200][amzn-Jindia][![buy-mzn!][buy-mzn]](https://amzn.to/2LIBu7T)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Toma corriente 15A UE 2 puertos USB | Aliexpress » 18,71€"]
|  |  |
|:-------------|:-------------:|
| <p>[**Toma Schuko Enchufe Pared 15A<br/> 2 puertos de carga USB,<br/> Blanco/...**](http://s.click.aliexpress.com/e/86Y7JIs)</p><p>- **Acceso remoto**: Toma de corriente<br/> con protección infantil integrada 15A.<br/> Uso simultáneo de todos los puertos,<br/> USB a 2.4A.<br/>Para la carga sin complicaciones de todos<br/> los dispositivos móviles que tienen una interfaz<br/> USB, como por ejemplo iPhones,<br/> iPads y teléfonos inteligentes.<br/>La carga máxima de los dos puertos USB<br/> es de 2.4A...</p> | ![200x200][amzn-shukowifi] [![buy-aliex!][buy-aliex]](http://s.click.aliexpress.com/e/86Y7JIs)</p> |
[/ui-accordion-item]
[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-Kaifire]: user:/pages/03.enchufes-Inteligentes/03.enchufes-empotrables/Kaifire.png?lightbox=1024&cropResize=200,200
[amzn-Jindia]: user://pages/03.enchufes-Inteligentes/03.enchufes-empotrables/Jindia.png?lightbox=1024&cropResize=200,200
[amzn-shukowifi]: user://pages/03.enchufes-Inteligentes/03.enchufes-empotrables/shukowifi.png?lightbox=1024&cropResize=200,200
[buy-mzn]: https://dabuttonfactory.com/button.png?t=Comprar+en+AMAZON!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=037ba2
[buy-aliex]: https://dabuttonfactory.com/button.png?t=Comprar+en+ALIEXPRESS!&f=Roboto-Bold&ts=16&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=ffae00

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