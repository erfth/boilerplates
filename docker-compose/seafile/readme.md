## Install docker-compose
Seafile v7.x.x (or newer versions) image uses docker-compose. You should install the docker-compose command.

for CentOS
```
yum install docker-compose -y
```
for Ubuntu
```
apt-get install docker-compose -y
````
## Download and modify docker-compose.yml
Download docker-compose.yml sample file to your host. Then modify the file according to your environment. The following fields are needed to be modified:

*The password of MySQL root (MYSQL_ROOT_PASSWORD and DB_ROOT_PASSWD)
*The volume directory of MySQL data (volumes)
*The volume directory of Seafile data (volumes).

## Start Seafile server
Start Seafile server with the following command
```
docker-compose up -d
```

Wait for a few minutes for the first time initialization, then visit http://seafile.example.com to open Seafile Web UI.

NOTE: You should run the above command in a directory with the docker-compose.yml.

## More configuration options

Please visit [https://manual.seafile.com](https://manual.seafile.com) to get deep and detailed explanation for all configuration.

