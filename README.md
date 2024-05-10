
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
![text](imgs/6%20docker%20push.JPG)
# 5 Persists


