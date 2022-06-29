# Jenkins-JCasC
Automate the installation and configuration of Jenkins using Docker and the Jenkins Configuration as Code (JCasC) method.

## Installation

JCasC will require docker and docker-compose installed on the host machine.

**Default login will be "admin" and password will be "jenkins". You can change it in docker-compose.yml**

**Jenkins default URL will be [http://localhost:9898](http://localhost:9898/) and can be replaced in casc.yml**

```sh
docker build -t jenkins:jcasc .
mkdir -p jenkins_data
chown 1000:1000 jenkins_data
docker-compose up -d
docker ps -a
```
Browse [http://localhost:9898](http://localhost:9898/) OR URL you mentioned in casc.yml
