
# Docker con app sencilla de Node.js 

Este repositorio contiene una aplicación Docker con app sencilla de Node.js que lista y persiste un conjunto de tareas

# 1 Overview 2Containerize 3 Update 

- Clonamos este repositorio.
- Ejecutamos `docker build -t mi-aplicacion .`. Esto hace se construya la app
(imgs\2 starting 2.JPG)
- Ejecutamos `docker run -p 3000:3000 mi-aplicacion`. Esto hace que se despliegue la app por el puerto que configuramos en el archivo Dcokerfile
- Accedemos a `http://localhost:3000`, donde se indexará la página principal.

![start](imgs/2%20starting%202.JPG)

# 4 Share the application

- Desde la cuenta de Dockerhub creamos el tag para luego acceder desde CMD más el inicio de sesión de Docker para acceder a la imagen pública del Docker

![start](imgs/4%20docker_view.JPG)
![hola](imgs/5%20docker%20tag.JPG)

- Se realiza push al repo creado
![text](imgs/6%20docker%20push.JPG)
![](imgs/7%20docker%20alpine.JPG)
# 5 Persists
- Crear el volumen
![](imgs/8%20dokcer%20rm.JPG)
![](imgs/9%20creacion%20docker%20con%20volume.JPG)
- Se crea un nuevo contenedor montando el volumen creado
![](imgs/9%20nuevo%20docker.JPG)
- Se verifica que los datos persisten a partir del volumen 
![](imgs/10%20docker%20persist.JPG)
- Profundizando en la información relacionada al volumen
![](imgs/11%20docker%20volume.JPG)


# 6: Use bind mounts

- Se crea un archivo .txt en el lado del contenedor Docker, y se comprueba que se agrega en el sistema de archivos

![](imgs/13%20mount%20data.JPG)
- Se borra el archivo .txt en el lado del contenedor Docker, y se comprueba que se borra en el sistema de archivos
![](imgs/14%20mount%20data.JPG)
- Se despliega la versión que permite al contenedor actualizarse localmente
![](imgs/15%20mount%20development.JPG)
- Se cambia la info al botón a Add, reflejando los cambios automáticamente
![](imgs/16%20mount%20dev%20cambios.JPG)
![](imgs/17%20localhsot.JPG)


# 7 Multi-container apps
- Se inicia un contenedor dedicado a la base de datos
![](imgs/18%20network%20y%20docker%20sql%20image.JPG)
- Accediendo a la base de datos dentro del contenedor, sin datos aun
![](imgs/19%20slq%20conn.JPG)
![](imgs/20%20mysql.JPG)
- Comprobando la persistencia
![](imgs/21%20mysql.JPG)
![](imgs/22%20mysql.JPG)

# 8 Docker composer
- compose.yaml
![](imgs/23%20docker%20compose.JPG)
- Levantar la orquestación de servicios
![](imgs/24%20correr%20docker%20compose.JPG)
- Localhost
![](imgs/17%20localhsot.JPG)


