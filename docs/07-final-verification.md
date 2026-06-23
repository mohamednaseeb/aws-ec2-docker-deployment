# Final Verification and Project Results

## Overview

After deployment, all components were verified to ensure successful operation.

---

## Docker Verification

Check running containers:

```bash
sudo docker ps
```

Expected Result:

```text
aws-portfolio   Up
```

---

## Docker Image Verification

```bash
sudo docker images
```

Expected Result:

```text
aws-portfolio:latest
```

---

## Web Application Verification

Application URL:

```text
http://<EC2-PUBLIC-IP>
```

Expected Output:

```text
AWS EC2 Docker Deployment

Successfully deployed on AWS EC2 using Docker.

Project by Mohamed Naseeb.
```

---

## Infrastructure Verification

Verified Components:

- AWS EC2 Instance
- Ubuntu Linux Server
- Docker Engine
- Custom Docker Image
- Running Container
- Nginx Web Server
- Security Group Rules
- Public Internet Access

---

## Commands Used

Verify container:

```bash
sudo docker ps
```

Verify image:

```bash
sudo docker images
```

Verify service access:

```bash
curl http://localhost
```

---

## Project Architecture

```text
AWS EC2
    |
Ubuntu Server
    |
Docker Engine
    |
Docker Container
    |
Nginx
    |
Custom Web Application
```

---

## Project Outcome

Successfully deployed a containerized web application on AWS EC2 using Docker and Nginx.

The application was made publicly accessible through an AWS Security Group and validated through browser testing.

---

## Technologies Used

- AWS EC2
- Ubuntu Linux
- Docker
- Dockerfile
- Nginx
- SSH
- Git
- GitHub

---

## Key Learnings

- AWS EC2 provisioning
- Linux server administration
- Docker image creation
- Container deployment
- Nginx web hosting
- AWS networking and security
- Infrastructure troubleshooting
- Cloud deployment workflows

---

## Resume Highlights

- Provisioned and configured Ubuntu EC2 instances on AWS.
- Installed and managed Docker containers on Linux servers.
- Built custom Docker images using Dockerfile and Nginx.
- Configured AWS Security Groups and networking for public web access.
- Deployed containerized web applications accessible through public IP addresses.
- Managed Linux servers remotely using SSH and command-line tools.
