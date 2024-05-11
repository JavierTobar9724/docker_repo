
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
![](imgs/7%20docker%20alpine.JPG)
![](imgs/8%20dokcer%20rm.JPG)
![](imgs/9%20creacion%20docker%20con%20volume.JPG)
![](imgs/9%20nuevo%20docker.JPG)
![](imgs/10%20docker%20persist.JPG)
![](imgs/11%20docker%20volume.JPG)







# 6: Use bind mounts
![](imgs/12%20mount.JPG)
![](imgs/13%20mount%20data.JPG)
![](imgs/14%20mount%20data.JPG)
![](imgs/15%20mount%20development.JPG)
![](imgs/16%20mount%20dev%20cambios.JPG)
![](imgs/17%20localhsot.JPG)


# 7 Multi-container apps
![](imgs/18%20network%20y%20docker%20sql%20image.JPG)
![](imgs/19%20slq%20conn.JPG)
![](imgs/20%20mysql.JPG)
![](imgs/21%20mysql.JPG)
![](imgs/22%20mysql.JPG)

# 8 Docker composer
![](imgs/23%20docker%20compose.JPG)
![](imgs/24%20correr%20docker%20compose.JPG)
![](imgs/17%20localhsot.JPG)


