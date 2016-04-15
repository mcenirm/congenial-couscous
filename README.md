# Simple dockerized web service

From Kubernetes's [Hello World Walkthrough](http://kubernetes.io/docs/hellonode/)

## Run as node.js application

```Shell
$ node server.js
```

Try at http://localhost:8080/

## Run in docker

```Shell
$ docker build -t congenial-couscous:v1 .
$ docker run -d -p 8080:8080 congenial-couscous:v1
```

Try at http://$(docker-machine ip):8080/

# Elastic Beanstalk

```Shell
$ eb init
$ eb local run
```

Try at http://$(docker-machine ip):8080/
