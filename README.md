## 💻 Linux System Administration – Hands-on Portfolio

![Linux](https://img.shields.io/badge/Linux-System%20Administration-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Ubuntu-Server-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-Web%20Server-D22128?style=for-the-badge&logo=apache&logoColor=white)
![SSH](https://img.shields.io/badge/SSH-Secure%20Access-blue?style=for-the-badge)
![Firewall](https://img.shields.io/badge/UFW-Firewall-green?style=for-the-badge)

---

## 👨‍💻 About This Project

This portfolio demonstrates hands-on Linux System Administration skills through practical lab work including user management, SSH configuration, firewall setup, and Apache web server deployment.

---

## 🎯 Core Objectives

- User management in Linux  
- Secure SSH configuration  
- Firewall setup using UFW  
- Apache web server deployment  
- Linux command-line operations  

---

# 👤 1. User Management

## 🎯 Objective
Create and manage Linux users using terminal commands.

## 🧪 Commands
```bash
sudo useradd testuser
sudo passwd testuser
cat /etc/passwd | grep testuser

## 📸 Screenshots
<img width="524" height="207" alt="Screenshot 2026-05-01 030535" src="https://github.com/user-attachments/assets/3eae7b3a-9a6a-4d73-9bac-aa39a14bdd09" />

## 📌 Outcome
Successfully created and managed Linux user accounts using command-line tools.

---

## 🔐 2. SSH Setup

## 🔐 SSH Setup & Basic Security (Linux)
## 📌 Overview

This project demonstrates installation and basic configuration of the SSH service on a Linux system to enable secure remote access.

## 🎯 Objectives
- Install OpenSSH server
- Start and enable SSH service
- Verify SSH service status
- Test local SSH connection

---

## ⚙️ Tools Used
- Kali Linux / Ubuntu
- OpenSSH Server
- systemd (systemctl)
- Terminal (CLI)

---

## 🧪 Steps Performed
## 1. Install SSH Server
Installed OpenSSH server package.

- sudo apt update
- sudo apt install openssh-server -y
  
  ---
  
## 2. Start SSH Service
Started the SSH service.

- sudo systemctl start ssh

---
## 3. Enable SSH on Boot
Enabled SSH to start automatically on system boot.

- sudo systemctl enable ssh

---
## 4. Check SSH Status
Verified that SSH service is running.

- sudo systemctl status ssh

✔ Expected output: active (running)
✔ SSH listening on port 22

---

## 5. Find System IP
Checked system IP address.

- hostname -i

---

## 6. Test SSH Connection (Localhost)
Tested SSH connection on local machine.

- ssh localhost

✔ Confirmed SSH authentication prompt
✔ Verified successful login

---

## 📸 Screenshots

- SSH installation output
- systemctl status ssh (active running)
- SSH login attempt (localhost prompt)
<img width="688" height="186" alt="Screenshot 2026-05-01 031523" src="https://github.com/user-attachments/assets/657aec4c-066e-4b4b-aef0-f1c0d9ee5862" />
---
<img width="759" height="352" alt="Screenshot 2026-05-01 031550" src="https://github.com/user-attachments/assets/4ecdd2cf-025c-4f95-86ea-29d99d6bfc61" />
---
<img width="739" height="191" alt="Screenshot 2026-05-01 031640" src="https://github.com/user-attachments/assets/038b184b-11b6-4477-95c1-f19e6c6aa418" />

---

## 🔐 Key Learning
- SSH provides secure remote access to Linux systems
- systemctl manages system services
- Port 22 is default SSH port
- Local testing confirms correct configuration

---

## 📌 Outcome
Successfully installed and configured SSH service on Linux and verified secure local access using SSH protocol.

---

## 🔥 3. Firewall Setup (UFW)

## 🔥 Linux Firewall Setup (UFW)
## 📌 Overview
This project demonstrates how to configure a firewall on Linux using UFW to control network access and improve system security.

---

## 🎯 Objectives
- Install and configure UFW firewall
- Allow essential services (SSH, HTTP)
- Enable firewall protection
- Verify firewall rules

---

## ⚙️ Tools Used
- Linux (Kali/Ubuntu)
- UFW Firewall
- Terminal (CLI)

---

## 🧪 Steps Performed
1. Install UFW
- sudo apt update
- sudo apt install ufw -y

---

2. Check Firewall Status
- sudo ufw status

✔ Expected: Status: inactive

---

## ⚠️ IMPORTANT
Before enabling firewall, always allow SSH to avoid losing access.

---

## 3. Allow SSH
- sudo ufw allow ssh

---

## 4. Enable Firewall
- sudo ufw enable

When asked:

- Proceed? (y/n)

## 👉 Type: y

## 5. Allow HTTP Traffic
- sudo ufw allow http

---

## 6. Check All Rules
- sudo ufw status verbose

✔ Expected:

SSH ALLOW
HTTP ALLOW
Status: active

---

## 7. (Optional) Block a Port
sudo ufw deny 23

---

## 📸 Screenshots
- UFW installation
- Firewall status (inactive)
- SSH allow rule
- Firewall enabled
- Final rules (status verbose)

---

<img width="847" height="609" alt="Screenshot 2026-05-01 035407" src="https://github.com/user-attachments/assets/b2c06872-caa6-4412-a2fe-e9971804c1cc" />
---
<img width="265" height="74" alt="Screenshot 2026-05-01 033058" src="https://github.com/user-attachments/assets/b46c7097-2065-4266-be76-2376dc43c222" />
---
<img width="275" height="85" alt="Screenshot 2026-05-01 033114" src="https://github.com/user-attachments/assets/1b03d2ae-e372-493a-91f7-4c7121c8d471" />
---
<img width="682" height="85" alt="Screenshot 2026-05-01 033136" src="https://github.com/user-attachments/assets/5adb838c-9bcf-4972-85d6-7e33db8367cf" />
---
<img width="591" height="217" alt="Screenshot 2026-05-01 033217" src="https://github.com/user-attachments/assets/66726acb-255d-416e-84cb-2c72ba5ab231" />

---

## 🔐 Key Learning
- Firewall controls system network access
- UFW simplifies Linux firewall management
- SSH must be allowed before enabling firewall
- Rules define allowed and blocked traffic

----

## 📌 Outcome
Successfully configured a Linux firewall to allow SSH and HTTP traffic while securing all other incoming connections.

---

## 🌐 Apache Web Server Project

## 📌 Overview
This project demonstrates how to install and configure Apache web server on Linux and host a basic web page.

---

## 🎯 Objectives
- Install Apache2  
- Start and enable Apache service  
- Create custom web page  
- Access server via browser  

---

## ⚙️ Tools Used
- Linux (Kali/Ubuntu)  
- Apache2  
- Terminal (CLI)  

---

## 🧪 Steps Performed

### 1. Install Apache
sudo apt install apache2 -y

### 2. Start Service
sudo systemctl start apache2  
sudo systemctl enable apache2  

### 3. Create Web Page
sudo nano /var/www/html/index.html  

### 4. Restart Server
sudo systemctl restart apache2  

### 5. Test in Browser
http://localhost  

---

## 📸 Screenshots

<img width="754" height="109" alt="Screenshot 2026-05-01 043624" src="https://github.com/user-attachments/assets/ce280481-9db7-4e47-ba52-f577267a4ac1" />
---
<img width="786" height="341" alt="Screenshot 2026-05-01 070725" src="https://github.com/user-attachments/assets/b5b831aa-9866-4190-aa4f-a75906a0c467" />


## 🧠 Key Learning
- Apache is used to host websites  
- index.html is the main web file  
- Browser is used to access server  
- Linux can act as a web server  

---

## 📌 Outcome
Successfully deployed Apache web server and hosted a custom HTML page on localhost.
