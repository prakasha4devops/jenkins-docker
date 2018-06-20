# Jenkins Docker

[![Build Status](https://travis-ci.org/maxpou/docker-symfony.svg?branch=master)](https://travis-ci.org/maxpou/docker-symfony)

![alt text](https://wiki.jenkins.io/download/attachments/138449918/docker-jenkins.png?version=1&modificationDate=1518968278000&api=v2)



1. Create the folder 
create '/var/jenkins_home' folder on your machine

  ```bash
 $sudo mkdir -p /var/jenkins_home


 $sudo chown -R 1000:1000 /var/jenkins_home


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
