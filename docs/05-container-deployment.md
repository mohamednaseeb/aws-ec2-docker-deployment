# Docker Container Deployment

## Overview

The custom Docker image was deployed as a running container on an AWS EC2 instance.

---

## Run the Container

```bash
sudo docker run -d -p 80:80 --name portfolio aws-portfolio
```

### Explanation

| Option | Description |
|----------|-------------|
| -d | Run container in detached mode |
| -p 80:80 | Map host port 80 to container port 80 |
| --name portfolio | Assign container name |
| aws-portfolio | Docker image name |

---

## Verify Running Container

```bash
sudo docker ps
```

Example output:

```text
CONTAINER ID   IMAGE          STATUS
xxxxxxxxxxxx   aws-portfolio  Up
```

---

## Port Mapping

```text
Host Port      Container Port
80             80
```

This allows users to access the application using the EC2 public IP address.

Example:

```text
http://3.xx.xx.xx
```

---

## Container Status Check

```bash
sudo docker ps
```

---

## Stop Container

```bash
sudo docker stop portfolio
```

---

## Start Container

```bash
sudo docker start portfolio
```

---

## Remove Container

```bash
sudo docker rm -f portfolio
```

---

## Result

The container was successfully deployed and made accessible over the internet through the AWS EC2 public IP address.

---

## Skills Demonstrated

- Docker container deployment
- Port mapping
- Nginx container hosting
- Linux server management
- AWS EC2 application deployment
- Container lifecycle management
