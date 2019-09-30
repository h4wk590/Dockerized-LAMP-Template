# Dockerized php/httpd/sql


# configure the volumes in docker-compose.yml

you'll have to change the path to whatever your working directory path is after ```volumes:```.

Do ```docker-compose build``` to build the image.

you can use ```docker-compose up -d``` to run the container in the terminal background.

```docker ps -a``` to view active containers

The Apache image & php image both use their own dockerfiles.

## The apache.conf serves the content to port 80, but this can be changed to any port very easily to avoid conflicts with the host port 80. 

Using the Alpine-Linux images was faster than any other for some reason.

```networks, frontend, and backend``` specify the containers to run together. This way I can refer to them using the container ids/names instead of digging around for ip addresses. Docker does this automagically.

Haven't tested the mysql.