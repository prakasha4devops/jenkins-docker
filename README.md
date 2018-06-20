# Jenkins docker

1. Create the folder 
create '/var/jenkins_home' folder on your machine with 777 permsiosn

  ```bash
 $sudo mkdir -p /var/jenkins_home

 $sudo chmod 777 /var/jenkins_home

  ```

2. Build/run containers with (with and without detached mode)

    ```bash
    $ docker-compose build
    $ docker-compose up -d
    $ docker-compose up -d --build

    ```
3.  ## Useful commands

    ```bash

#To see running docker
$ docker-compose ps

# To check logs 
$ docker-compose logs -f


# Delete all containers
$ docker rm -f $(docker ps -aq)

# Delete all images
$ docker rmi $(docker images -q)

# Restarting all running docker containers
$ docker restart $(docker ps -aq)

# docker restart
$ docker-compose restart

 ```
