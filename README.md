# Django deployment by Docker

This project use docker to deploy simple django project on Ubuntu
This project use three docker-compose to acheive deployment
* Nginx reverse proxy with HTTPS support by following two project
  1. jwilder/nginx-proxy
  2. JrCs/docker-letsencrypt-nginx-proxy-companion
* PostgreSQL from Docker Hub
* django_project which contains nginx from Docker Hub and a simple Django project 

## Getting Started

1. Install docker and docker-compose(the version of docker-compose should >= 1.18) on your machine
2. Clone this project
3. Copy your django project folder into django_project/
4. Setup config.sh

## Built With

* [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy) - Nginx reverse proxy by Docker
* [JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) - Let's encrypt companion container for nginx-proxy
* [Python](https://hub.docker.com/_/python) - Python 3.6 on Docker Hub
* [Nginx](https://hub.docker.com/_/nginx) - Nginx on Docker Hub
* [PostgreSQL](https://hub.docker.com/_/postgres) - PostgreSQL on Docker Hub

## Versioning

* v0.0.1

## Authors

* **AlenShiun** - *Initial work*

## License

## Acknowledgments

* Inspiration by following projects
  * [twtrubiks/docker-django-nginx-uwsgi-postgres-tutorial](https://github.com/twtrubiks/docker-django-nginx-uwsgi-postgres-tutorial/blob/master/README.en.md)
