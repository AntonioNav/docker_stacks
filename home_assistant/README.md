Home-Assistant, junto con Mosquitto, Node-Red y Zigbee2MQTT

<https://www.home-assistant.io/installation/linux#install-home-assistant-container>

<https://hub.docker.com/_/eclipse-mosquitto#>!

<https://nodered.org/docs/getting-started/docker>

<https://www.zigbee2mqtt.io/guide/getting-started/#installation>

Ejecuta Home Assistant, con acceso a la red del host directamente. Ajustar la ruta del directorio de configuración.
Las variables de entorno son para el proxy-inverso con nginx+letsencrypt, para que redireccione el sub-dominio y genere los certificados SSL

Node-Red y ZigBee2mqtt se pueden quitar si no se usan. Mosquitto, posiblemente sea mejor dejarlo ya que muchos elementos domóticos pueden usar MQTT directamente. Ajustar las rutas de los directorios de configuración.

Para ZigBee2mqtt, hay que ajustar también el dispositivo a utilizar (/dev/XXXXXX)