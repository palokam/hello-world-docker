# docker-hello-predix

Sample docker to test out Docker on Predix.io

Docker says "Hello" to Predix.io

```shell
# clone this repository
$ git clone https://github.com/indaco/docker-hello-predix

cd docker-hello-predix

# build an image using Dockerfile
docker build -t hello-predix .

# create and test a container locally
docker run --name mypredixhello -p 8080:80 hello-predix

# open a browser window at http://localhost:8080

# push to predix cloud
cf push your-app-name --docker-image indaco/docker-hello-predix:latest -m 64M
```
