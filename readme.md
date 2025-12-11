## Run a Python application using mysql database using docker compose.


**Docker concepts used :**
* Docker Volumes
* Docker Network
* Environment Variables


**How to run this project ?** \
`cd /pythonapp` \
`docker-compose up -d`

**Check if flask-app container is able to connect to mysql-container** \
`docker exec -it flaskapp mysql -h mysql-container -u admin -p`

**Cleanup the container from compose file** \
`docker compose down`  _#!Removes docker containers, networks from compose file_

![dockercomposedownall](./dc.png)

`docker compose down --rmi all -v`  _#!Removes docker images, networks, volumes from compose file_

![dockercomposedownall](./dc-down-all.png)