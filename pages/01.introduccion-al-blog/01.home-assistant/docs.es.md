---
title: 'Home Assistant'
media_order: Interface.png
metadata:
    key(home_assistant): 'Valor(domotizar,casa,home,assistant,wi-fi,windows,wifi,plex,kodi,arduino,python3,python,google,iftt,xiaomi)'
taxonomy:
    category:
        - docs
    tag:
        - domotizar
        - casa
        - home
        - assistant
        - wi-fi
        - windows
        - wifi
        - plex
        - kodi
        - arduino
        - python3
        - python
        - google
        - iftt
        - xiaomi
sitemap:
    changefreq: hourly
    priority: 0.5
visible: true
---

**Home Assistant** es una plataforma de domótica de código abierto que se ejecuta en _Python3_. También te da la posibilidad de rastrear y controlar todos los dispositivos del hogar y automatizar su control.
![](Interface.png)
**Home Assistant** se suele montar en un dispositivo como un **_Raspberry Pi_**, **_Orange Pi Zero_** o **Windows** **(la mejor opción de entrada para poder aprender y no tener que invertir en un nuevo dispositivo)**
Lo que hacemos con este software es centralizar el control de todos estos aparatos para no tener que controlarlos de forma independiente.

Todo este sistema se puede gestionar de forma totalmente modular, pudiendo organizar a nuestro gusto todos los dispositivos de manera que podamos encontrarlos rápidamente cuando lo necesitemos y no tener que buscarlos dentro de una caótica interfaz como ocurre con otras plataformas alternativas.



**Home Assistant se integra con distintos servicios:**<br/>
**Home Assistant** se encargará de controlar automáticamente el estado de todos los dispositivos inteligentes además de darnos la posibilidad de usar aplicaciones como _IFTTT_ para crear recetas, _Plex_, _Kodi_ o _Arduino_. Además, se puede integrar con una gran variedad de APIs como _HUE_, _Nest_, _WeMo_ e incluso dispositivos _Xiaomi_.

**Automatización:**<br/>
**Home Assistant** se basa en reglas para controlar el sistema. Todas las reglas cuentan con tres elementos:

* **Trigger**: lo que hace que se lance la regla.
* **Condition**: condición a comprobar para que se ejecute la regla.
* **Action**: acción que realiza la regla.

En cualquier de estos tres elementos cuentas con un motor de plantillas que te permiten extender las comprobaciones a algo más allá de la simple: "si _A_ entonces _B_".

Gracias a esta característica puedes crear variables, aplicar transformaciones y hacer todas las comprobaciones que consideres necesarias.

**Interfaz:**<br/>
Su interfaz esta basada en _Material Design_ y cuenta con varias características interesantes como el soporte a _WebSockets_ que permite al sistema reaccionar en tiempo real. Esto permite mostrar los valores de los sensores en cada momento sin necesidad de recargar la página.

Podemos decir en resumen que su interfaz es simple, clara y moderna, perfectamente adaptable a cualquier dispositivo.

---
