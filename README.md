
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

## Docker Container Management

### Check running containers
```bash
docker ps
```

### View all containers
```bash
docker ps -a
```

### Stop the web server
```bash
docker stop codealpha-web
```

### Start the web server
```bash
docker start codealpha-web
```

### View container logs
```bash
docker logs codealpha-web
```

### Check container health
```bash
docker inspect --format='{{.State.Health.Status}}' codealpha-web
```

### Test the web server
```bash
curl http://localhost:8082
```

## Key Learnings

- Built a web server Docker image using Nginx Alpine.
- Ran a container with Docker port mapping.
- Configured a Docker health check.
- Practised container lifecycle and troubleshooting commands.
