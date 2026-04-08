---Linux for devOps maintain---
# Linux for DevOps Engineers 🐧

This guide covers **essential Linux commands for DevOps**, including file management, permissions, networking, process control, logs, and automation.
Useful for **CI/CD, Cloud, Containers, and Production servers**.

---

# 📁 File & Directory Management

```bash
pwd
ls
ls -la
cd /path
mkdir project
rm file.txt
rm -rf folder
cp file1 file2
mv old new
touch file.txt
```

---

# 📄 File Viewing Commands

```bash
cat file.txt
less file.txt
more file.txt
head file.txt
tail file.txt
tail -f app.log
```

---

# 🔍 Search Commands (Very Important)

Find file

```bash
find / -name file.txt
```

Search inside file

```bash
grep "error" file.txt
```

Search recursively

```bash
grep -r "error" .
```

Search running process

```bash
ps aux | grep nginx
```

---

# 🔐 Permissions & Ownership

Check permissions

```bash
ls -l
```

Change permission

```bash
chmod 777 file.txt
chmod +x script.sh
```

Change ownership

```bash
chown user:user file.txt
```

---

# ⚙️ Process Management

Show running processes

```bash
ps aux
```

Real time process monitor

```bash
top
```

Kill process

```bash
kill PID
kill -9 PID
```

Find process

```bash
pgrep nginx
```

---

# 🌐 Networking Commands

Check IP

```bash
ip a
```

Ping server

```bash
ping google.com
```

Check open ports

```bash
netstat -tulnp
```

Check port usage

```bash
lsof -i :8080
```

Test API

```bash
curl http://localhost:3000
```

Download file

```bash
wget https://example.com/file.zip
```

---

# 📦 Package Management

Ubuntu / Debian

```bash
apt update
apt upgrade
apt install nginx
```

CentOS / RHEL

```bash
yum install nginx
```

---

# 📊 Disk & Memory Monitoring

Check disk

```bash
df -h
```

Check folder size

```bash
du -sh *
```

Check memory

```bash
free -m
```

---

# 📜 Logs (DevOps Most Important)

System logs

```bash
/var/log/syslog
```

View logs

```bash
tail -f /var/log/syslog
```

Docker logs

```bash
docker logs container
```

Nginx logs

```bash
/var/log/nginx/access.log
```

---

# 👤 User Management

Create user

```bash
useradd devops
```

Switch user

```bash
su devops
```

Sudo command

```bash
sudo apt update
```

---

# 🔄 Service Management (Systemctl)

Start service

```bash
systemctl start nginx
```

Stop service

```bash
systemctl stop nginx
```

Restart service

```bash
systemctl restart nginx
```

Check status

```bash
systemctl status nginx
```

Enable on boot

```bash
systemctl enable nginx
```

---

# 📦 Archive & Compression

Zip

```bash
zip file.zip file.txt
```

Unzip

```bash
unzip file.zip
```

Tar

```bash
tar -cvf file.tar folder
```

Extract

```bash
tar -xvf file.tar
```

---

# ⚡ DevOps Automation Commands

Environment variables

```bash
export ENV=production
echo $ENV
```

Run script

```bash
bash deploy.sh
```

Make executable

```bash
chmod +x deploy.sh
./deploy.sh
```

---

# ⭐ Most Important Linux Commands for DevOps

```
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
du -sh
free -m
curl
wget
systemctl
tail -f
```

---

# 🧠 DevOps Use Cases

* Server deployment
* CI/CD pipelines
* Log monitoring
* Docker & Kubernetes management
* Cloud instance setup
* Automation scripts
* Production debugging

---

# 🚀 DevOps Linux Workflow

```
Connect to Server (SSH)
        ↓
Pull Code (Git)
        ↓
Install Dependencies
        ↓
Build Application
        ↓
Restart Service
        ↓
Monitor Logs
```
