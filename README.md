# docker_stacks

Esta es mi configuración para mi servidor local con Linux usando Docker. Una vez instalado Docker y funcionando, la idea es usar Portainer para ir añadiendo las aplicaciones que me interesan.

- Crear un directorio donde se montarán todos los volúmenes de las diferentes aplicaciones (p.ej. /docker_data/)
- Crear los directorios de cada aplicación, según su fichero .env y revisar posibles problemas de permisos (si no se usa docker como root).
- Descargar el directorio de Portainer al servidor (/home/usuario/portainer o similar).
- Entrar en el directorio, ajustar el .env con la ruta del directorio correcta (/docker_data/Portainer).
- Ejecutar: docker up -d
- Acceder a portainer en la ruta http://xxx.xxx.xxx.xxx:9000 siendo las xxx la IP del servidor.
- Añadir el resto de las aplicaciones como 'Custom Templates' para gestionarlo desde Portainer.