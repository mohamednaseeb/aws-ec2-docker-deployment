# AWS Networking and Security Configuration

## Overview

To make the Dockerized web application publicly accessible, AWS networking and security configurations were implemented.

---

## EC2 Instance Details

| Resource | Configuration |
|-----------|---------------|
| Cloud Provider | AWS |
| Service | EC2 |
| Operating System | Ubuntu Server 24.04 LTS |
| Instance Type | t3.micro |
| Region | us-east-1 |

---

## Security Group Configuration

A custom security group was created and attached to the EC2 instance.

### Inbound Rules

| Port | Protocol | Source | Purpose |
|--------|----------|----------|----------|
| 22 | TCP | My IP | SSH Access |
| 80 | TCP | 0.0.0.0/0 | HTTP Traffic |
| 443 | TCP | 0.0.0.0/0 | HTTPS Traffic |

---

## SSH Remote Access

The EC2 instance was managed remotely using SSH authentication.

### Example

```bash
ssh -i aws-devops-key.pem ubuntu@<PUBLIC-IP>
```

---

## Public Web Access

The Docker container was exposed using:

```bash
-p 80:80
```

This mapped:

```text
Host Port 80 → Container Port 80
```

allowing users to access the web application through the EC2 Public IP.

---

## Network Flow

```text
Internet User
       |
       v
AWS Security Group
       |
       v
EC2 Instance
       |
       v
Docker Container
       |
       v
Nginx Web Server
       |
       v
Web Application
```

---

## Security Best Practices Implemented

- Restricted SSH access to personal IP.
- Enabled only required ports.
- Used key-based SSH authentication.
- Isolated application inside Docker container.
- Maintained separation between host OS and application runtime.

---

## Result

The application was securely exposed to the internet while maintaining controlled administrative access through SSH.

---

## Skills Demonstrated

- AWS Security Groups
- EC2 Networking
- Public IP Management
- Linux Server Administration
- SSH Authentication
- Docker Networking
- Web Application Hosting
