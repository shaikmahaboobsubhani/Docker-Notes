## Manual setup
* install java * apache maen
 refered [here] ``` sudo apt-get update && sudo apt-get install openjdk-8-jdk```
# install maven

* ``` apt-get install maven -y ```
# installin git
``` apt-get install git -y ```
 
* ``` Refered [here] git pull https://github.com/spring-projects/spring-petclinic.git ```
# Build the package / creating jar file
 * ``` mvn clean package ```
 # deploy a jar /project 
 * ``` java -jar spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar ```

 # accessing project
 * localhost/ip:8080