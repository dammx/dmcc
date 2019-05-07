---
title: 'nMap para windows (Tracker ID)'
metadata:
    key(nmap_para_windows): 'Valor(Blog,Grav)'
    key(nmap_windows): 'Valor(Blog,Grav)'
taxonomy:
    category:
        - docs
visible: true
---

#### nMap ###
#### (Rastreador dispositivos conectado a la red) ####

**Instalando este rastreador de dispositivos en un sistema conectado a nuestra red, podremos crear automatizaciones en Home Assistant basadas en nuestra presencia en nuestra casa.**

Puedes descargarlo desde aqui: [nMap para Windows](http://bit.ly/2Lud6Xs)

Nmap ("Network Mapper") es una herramienta de código abierto para la exploración de redes y la auditoría de seguridad. Fue diseñado para escanear rápidamente redes grandes, aunque funciona bien contra hosts individuales. Nmap utiliza paquetes de IP sin procesar en formas novedosas para determinar qué hosts están disponibles en la red, qué servicios (nombre y versión de la aplicación) ofrecen esos hosts,
qué sistemas operativos (y versiones de sistema operativo) están ejecutando, qué tipo de filtros de paquetes / cortafuegos están en uso, y docenas de otras características. Si bien Nmap se usa comúnmente para auditorías de seguridad, muchos administradores de sistemas y redes lo encuentran útil para tareas rutinarias como el inventario de redes, la administración de programas de actualización de servicios,
y monitoreando el tiempo de actividad del host o del servicio.

La salida de Nmap es una lista de objetivos escaneados, con información complementaria sobre cada uno, dependiendo de las opciones utilizadas. La clave entre esa información es la "tabla de puertos interesantes". Esa tabla muestra el número de puerto y el protocolo, el nombre del servicio y el estado. El estado es abierto, filtrado, cerrado,
o sin filtrar. Abrir significa que una aplicación en la máquina de destino está escuchando las conexiones / paquetes en ese puerto. Filtrado significa que un firewall, filtro u otro obstáculo de la red está bloqueando el puerto, por lo que Nmap no puede saber si está abierto o cerrado. Los puertos cerrados no tienen aplicación escuchando en ellos,
aunque podrían abrirse en cualquier momento. Los puertos se clasifican como no filtrados cuando responden a las sondas de Nmap, pero Nmap no puede determinar si están abiertas o cerradas. Nmap informa de las combinaciones de estado abierto | filtrado y cerrado | filtrado cuando no puede determinar cuál de los dos estados describe un puerto.
La tabla de puertos también puede incluir detalles de la versión del software cuando se ha solicitado la detección de la versión. Cuando se solicita una exploración de protocolo IP (-sO), Nmap proporciona información sobre protocolos IP compatibles en lugar de puertos de escucha.

Además de la interesante tabla de puertos, Nmap puede proporcionar más información sobre los destinos, incluidos los nombres de DNS inversos,
adivinanzas del sistema operativo, tipos de dispositivos y direcciones MAC.

En el Ejemplo 15.1 se muestra una exploración típica de Nmap. Los únicos argumentos de Nmap utilizados en este ejemplo son -A, para habilitar la detección de versiones y sistemas operativos, escaneo de scripts y traceroute; -T4 para una ejecución más rápida; y luego el nombre de host.



