## Dockerized multiple services

React application for getting the fibonacci number for a given index. The application itself is not of value here. The aim is to have mutiple docker services (server, client, worker) running and ensuring we bring the building time of the 3 containers to a minimum. 

Aside from our 3 services, we also make use of a Postgres and Redis DB. Along with nginx as our proxy. 

## Arthitecture

![arthitecture](./sources/arthitecture.png)

## Getting started

Bring up Redis, Postgres and our server, client and worker with:
> docker-compose up

> [localhost:3050](http://localhost:3050/)

Starting the containers separately:
#### Client
> cd client

> docker build -f Dockerfile.dev .

> docker run <containerId>

#### Server
> cd server

> docker build -f Dockerfile.dev .

> docker run <containerId>

#### Worker
> cd worker

> docker build -f Dockerfile.dev .

> docker run <containerId>

#### Nginx
> cd nginx

> docker build -f Dockerfile.dev .

> docker run <containerId>

## Source

[Resource](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/)