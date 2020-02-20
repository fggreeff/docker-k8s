# node-visits

Example for building two docker containers. One containing a node express app which will count the number of times for a page visit and one container with Redis storing the count.

## Getting started

- cd `node-visits`
- Build and run image `docker-compose up --build`
- Visit [localhost](http://localhost:4001/)

## Tearing down

- Stop containers `docker-compose down`

### Useful commands

- Run docker containers as background process `docker-compose up -d`
- View running containers for the compose file `docker-compose ps`
- Exec into machine: `docker exec -it <docker_id> sh`

## Source

[Resource](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/)

