# node-web

Example for building node express app in docker

## Getting started

- cd `node-web-image`
- Build image with tag `docker build -t <docker_id>/node-web .`
- Map inbound port from local (3000) to docker (8080) `docker run -p 3000:8080 <docker_id>/node-web`
- Visit [localhost](http://localhost:3000/)

### Useful schortcuts

- Use `ctrl`+`d` to exit container
- Use `ctrl`+`c` to stop container
- Exec into machine: `docker exec -it <docker_id> sh`

## Source

[Resource](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/)

