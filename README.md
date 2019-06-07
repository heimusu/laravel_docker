# Sample for Laravel with Docker
## Requirement
- Docker
- Docker-Compose

## Prepare for development
+ `$ docker-compose up -d`
+ `$ docker-compose exec php bash`
+ `$ laravel new`
+ Access `http://localhost:80`

## Tips
If you show the error about `docker: Error response from daemon: driver failed programming external connectivity on endpoint xxx (xxx):x Error starting userland proxy: Bind for 0.0.0.0:80: unexpected error (Failure EADDRINUSE).`
 , stop the service that using `80` port like this.
 
```
sudo lsof -i -P | grep "LISTEN"
sudo apachectl stop
```
