Composer file and its commands


command to creat an image 

in the directory where dockerfile exist open terminal and write command

> docker build -t image_name .

run the container from and image 

> docker run -phost port:project port --containername imagename -d is used to run container in detached mode 

stop a container 

>docker stop container name or id

delete container 

>docker rm image name or id 

delete image

>docker rmi image name or idtouch path/to/your/file.md


inspect docker container 

>docker inspet container name opr id 

view logs 

>docker logs container name or id 

list docker running containers 

>docker ps  or -a with this command shows all available containers in running or stope status

docker networks and volume 

to creat a docker volume use 


>docker volume creat vloume name

delete the volume 

>docker rm vloume name or id

list all the volumes 

>docker volume ls



