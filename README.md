# Pyramid Compose  - WIP README

Microservices architecture composed of Docker + Pyramid + Caddy.

- [Pyramid](http://docs.pylonsproject.org/en/latest/docs/pyramid.html) as backend (service)
- [Caddy](http://caddyserver.com/docs/caddyfile) to use with frontend what you want (Angular.js, Ember.js, React)


### Install

```
git clone https://github.com/marioidival/pyramid_compose.git name_of_you_project
cd name_of_you_project
docker-compose up
```
```
$DOCKER_MACHINE_IP:3333 - backend
$DOCKER_MACHINE_IP:3334 - frontend
```
