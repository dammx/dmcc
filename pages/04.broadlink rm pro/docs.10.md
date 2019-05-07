---
title: 'BroadlinkRM Pro WIFI + IR + Control RemotoRF'
media_order: 'Broadlink.png,rm_pro.png,rm_mini_3.png'
published: true
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> ¿Cansado de que todo tu mundo dependa de numerosos mandos a distancia? Si miras a tu alrededor posiblemente encuentres numerosos electrodomésticos en tu hogar, tienen uno, lo cual no hace más que complicar las cosas ...

Pues bien, ahora el `Broadlink RM pro WIFI + IR + Control Remoto RF` es un dispositivo nuevo que ha venido a facilitarte la vida. Y es una novedad asombrosa que ya puedes comprar en _Amazon_ o _Aliexpress_.

Televisores, aires acondicionados, ventanas, reproductores de música y reproductores de DVD funcionan mediante mandos a distancia. Para facilitar su uso a veces se usan versiones universales, aunque estas no son siempre compatibles con todos los electrodomésticos del hogar. Pero esto cambia definitivamente con esta novedad de la electrónica.

---

[ui-accordion independent=true open=none]

[ui-accordion-item title="Broadlink RM pro | »39,89€"]
|  |  |
|:-------------|:-------------:|
| <p>[**BroadLink RM Pro+ WiFi Smart Home...**](https://amzn.to/2Lskans)</p><p>Automatización Todo en uno<br /> Aprendizaje Controlador Remoto Universal<br /> Compatible para Dispositivos iOS/Android<br /> (EU Standard)</p><p> | ![200x200][amzn-BL-RMPRO] [![buy-mzn!][buy-mzn]](https://amzn.to/2Lskans)</p> |
[/ui-accordion-item]

[ui-accordion-item title="Broadlink RM Mini3 | » 19.99€"]
|  |  |
|:-------------|:-------------:|
| <p>[**Broadlink RM Mini3...**](https://amzn.to/2WtK7DW)</p><p>-Wi-Fi Universal Remote integra todos<br />tus dispositivos controlados IR-<br />En comparacióncon RMPRO,<br />no dispone la función de RF 433 Mhz.<br /> Con la aplicación IHC en tu<br />teléfono inteligente puedes controlar<br />todos los dispositivos,<br /> usa un cable USB para conectar con<br />la energía.<br /> Fácil configuración.</p> | ![200x200][amzn-BL-RMMINI3] [![buy-mzn!][buy-mzn]](https://amzn.to/2WtK7DW)</p> |
[/ui-accordion-item]

[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-BL-RMPRO]: user://pages/04.BroadlinkRM+Pro+WIFI+IR+Control+RemotoRF/rm_pro.png?lightbox=1024&cropResize=200,200
[amzn-BL-RMMINI3]: user://pages/04.BroadlinkRM+Pro+WIFI+IR+Control+RemotoRF/rm_mini_3.png?lightbox=1024&cropResize=200,200
[buy-mzn]: https://dabuttonfactory.com/button.png?t=Comprar+en+AMAZON!&f=Roboto-Bold&ts=18&tc=fff&w=200&h=40&c=5&bgt=unicolored&bgc=037ba2

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
