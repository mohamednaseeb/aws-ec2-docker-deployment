# Dockerfile and Custom Image Creation

## Overview

A custom Docker image was created using Nginx as the base image and a custom web page was deployed inside the container.

---

## Project Structure

```text
aws-docker-deployment/
├── Dockerfile
├── index.html
└── docs/
```

---

## Dockerfile

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80
```

---

## Build Custom Image

```bash
sudo docker build -t aws-portfolio .
```

---

## Verify Image Creation

```bash
sudo docker images
```

Example output:

```text
REPOSITORY      TAG       IMAGE ID
aws-portfolio   latest    xxxxxxxxxxxx
```

---

## Image Components

### Base Image

```text
nginx:latest
```

Provides:

- Web server
- HTTP service
- Static content hosting

### Custom Content

```text
index.html
```

Copied into:

```text
/usr/share/nginx/html/
```

---

## Result

A custom Docker image named **aws-portfolio** was successfully created and prepared for deployment.

---

## Skills Demonstrated

- Dockerfile creation
- Docker image building
- Nginx configuration
- Containerized web hosting
- Docker image management
