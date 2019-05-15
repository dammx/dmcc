---
title: 'nMap para windows (Tracker ID)'
media_order: 'trakers.png,devices.png'
metadata:
    'key(nmap,windows)': 'Valor(domotizar,casa,windows,wifi,wi-fi,inteligente,nmap,home,python,assistant,tracker,rastrear,dispositivo'
taxonomy:
    category:
        - docs
    tag:
        - domotizar
        - casa
        - windows
        - wifi
        - wi-fi
        - inteligente
        - nmap
        - home
        - python
        - assistant
        - tracker
        - rastrear
        - dispositivo
sitemap:
    changefreq: hourly
    priority: 0.5
visible: true
---

### nMap ###

!!! Rastreador dispositivos conectado a la red)
!!! * Instalando este rastreador de dispositivos en un sistema conectado a nuestra red, podremos crear automatizaciones en Home Assistant basadas en nuestra presencia en nuestra casa.
!!! * Puedes descargarlo desde aquí: [nMap para Windows](https://nmap.org/dist/nmap-7.70-setup.exe)

_Nmap_ ("Network Mapper") es una herramienta de código abierto para la exploración de redes y la auditorías de seguridad. Fue diseñado para escanear rápidamente redes grandes, aunque funciona bien contra _hosts_ individuales. _Nmap_ utiliza paquetes de IP sin procesar en formas novedosas para determinar qué _hosts_ están disponibles en la red, qué servicios (nombre y versión de la aplicación) ofrecen esos hosts,
qué sistemas operativos (y que versiones de sistema operativo) se están ejecutando, qué tipo de filtros de paquetes / cortafuegos están en uso, y docenas de otras características. Si bien _Nmap_ se usa comúnmente para auditorías de seguridad, muchos administradores de sistemas y redes lo encuentran útil para tareas rutinarias como el inventario de redes, la administración de programas de actualización de servicios y/o monitorear el tiempo de actividad del _host_ o del servicio.

Para editar el archivo `configuration.yaml` recomendamos que utilices el editor [_Notepad++_](https://notepad-plus-plus.org/download/)

Para la configuración de **"nmap device tracker"** debes añadir ésto en tu `configuration.yaml`:

```
device_tracker:
  - platform: nmap_tracker
    hosts: 192.168.1.0/24
```  
Una vez añadido y guardado el archivo `configuration.yaml` ,debes reiniciar **Home Assistant**.

La salida de _Nmap_ es una lista de objetivos escaneados, que se guardan en un fichero `known_devices.yaml` dentro de la carpeta de la configuración de `.homeassistant`, los cuales podrás editar y nombrar e incluso asignar una imagen personalizada
![](devices.png)

```
b0_e1_7e_2a_6a_ca:
  hide_if_away: false
  icon:
  mac: B0:E1:7E:2A:6A:CA
  name: Eric                    # <- Nombre del dispositivo o del ususario
  picture:  /local/Eric1.jpg    # <- imagen del dispositivo o del usuario
  track: true                   # <- mostrar: `true` /  ocultar: `false`
```
La imagen debes tenerla en una carpeta, dentro de `.homeassistant`, y llamarla `www`, si no la tienes debes crearla.
![](trakers.png)
  
    





