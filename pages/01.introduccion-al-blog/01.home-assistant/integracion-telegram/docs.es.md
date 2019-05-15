---
title: 'Integración Telegram'
media_order: hate.png
taxonomy:
    category:
        - docs
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

Cuando no proponemos tener una casa inteligente, nos damos cuenta que necesitamos estar informados de todos los cambios que pertenezcan a los dispositivos de la casa, si se ha quedado la puerta de garaje abierta al irnos, si se  ha disparado la alarma cuando no estamos en casa , o , si se ha encendido el termostato por error.
![](hate.png)
Todos estos cambios de estado se pueden automatizar con un mensaje vía la Aplicación Telegram, n sistema de mensajería que, para aquellos que no lo conozcáis, es un estilo a Whatsapp, solo que, en mi opinión, es mucho mejor en todos los aspectos, entre ellos, con la existencia de los “bots”, es decir, robots con los que podemos interactuar y, en nuestro caso, haremos que sea “la voz” de nuestra casa. para ello necesitamos realizar unos pasos sencillos y podremos integrar este servicio en nuestro sistema domótico 


Si ya tenéis Telegram, podéis seguir la guía de integración, pero, para aquellos que no, os recomiendo que busquéis en vuestra tienda de aplicaciones, como _Play Store_ o _App Store_, para descargarlo y ponerlo en marcha, al igual que se hace en Whatsapp. Una vez que tengáis Telegram en funcionamiento, podemos seguir para crear nuestro bot, el cual, será el que nos informará y más adelante podrá recibir órdenes para poder hacer cosas en casa desde Telegram.

---

[/ui-tab]

[ui-tab title="Integración ..."]

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
---

[/ui-tab]

[/ui-tabs]