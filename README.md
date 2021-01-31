# Django & React Boilerplate with Docker

A dockerized starter boilerplate template for Django backend & React frontend.<br/>

<p><b>Stacks used:</b></p>

- Django 
- MySQL
- React (with webpack and hot reload)
- Nginx
- Docker


<p><b>Notes</b></p>

- This is a decoupled web application i.e Django Rest API <> React Client
- React app will be built and bundled into <b>/static</b> folder where <b>index.html </b> will be served via Nginx proxy
- For local environment, create your own .env file (see <b>.env.example</b> file in <b>/app</b> folder)


## Prerequisites

1. Docker
2. A cup of coffee :)


## Usage

In the project root folder (where docker-compose.yml file resides)

```bash
docker-compose up

```

```bash
#start development server - run this inside Docker container (/frontend)
npm run start
```

```bash
#build react application - run this inside Docker container (/frontend)
npm run build
```

Following ports are available upon a successful start

- <b>localhost:8000</b> : Django application
- <b>localhost:80</b> : React application (deployed)
- <b>localhost:3000</b> : React development server
