
# CodeAlpha Docker Web Server

A simple Nginx web server running inside a Docker container, created as part of the CodeAlpha DevOps Internship.

## Technologies Used
- Docker
- Nginx
- HTML
- Ubuntu Linux

## Project Structure
- `Dockerfile` — Instructions to build the Docker image.
- `site/index.html` — Website content.
- `README.md` — Project documentation.

## Build the Docker Image

```bash
docker build -t codealpha-webserver:1.0 .
```

## Run the Container

```bash
docker run -d --name codealpha-web -p 8082:80 codealpha-webserver:1.0
```

## Test the Website

```bash
curl http://localhost:8082
```

## Check Container Health

```bash
docker inspect --format='{{.State.Health.Status}}' codealpha-web
```

## Learning Outcomes
- Built a Docker image.
- Deployed an Nginx web server in a container.
- Configured port mapping.
- Implemented a Docker health check.
- Tested the website and container status.
=======
# CodeAlpha_DockerWebServer
Dockerized Nginx web server with container lifecycle management, health checks and troubleshooting for the CodeAlpha DevOps Internship.
>>>>>>> ad55c4a0f0091735e0564a21e36e3a6b99ffff88
