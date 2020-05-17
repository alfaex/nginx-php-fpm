# NGINX PHP-FPM

Example on how to separeta nginx from php.

The aim of this is to complitly remove the necessity to put php files on the nginx server.

Allowing to have each docker container in a separeted server

Example:
```
                / SERVER1 running 5 containers
NGINX SERVER    - SERVER2 running 3 containers
                \ SERVER3 running 5 containers
```

Docker compose with scale config for reference

`$ docker-compose up -d --scale php=3`

PS: this repo is a personal reminder of how to setup this php-fmp configuation.