docker run -d --name nginx-container nginx
docker run -d --name postgres-container postgres
docker run -d --name redis-container redis

docker stop nginx-container
docker stop postgres-container

docker ps

docker stop redis-container

docker containers purge
docker images purge
