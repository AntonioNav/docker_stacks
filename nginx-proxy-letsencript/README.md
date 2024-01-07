Nginx Proxy + Let's encrypt

Referencias: 
    <https://gist.github.com/saniaky/dc75cbf64922e418400b0f54ed5b2c3a>
    <https://github.com/nginx-proxy/nginx-proxy>
    <https://github.com/nginx-proxy/acme-companion>

Básicamente se encarga de redireccionar los subdominios a los contenedores que los definen en sus variables de entorno (ver el composer de HomeAssistant). A la vez, con el complemento, genera y renueva los certificados de Let's Encrypt.

En este caso la red está forzada a ser la del Host (por HomeAssistant, aunque quizá no fuese ni necesario). En otros ámbitos, solo es necesario que los contenedores sean accesibles entre ellos por una misma red.