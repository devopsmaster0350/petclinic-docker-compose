## spring petclinic using Docker compose
* Commands we need to use is to
* for build the docker image
```
   docker compose -p petclinic build
```
* to up the docker compose service
```
   docker compose -p petclinic up -d
```
* to connect the application to postgres we need to change the connection string name in file `src/main/resources/application-postgres.properties` according to you postgres container name or ip followed by port name.
```
  petclinic-postgres-1:5432 or 172.18.0.2:5432
```
*Note this peoject will work only if you set the -p (project name) to petclinic otherwise , container name will get changed we need to modify the connection string according to it, then only application will work. 

