# node - container
#### EXAMPLE
```sh
touch Dockerfile
vim Dockerfile
vim app.js
docker build -t apirath/node8:v8.12-test .
docker images
docker run --name node8.12-test apirath/node8:v8.12-test
docker ps -a
docker rm <container-id>
docker run -d -p 8088:80 --name node8.12-test apirath/node8:v8.12-test
docker ps
docker logs -f <container-id>
curl localhost:8088
docker stop <container-id>
docker run -d --rm -p 8089:80 apirath/node8:v8.12-test
docker stats
curl localhost:8089
docker tag apirath/node8:v8.12-test apirath/node8:latest
docker push apirath/node8:latest
docker ps -aq
docker stop $(docker ps -aq)
docker rm $(docker ps -aq)
docker rmi $(docker images -aq)
```
