# Django deployment by Docker

This project use docker to deploy simple django project on Ubuntu
This project use three docker-compose to acheive deployment
* Nginx reverse proxy with HTTPS support by following two project
  1. jwilder/nginx-proxy
  2. JrCs/docker-letsencrypt-nginx-proxy-companion
* PostgreSQL from Docker Hub
* django_project which contains nginx from Docker Hub and a simple Django project 

## Getting Started

1. Install docker and docker-compose( >= 1.18) on your machine
2. Clone this project
3. Copy your django project folder into django_project/
4. Setup config.sh
    * Keep LETS_ENCRYPT_TEST_RUN=1 to get stage certification for testing your domain or set LETS_ENCRYPT_TEST_RUN=0 to request real certification from Let's encrypt
    * DJANGO_PROJECT_NAME: Project name of Django
    * HOST_NAME: Your domain name
    * MAINTAINER: Your email
5. Run init_all.sh
6. Run run_all.sh
7. Open your browser and go to web site with HOST_NAME

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

