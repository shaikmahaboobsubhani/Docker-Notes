# Installation Visual studio code
 * chocolatey : Refered [here]: (https://chocolatey.org/)
# for Linux 
 * Linux: Refered [here] : (https://code.visualstudio.com/docs/setup/linux)
 
 * windows : Refered [here]: (https://code.visualstudio.com/docs/setup/windows)

 * Macos : Refered [here] : (https://code.visualstudio.com/docs/setup/mac)

## Senario:
* I need tomcat8
* Approach: in vm's
* login to the linux machine
    *Execute a commad: ```sudo apt-get update && sudo apt-get install tomcat8 -y ```
## crate Docker Containers
# Approach:Docker play ground
*let us use Docker playground .. Refered [here] (https://labs.play-with-docker.com/) -> start
* Media:Refered [here] (hub.docker.com)
*  create docker hub id & then start

    docker run -p 8080:8080 -d tomcat:8
    docker run -p 8081:8080 -d tomcat:9
    docker run -p 8082:8080 -d tomcat:9
## Dockr RUN - to create a new container
    Docker Daemon,Docker Client
* Docker client forwords run request with image name to docker Daemon
* Docker Daemon checks for image in local images
* if it is not found it tries to download from registry:(Dockerhub.com)

# Importance 
* we must know how to create docker images for the applications which your team is building

# How to create images ?
* Standard Approach: create images by writing Dockerfile

* clone Approach: create container and then copy image