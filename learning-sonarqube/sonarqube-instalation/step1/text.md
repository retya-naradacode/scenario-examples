
Install Sonarqube Via Docker

<br>

### Solution
Install sonarqube using docker

```plain
docker run -d --name sonarqube -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube:latest
```{{exec}}

Wait until Sonarqube is Up and Running

```plain
while [[ "$(curl -s -o /dev/null -w ''%{http_code}'' localhost:9000)" != "200" ]]; do sleep 5; done
```{{exec}}

Once your instance is up and running, Log in Sonarqube dashboard by Traffic Port Accessor. Click burger button on the top left of terminal and choose Traffic Port Accessor. Fill Custom Ports using Sonarqube default port : 9000

```plain
System Administrator credentials:

login: admin
password: admin

```{{exec}}

Change Default Password of Sonarqube


