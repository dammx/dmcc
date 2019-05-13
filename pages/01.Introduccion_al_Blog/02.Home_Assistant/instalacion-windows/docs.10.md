---
title: 'Instalación en Windows'
media_order: 'Inicio Home Assistant.png'
metadata:
    'key(instalacion,home,assistant,windows)': 'Valor(domotizar,casa,windows,python,wi-fi,wifi,home,assistant,aliexpress,amazon'
taxonomy:
    category:
        - docs
visible: true
---

Con el fin de hacer pruebas y aprender el funcionamiento, empecé por **instalar Home Assistant en Windows**, antes de comprar un Rasperri pi, más el alimentador, la tarjeta SD y demás accesorios, que supondría un coste adicional de unos 80€, opté por esta opción. para mi fue una buena opción para poder empezar a probar dispositivos básicos como enchufes y interruptores que como veréis en el blog, estan a un precio accesible, a partir de ahí, fui ampliando la instalación con varios dispositivos.
La ventaja de instalar en Windows, para los que no somos programadores, es que **tienes acceso al archivo "configuration.yaml**",el archivo madre de la configuración de Home Assistant, sin tener que hacer grandes instalaciones de acceso a través de DDns o configuraciones más complicadas.

**Empezaremos por instalar Python3 en Windows:**<br/>lo podremos hacer desde este enlace: [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)

**Instalación Home Assistant en Windows:**<br/> Abriremos una consola de comandos `cmd` y escribiremos lo siguiente:

```
  py -m pip install homeassistant (Enter)  
  py -m homeassistant —-open-ui (Enter)
  
```

Al final de la instalación, ya podremos entrar en Home Assistant a través del navegador con una dirección URL:  [http://localhost:8123](http://localhost:8123)

Nos pedirá que creemos un usuario con contraseña y estaremos dentro de la configuración de Home Assistant.
![](Inicio%20Home%20Assistant.png)





 

