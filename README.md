# Should be working out of box.

Use 

```

docker-compose build 

```
to build the image.

you can you ```docker-compose up -d``` to run the container in the terminal background.

```docker-compose ps -a``` to view images

```docker-compose -it < container id > bash``` to go into the container.

the php & apache images have their own dockerfiles. 