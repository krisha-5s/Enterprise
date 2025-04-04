Spring Microservice on Docker
=====================

Author: HBF
Date: 2024-09-30


### docker commands on Linux

sudo docker build -t spring-boot .

sudo docker image ls

sudo docker run -d -p 8081:8080 --name spring-boot-ms -t spring-boot

Note that the -d option is to run the container in backgroud

sudo docker container ls

curl http://localhost:8081/json/ec

curl http://localhost:8081/xml/ec

sudo docker container stop spring-boot-ms

sudo docker container rm spring-boot-ms

sudo docker save spring-boot > spring_boot.tar

This command saves the spring-boot image to local file spring_boot.tar, which can be deployed and loaded in a self-managed style. 

sudo docker image rmi spring-boot

This command removes spring-boot image from the repo. 

sudo docker image ls

sudo docker load < spring_boot.tar

This command loads the saved image from file spring_boot.tar

sudo docker run -p 8081:8080 --name spring-boot-ms -t spring-boot

This run the spring-boot-ms container in front. Open a new command line terminal, test it by the following command

curl http://localhost:8081/json/ec

sudo docker container stop spring-boot-ms

sudo docker container rm spring-boot-ms

sudo docker image rmi spring-boot




