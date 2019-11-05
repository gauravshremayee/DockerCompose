version: '2'
services:
        databases:
                image: mysql
                ports: 
                - "3306:3306"
                environment:
                        - MYSQL_ROOT_PASSWORD=andaman
                        - MYSQL_USER=user
                        - MYSQL_PASSWORD=andaman
                        - MYSQL_DATABASE=demodb

        web: 
          image: nginx



$docker-compose up -d 

$docker run --name=testsql -e MYSQL_ROOT_PASSWORD=******* -d mysql 



Step 1: Pull phpMyAdmin image from docker hub
docker pull phpmyadmin/phpmyadmin
Step 2: To link our existing MySQL container with phpMyAdmin application use the following.
docker run --name myadmin -d --link testsql:db -p 8080:80 phpmyadmin/phpmyadmin 


# DockerCompose
# Composing Docker 
$ docker-compose up -d

$ ./run_tests

$ docker-compose down

$docker images

REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
dockerubuntu_web    latest              e3c2e63d1cca        38 seconds ago      251MB


$ docker-compose up -d
Creating network "dockercompose_default" with the default driver
Creating volume "dockercompose_logvolume01" with default driver
