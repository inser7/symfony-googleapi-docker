## Installation

Just follow next instructions:

```
git clone https://github.com/inser7/symfony-googleapi-docker.git
cd symfony-googleapi-docker
```

Docker setup:**

Both [Docker](https://docs.docker.com/install/)
and [Docker Compose](https://docs.docker.com/compose/install/) are need to be installed.

Verbose mode:

`docker-compose up`

Detached state:

`docker-compose up -d`

Shutdown:

`docker-compose down`

## Run application

Point your browser at [http://localhost:8080/api/getbooks?q=ff&page=1](http://localhost:8080/api/getbooks?q=ff&page=1) to get json