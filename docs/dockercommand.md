$ docker images (show all image)
$ docker build -t nginx_image .
$ docker search <image> (search images in dockerhub(official or non official images))
$ docker ps -a (show all active container)
$ docker run hello world ()
$ docker exec -it 00e72  sh -c "/entrypoint.sh bash"  (enter inside container with entrypoint)
$ docker system prune (Delete all unused containers, unused networks, and dangling images.)
$ docker container kill $(docker ps -q) (kill all running container)
$ docker container rm $(docker ps -a -q) Delete all containers that are not running.
$ docker image history my_image (Display an image’s intermediate images with sizes and how they were created)
$ docker system prune -a --volumes ( Remove unused volumes. We’ll talk more about volumes in the next article.)
$ docker ps -aq (List all containers (only IDs) 
$ docker stop $(docker ps -aq) (Stop all running containers)
$ docker rm $(docker ps -aq) (Remove all containers)
$ docker info # gives running container,images,engine information
$ docker rmi $(docker images -q) (Remove all images)
$  docker network create --driver =bridge folderone (create own network )
$ docker volume inspect volume_name
$ docker  network inspect volume_name
Network:- 
1. Bridge :- docker run image_name (IP series comes 172.17.0.3,172.17.0.2)
2. none :- docker run image_name -network=none
3. host:- docker run image_name  -network=host
docker network ls // check container connect network  
