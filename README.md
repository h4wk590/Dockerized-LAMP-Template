# Dockerized php/httpd/sql

## This was created to aid an in-class lab

I created this to help other students utlize multiple environments for development during class.
It was utilized by the instructor and provided extra marks for other projects being able to 
'dockerize' applications/dev environments.


# configure the volumes in docker-compose.yml

you'll have to change the path to whatever your working directory path is after ```volumes:```.

Do ```docker-compose build``` to build the image.

you can use ```docker-compose up -d``` to run the container in the terminal background.

```docker ps -a``` to view active containers

The Apache image & php image both use their own dockerfiles.


```networks, frontend, and backend``` specify the containers to run together. This way I can refer to them using the container ids/names instead of digging around for ip addresses. Docker does this automagically.

