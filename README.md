# 💻 Linux System Administration – Hands-on Portfolio

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
```

## 📸 Screenshot

<img width="524" height="207" alt="Screenshot 2026-05-01 030535" src="https://github.com/user-attachments/assets/6fd45a75-a44c-4c47-a82a-ed27cbe13909" />

##📌 Outcome

Successfully created and managed Linux user accounts using command-line tools.

---

## 🔐 2. SSH Setup (COPY-PASTE READY)

## 🔐 2. SSH Setup

## 🎯 Objective
Enable secure remote access using SSH.

## 🧪 Commands

```bash
sudo apt update
sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh
sudo systemctl status ssh
hostname -i
ssh localhost
```
---

## 📸 Screenshot
---
```sudo apt install openssh-server -y```
<img width="714" height="85" alt="Screenshot 2026-05-01 024132" src="https://github.com/user-attachments/assets/1d5b6186-daaa-41cb-a2ec-3eb75c2282ad" />

```sudo systemctl status ssh```
<img width="759" height="352" alt="Screenshot 2026-05-01 031550" src="https://github.com/user-attachments/assets/68129bb7-63bd-495b-b764-65132225c358" />

```ssh localhost```
<img width="739" height="191" alt="Screenshot 2026-05-01 031640" src="https://github.com/user-attachments/assets/1be1f417-7037-48e8-b371-edfce52bd51c" />

---

📌 Outcome

SSH service successfully installed, enabled, and tested locally.

## 🔥 3. Firewall Setup (UFW)

## 🔥 3. Firewall Setup (UFW)

## 🎯 Objective
Secure system using firewall rules.

## 🧪 Commands

```bash
sudo apt update
sudo apt install ufw -y
sudo ufw status
sudo ufw allow ssh
sudo ufw enable
sudo ufw allow http
sudo ufw status verbose
```
## 📸 SCREENSHOTS 
```sudo ufw status```
<img width="265" height="74" alt="Screenshot 2026-05-01 033058" src="https://github.com/user-attachments/assets/108d96e0-8d2c-409e-81db-120fcc237f2e" />

```sudo ufw allow ssh```
<img width="275" height="85" alt="Screenshot 2026-05-01 033114" src="https://github.com/user-attachments/assets/31bffde0-26dc-4f36-9c55-3d3d1740c66c" />

```sudo ufw enable```
<img width="682" height="85" alt="Screenshot 2026-05-01 033136" src="https://github.com/user-attachments/assets/7ad37209-b338-4779-be69-9d4b24775ab6" />

```sudo ufw status verbose```
<img width="591" height="217" alt="Screenshot 2026-05-01 033217" src="https://github.com/user-attachments/assets/39479992-18c2-453d-a2f1-c70975193f6f" />

📌 Outcome

Firewall successfully configured to allow SSH and HTTP traffic.

---

## 🌐 4. Apache Web Server (COPY-PASTE READY)
## 🌐 4. Apache Web Server Setup

## 🎯 Objective
Deploy a web server using Apache on Linux.

## 🧪 Commands

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
sudo systemctl status apache2
```

## 🌍 Test in Browser

http://localhost/

## 📸 SCREENSHOTS
```sudo apt install apache2 -y```
<img width="798" height="465" alt="Screenshot 2026-05-01 040921" src="https://github.com/user-attachments/assets/9ed32dbf-9bfb-46b6-88cf-1ad098f48f2b" />
```sudo systemctl status apache2```
<img width="754" height="109" alt="Screenshot 2026-05-01 043624" src="https://github.com/user-attachments/assets/b061ecde-ebc5-4ad7-a90b-4961bf34fae6" />

## 3. Browser output
http://localhost/

## 📌 Outcome
Apache web server successfully installed and a default web page is running on localhost.
