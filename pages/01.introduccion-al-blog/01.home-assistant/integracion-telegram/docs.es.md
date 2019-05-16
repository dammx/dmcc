---
title: 'Integración Telegram'
media_order: 'hate.png,Telegram1.jpg,Telegram2.jpg,Telegram3.jpg,Telegram5.jpg,Telegram4.jpg,Telegram6.jpg,Telegram7.jpg,Telegram8.jpg'
metadata:
    Key(Telegram_home_assistant): 'Valor(domotizar,casa,google,home,assistant,telegram,bot,botfhader,mensaje,domotica)'
taxonomy:
    category:
        - docs
    tag:
        - domotizar
        - casa
        - google
        - home
        - assistant
        - telegram
        - bot
        - botfhader
        - mensaje
        - domotica
        - automatizar
sitemap:
    changefreq: hourly
    priority: 0.5
visible: true
---

![win10](image://os-compat.png)

[ui-tabs position="top-left" active="0" theme="lite"]
[ui-tab title="Descripción ..."]

> !!! _Cuándo nos proponemos tener una casa inteligente, nos damos cuenta que necesitamos estar informados de todos los cambios que pertenezcan a los dispositivos de la casa, si **se ha quedado la puerta de garaje abierta** al irnos, si **se  ha disparado la alarma cuando no estamos en casa** , o , si **se ha encendido el termostato por error**._

![](hate.png)
Todos **éstos cambios de estado se pueden automatizar con un mensaje** vía la Aplicación **_Telegram_**, un sistema de mensajería que, para aquellos que no lo conozcáis, es un estilo a _Whatsapp_, solo que, en mi opinión, es mucho mejor en todos los aspectos, entre ellos, con la existencia de los “bots”, es decir, robots con los que podemos interactuar y, en nuestro caso, **haremos que sea “la voz” de nuestra casa**. para ello necesitamos realizar unos pasos sencillos y podremos integrar éste servicio en nuestro sistema domótico. 


Si ya tenéis _Telegram_, podéis seguir **la guía de integración**, pero, para aquellos que no, os recomiendo que busquéis en vuestra tienda de aplicaciones, como _[Play Store](http://bit.ly/2VDrYay)_ o _[App Store](https://apple.co/30kq8u1)_, para descargarlo y ponerlo en marcha, al igual que se hace en _Whatsapp_. **Una vez que tengáis _Telegram_ en funcionamiento, podemos seguir para crear nuestro bot**, el cual, será el que nos informará y más adelante podrá recibir órdenes para poder hacer cosas en casa desde _Telegram_.

---

[/ui-tab]

[ui-tab title="Crear Bot..."]

**Como crear un bot de Telegram**:<br />
Buscamos el usuario BotFather, que es, el el usuario que generará el bot:<br />
![](Telegram1.jpg)
Ponemos /start y podemos empezar a ver la lista de comandos que necesitaremos, aunque, si queremos ver la lista completa, después de /start, podemos poner / y nos aparecerá la lista completa de los comandos que queremos:<br />
![](Telegram2.jpg)
Escribimos /newbot para que empecemos la creación:<br />
![](Telegram3.jpg)
Para el nombre, escribimos lo que queramos, ya que es el nombre mostrado, no el nombre de usuario, en mi caso he puesto Domótica:<br />
![](Telegram4.jpg)
Posteriormente nos pide el nombre de usuario, y, en este lugar si que Telegram obliga a que acabe en la palabtra “bot”, sea en mayúsculas o minúsculas, en mi caso he puesto Domotizarmicasa_bot:<br />
![](Telegram5.jpg)
Ya tenemos nuestro bot y, como veis, botfather nos da una clave (token) para poder hacer uso del bot por web. Si os gusta este tema, os recomiendo buscar información sobre los bots porque tienen mucho potencial.<br />
![](Telegram6.jpg)

**Obtener nuestro ID de chat para integrar nuestro bot en Home Assistant**<br />
Para poder integrar en nuestra instalación necesitamos tan solo un dato, nuestro ID de conversación para que nuestro bot sepa a quien hablar, para eso, buscamos al bot IDBot:<br />
![](Telegram7.jpg)
En el, pondremos /start y posteriormente el comando /getid y os contestará un número:<br />
![](Telegram8.jpg)
Con ese número apuntado, ya podemos configurar nuestro Home Assistant para comunicarse con nosotros desde Telegram:<br />
![](Telegram9.jpg)
Puedes ver la integración en la siguiente pestaña.<br />





[/ui-tab]
[ui-tab title="Integración..."]

**Para Integrarlo en Home Assitant**<br />
+ Vamos a usar la llamada `Telegram Polling` para poder mandar mensajes a nuestro usuario en Telegram. Para ello, abriremos el `configuration.yaml` y añadiremos lo siguiente:<br />

```text

telegram_bot:
  platform: polling
  api_key: 719825869:AAGA9CRytgCMkF3FGX0oPE_cDOdUAuxG9g0Q
  allowed_chat_ids:
    - 77685961    

```
+ Para crear el notificador, `configuration.yaml`:

```text

notify:
  - name: telegram
    platform: telegram
    chat_id: 77685961 

```
---

[/ui-tab]

[/ui-tabs]