# Docker-project
PROJECT OBJECTIVE
------------------

Using the Drupal and PostgreSQL images from Docker Hub offers the following benefits:

1. The configuration of the software has been done for you, which means that you don’t need to follow a step-by-step 
   process for each application to get them running on your system.

2. Updating your software is as simple as downloading the latest images from Docker Hub.


3. Images and containers are self-contained, which means that they are easy to clean up if you decide to remove them.


STEP 1: Prior to running the docker services, you are required to disable the firewall
and SELinux using the following command:
      systemctl stop firewalld

STEP 2: Disabling the SELinux:
       setenforce 0

STEP 3: Start docker services:
systemctl start docker

STEP 4: Pull the latest version of postgresql docker image from hub.docker.com
docker pull postgres:latest

STEP 5 Pull the latest version of drupal docker image from hub.docker.com
docker pull drupal:latest

STEP 6: To see all docker images:
docker images

STEP 7: Create a directory named “mydrupal” in the root folder:
mkdir mydrupal

STEP 8: Create a file named “docker-compose.yml” inside the “mydrupal” directory.
cd mydrupal
vim docker-compose.yml

STEP 9: Enter the source code

STEP 10: Run the docker-compose file: docker-compose up

STEP 11: Inpect the drupal container using its container ID:
docker inspect [CONTAINER ID]

STEP 12: Get the IP address of drupal container.

STEP 13: Open the browser and browse with URL:
        172.19.0.3:80

STEP 14: Proceed with the Drupal installation steps and finish configuring the website.







