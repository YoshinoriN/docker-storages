# Usaga

```sh
docker build -t maria:storage -f Dockerfile .
docker create --name maria-storage maria:storage
docker run --volumes-from maria-storage -e MYSQL_ROOT_PASSWORD=mypass -p 4306:3306 -d mariadb:latest
```
