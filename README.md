
# EC2 Service Using Linux (Ubuntu / Amazon Linux)

This guide explains how to launch, connect, configure, and deploy applications on an AWS EC2 instance using Linux-based operating systems such as Ubuntu or Amazon Linux.

---

1. Launch an EC2 Instance

### Steps:
1. Log in to AWS Console.
2. Open **EC2** from the services menu.
3. Click **Launch Instance**.
4. Enter an instance name.
5. Select AMI:
   - Ubuntu Server 22.04 LTS  
   - Amazon Linux 2023
6. Choose instance type: **t2.micro** (Free-tier eligible).
7. Create or select an existing **key pair** (.pem file).
8. Configure network:
   - Allow **SSH (22)**
   - Allow **HTTP (80)** if hosting a website
   - Allow **HTTPS (443)** if using SSL
9. Add storage (default 8–16 GB is enough).
10. Click **Launch Instance**.

---

 2. Connect to EC2 (SSH)

chmod 400 your-key.pem
ssh -i your-key.pem ec2-user@your-public-ip




