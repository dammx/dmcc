---
title: 'Instalación en Windows'
media_order: 'Inicio Home Assistant.png,2019-05-15_11-38-45.gif,2019-05-15_11-49-16.gif'
metadata:
    key(home_assistant_windows): 'Valor(domotizar,casa,windows,python,wi-fi,wifi,home,assistant)'
taxonomy:
    category:
        - docs
    tag:
        - domotizar
        - casa
        - windows
        - python
        - wi-fi
        - wifi
        - home
        - assistant
sitemap:
    changefreq: hourly
    priority: 0.5
visible: true
---

Con el fin de hacer pruebas y aprender el funcionamiento, empecé por **instalar Home Assistant en Windows**, antes de comprar un Rasperri pi, más el alimentador, la tarjeta SD y demás accesorios, que supondría un coste adicional de unos 80€, opté por esta opción. para mi fue una buena opción para poder empezar a probar dispositivos básicos como enchufes y interruptores que como veréis en el blog, estan a un precio accesible, a partir de ahí, fui ampliando la instalación con varios dispositivos.
La ventaja de instalar en Windows, para los que no somos programadores, es que **tienes acceso al archivo "configuration.yaml**",el archivo madre de la configuración de Home Assistant, sin tener que hacer grandes instalaciones de acceso a través de DDns o configuraciones más complicadas.<br />Su ubicación predeterminada en windows: `C:\Users\admin\AppData\Roaming\.homeassistant`<br />
Para editar el archivo `configuration.yaml` recomendamos que utilices el editor [_Notepad++_](https://notepad-plus-plus.org/repository/7.x/7.6.6/npp.7.6.6.Installer.exe)
___

**Empezaremos por instalar Python3 en Windows:**<br/>lo podremos hacer desde este enlace: [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)

---

**Instalación Home Assistant en Windows:**<br/> Abriremos una consola de comandos `cmd` y escribiremos lo siguiente:

```
  py -m pip install homeassistant (Enter)    
  
```

![home-assistant-install](2019-05-15_11-38-45.gif)

---

**Arranque Home Assistant:**

```
py -m homeassistant —-open-ui (Enter)

```
![home-assistant-open-ui](2019-05-15_11-49-16.gif)

+ Al final de la instalación, ya podremos entrar en **Home Assistant** a través del navegador con la dirección URL:  [http://localhost:8123](http://localhost:8123)

Finalmente, nos pedirá que creemos un _usuario_ con _contraseña_ y ya estaremos dentro de la configuración de **Home Assistant**!.

---





 


