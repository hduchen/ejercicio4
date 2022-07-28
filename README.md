# Pasos 

* Bajar Jar

* Generar Docker File

* Compilamos la imagen 
```
$  docker build -f .\Dockerfile.v3 --no-cache  -t hduchen/passwordapi:2.0.0 . 
```
* validamos la imagen 
```
$ docker image ls
```
* Exponemos el puerto y visualizmos en localhost
```
$ docker run --name eje4 -p 3000:8080 hduchen/passwordapi:2.0.0
```
* Subimos la imagen a dockerhub
```
$ docker push hduchen/passwordapi:2.0.0    
```
https://hub.docker.com/repository/docker/hduchen/passwordapi
