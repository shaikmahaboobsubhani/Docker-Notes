## Pull the image from Docker hub in Docker file
* FROM ubuntu:18.04
## Information about project/developer
LABEL Author=subhani
LABEL Org=TECHMAHINDRA
# installing java
``` sudo apt-get update && apt-get install openjdk-8-jdk ```

FROM ubuntu:18.04
LABEL Author=subhani
LABEL org=Mahinda
RUN apt-get update && apt-get install openjdk-8-jdk -y
ADD https://s3-ap-southeast-1.amazonaws.com/dev.k8s.subhanidevops.tk/org.springframework.petclinic.repository.eclipselink-2.1.0.release.jar  /spring-petclinic.jar
EXPOSE 8080
CMD ["java", "-jar", "/spring-petclinic.jar" ]

~

# Run a Docker file / creting a containers & images
 * ``` docker build -t spc:ubuntu . ```
 # creating a contaner using image
 ``` docker container run --name myapp -p 8081:8080 -d spc:ubuntu ```
 # Check running containers in Docker 
 * ``` docker ps ```