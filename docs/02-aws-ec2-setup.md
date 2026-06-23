# AWS EC2 Setup

## EC2 Configuration

### Instance Details

* Operating System: Ubuntu Server 24.04 LTS
* Instance Type: t3.micro
* Platform: AWS EC2

### Networking

* VPC: Default VPC
* Subnet: Public Subnet
* Public IP: Enabled

### Security Group Rules

| Port | Protocol | Purpose               |
| ---- | -------- | --------------------- |
| 22   | SSH      | Remote Administration |
| 80   | HTTP     | Web Traffic           |
| 443  | HTTPS    | Secure Web Traffic    |

## Verification

Verified instance status and successful SSH connectivity.
