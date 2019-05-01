---
title: 'Instalación en Windows'
media_order: Interface.png
taxonomy:
    category:
        - docs
visible: true
---

Con el fin de hacer pruebas y aprender el funcionamiento, empecé por instalar Home Assistant en windows, antes de comprar un Rasperri pi, más el alimentador, la tarjeta SD y demás accesorios, que supondria un coste adicional de unos 80€, opté por esta opción. para mi fue una buena opción para poder empezar a probar dispositivos básicos como enchufes y interruptores que como veréis en el blog, estan a un precio accesible, a partir de ahí, fui ampliando la instalacion con varios dispositivos.
La ventaja de instalar en Windows, para los que no somos programadores, es que tienes acceso al archivo "configuration.yaml",el archivo madre de la configuracion de Home Assistant, sin tener que hacer grandes instalaciones de acceso a través de DDns o configuraciones más complicadas.

Empezaremos por instalar Python 3 en Windows, lo podremos hacer desde este enlace: [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)

Abriremos una consola de comandos cmd:

py -m pip install homeassistant

py -m homeassistant —-open-ui


Al final de la instalación, ya podremos entrar en Home Assistant a través del navegador con una direccion URL:  [http://localhost:8123](http://localhost:8123)

![Inferface](Interface.png)

Nos pedirá que creemos un usuario con contraseña y estaremos dentro de la configuración de Home Assistant.




 


