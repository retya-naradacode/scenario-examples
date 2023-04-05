
Install Sonarqube Via Docker

SonarQube is a Code Quality Assurance tool that collects and analyzes source code, and provides reports for the code quality of your project.

<br>

### Solution
Install sonarqube using docker

```plain
docker run -d --name sonarqube -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube:latest
```{{exec}}

Check Sonarqube is already Up 

```plain
while [[ "$(curl -s -o /dev/null -w ''%{http_code}'' localhost:9000)" != "200" ]]; do sleep 5; done; echo "UP & Running"
```{{exec}}

Wait until Script above produce output "Up and Running"

```plain
Up & Running
```{{exec}}

Once your Sonarqube is up and running, Login to Sonarqube dashboard by Traffic Port Accessor. Click burger button on the top right of terminal and choose Traffic Port Accessor. Fill Custom Ports using Sonarqube default port 9000. Please use credential below to Login Sonarqube

```plain
System Administrator credentials:

login: admin
password: admin

```{{exec}}

Change Default Password of Sonarqube. And now you are done to setup Sonarqube


