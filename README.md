# Linux for DevOps using AWS EC2 (Ubuntu) 🐧☁️

This guide explains how to **use AWS EC2 Ubuntu as a Linux machine for DevOps practice**.
You can use this VM for **Linux commands, Git, Docker, CI/CD, deployment, and automation**.

---

# 🎯 Purpose of Using Linux on AWS EC2 for DevOps

* Practice Linux commands on real server
* Deployment environment
* CI/CD pipeline server
* Docker & Kubernetes practice
* Git server operations
* Log monitoring
* Automation scripting
* Production-like environment

---

# 🚀 Step 1 — Create Linux VM (Ubuntu EC2)

Launch instance with:

```
Name: devops-linux-server
AMI: Ubuntu Server 22.04 LTS
Instance: t2.micro
Security: Allow SSH, HTTP, HTTPS
```

Download key:

```
devops.pem
```

---

# 🔐 Step 2 — Connect to Linux Server

```bash
chmod 400 devops.pem
ssh -i devops.pem ubuntu@your-ec2-ip
```

Now you are inside **Linux machine**.

---

# 🐧 Basic Linux Commands for DevOps

### File Commands

```bash
pwd
ls
ls -la
cd /var/www
mkdir project
rm -rf folder
```

### File Viewing

```bash
cat file.txt
less file.txt
tail -f app.log
```

---

# 📦 Install DevOps Tools on Linux

Update system

```bash
sudo apt update && sudo apt upgrade -y
```

Install Git

```bash
sudo apt install git -y
```

Install Docker

```bash
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
```

Install Node

```bash
sudo apt install nodejs npm -y
```

---

# 🌐 Linux Networking Commands

```bash
ip a
ping google.com
curl localhost:3000
netstat -tulnp
```

---

# ⚙️ Process Management

```bash
ps aux
top
kill -9 PID
```

---

# 📊 Monitor Linux Server

Check memory

```bash
free -m
```

Check disk

```bash
df -h
```

Check CPU

```bash
top
```

---

# 📜 Linux Logs (DevOps Important)

System logs

```bash
tail -f /var/log/syslog
```

Nginx logs

```bash
tail -f /var/log/nginx/access.log
```

App logs

```bash
tail -f app.log
```

---

# 🔄 DevOps Deployment on Linux

Clone repository

```bash
git clone https://github.com/user/project.git
cd project
```

Install dependencies

```bash
npm install
```

Run app

```bash
npm start
```

Run in background

```bash
nohup npm start &
```

---

# 🔐 Linux Permissions (DevOps Must Know)

```bash
chmod 777 file
chmod +x deploy.sh
chown ubuntu:ubuntu file
```

---

# 🔁 Service Management

Start service

```bash
sudo systemctl start nginx
```

Stop service

```bash
sudo systemctl stop nginx
```

Restart service

```bash
sudo systemctl restart nginx
```

---

# 🧠 DevOps Linux Workflow

```
Create EC2 Ubuntu
        ↓
SSH into Linux
        ↓
Install Git/Docker
        ↓
Clone Repository
        ↓
Build Application
        ↓
Run Application
        ↓
Monitor Logs
```

---

# ⭐ Most Important Linux Commands for DevOps

```bash
ssh
ls
cd
pwd
chmod
chown
grep
find
top
kill
ps
df -h
free -m
tail -f
systemctl
```

---

# 📌 Use Case

* Linux practice
* DevOps practice
* Deployment server
* CI/CD server
* Docker host
* Kubernetes node
* Cloud Linux machine

---
