# drf-react

drf-react is a project created to learn how to build applications using Django REST Framework and React.

drf-react uses [Django REST Framework ](https://www.django-rest-framework.org/) to construct an API and [django-cors-headers](https://pypi.org/project/django-cors-headers/) to add Cross-Origin Resource Sharing (CORS) headers to responses in order to allow React to make requests.

The project is currently a TODO list in which list items can be added, deleted, updated, etc. through HTTP requests.

A Dockerfile is included for both backend and frontend services and a docker-compose.yml file is included to allow for development using a Docker container.


## Setting Up the Dev Environment

Ensure that [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/install/) is installed. This will also install [Docker Compose](https://docs.docker.com/compose/), which is used for defining and running Docker apps using the Dockerfile and docker-compose.yml files.

After cloning this repository;
```bash
git clone https://github.com/djknox/drf-react.git
```

Build the image and run the container with Docker Compose:
```bash
docker-compose up --build
```
This will set up:  
* a PostgreSQL database at port 5432  
* serve the Django API at port 8000  
* serve the React frontend at port 3000

The container can be stopped and removed with:
```bash
docker-compose down
```