---
title: Sensores
media_order: Up.png
published: true
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

---

[ui-accordion independent=true open=none]
[ui-accordion-item title="Sensor de puerta o ventana RF 433 Mhz| Aliexpress » 3,06€ "]


<a href="http://s.click.aliexpress.com/e/c67wZ348" target="_parent"><img src="//ae01.alicdn.com/kf/HTB1wpymafvsK1Rjy0Fiq6zwtXXaD/-font-b-Qolelarm-b-font-font-b-house-b-font-font-b-433MHz-b-font.jpg_220x220.jpg"/><span style="display:block;">Sensor de puerta o ventana con conectividad 433 Mhz. Podemos usarlo en HA si tenemos algún gateway de RF como el Sonoff Bridge. </span></a>      
[/ui-accordion-item]


    
[/ui-accordion]

<!--- REFERENCIA A IMAGENES AL PIE DEl ARTÍCULO --->

[amzn-touch2]: user://pages/02.interruptores/sonoff_touch2.png?lightbox=1024&cropResize=500,500
[amzn-touch1]: user://pages/02.interruptores/touch1.png?lightbox=1024&cropResize=500,500
[amzn-basic]: user://pages/02.interruptores/basic.png?lightbox=1024&cropResize=500,500
[amzn-touch3]: user://pages/02.interruptores/sonoff_touch3.png?lightbox=1024&cropResize=500,500
[amzn-shelly1]: user://pages/02.interruptores/shelly11.png?lightbox=1024&cropResize=500,500
[amzn-persiana]: user://pages/02.interruptores/Persiana.png?lightbox=1024&cropResize=500,500
[amzn-vhome]: user://pages/02.interruptores/vhome.png?lightbox=1024&cropResize=400,400

---

[![](up1_azul1.png)](# "Volver al Inicio")

[/ui-tab]

[ui-tab title="Integración ..."]

La **Integración en Google Home** es muy secilla, solo tienes que añadir la cuenta que creaste en la aplicacion del disposivo, en este caso sera **_eWelink_**, para los dispositivos **_Sonoff_** y **_Shelly Cloud_**, para los dispositivos **_Shelly_**, en la configuración de añadir dispositivos de _Google Home_, aquí tenéis los enlaces para descargar la que necesitéis:
 * [**eWelink android**](http://bit.ly/304iAeG)
 * [**eWelink Iphone**](https://apple.co/2VO5ZwV)    
 * [**Shelly Cloud android**](http://bit.ly/2DYDjHj)
 * [**Shelly Cloud Iphone**](https://apple.co/2WuWTCk)

###### **_(Aúnque en el Ejemplo usamos la aplicación Kasa, el procedimiento para la integración és el mismo, utilizando la aplicación correcta del componente, arriba indicada, según proceda)._**.###### 
![](integracion_google_home.gif)

**Para Integrarlo en Home Assitant**

+ Ejemplo configuración dispositivos **_Shelly_**  `configuration.yaml`:

```text

switch:
  - platform: rest
    name: "Shelly2 Switch1"
    scan_interval: 5
    resource: http://192.168.0.28/relay/0    (IP de nuestro Shelly1)
    body_on: 'turn=on'
    body_off: 'turn=off'
    is_on_template: '{{ value_json.ison == true}}'
    headers:
      content-type: application/x-www-form-urlencoded

```
+ Ejemplo configuración dispositivos **_Sonoff_**  `configuration.yaml`:

```text

sonoff:
  username: nuestrocorreo@correo.es
  password: nuestracontraseña
  scan_interval: 60
  grace_period: 600
  api_region: 'eu'

```
!! _"En el caso de la configuración de los disposivos **Sonoff**, la aplicación **eWelink**, **no permite estar abierta en dos aplicaciones al mismo tiempo** así que, recomiendo que abras otra cuenta de correo, solo para Home Assistant, y que désde la cuenta principal del móvil, compartas los dispositivos a la cuenta de correo de Home Assistant, de ésta manera podrá estar abierta en las dos aplicaciones a la vez."_
---

[/ui-tab]

[/ui-tabs]