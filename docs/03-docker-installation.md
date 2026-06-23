# Docker Installation

## Overview

Docker was installed on an Ubuntu EC2 instance to enable containerized application deployment.

---

## Update Package Repository

```bash
sudo apt update
```

---

## Install Docker

```bash
sudo apt install docker.io -y
```

---

## Start Docker Service

```bash
sudo systemctl start docker
```

---

## Enable Docker on Boot

```bash
sudo systemctl enable docker
```

---

## Verify Docker Installation

Check Docker version:

```bash
docker --version
```

Run the Docker test container:

```bash
sudo docker run hello-world
```

---

## Expected Output

The hello-world container confirms:

- Docker Engine is installed.
- Docker daemon is running.
- Containers can be downloaded and executed successfully.

---

## Result

Docker was successfully installed and configured on the AWS EC2 Ubuntu server.

---

## Skills Demonstrated

- Linux package management
- Docker installation
- Service management with systemctl
- Container verification
- Linux server administration
