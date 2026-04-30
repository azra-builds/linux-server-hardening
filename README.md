## 💻 Linux System Administration Projects
## 📌 Overview

This repository contains Linux administration projects including user management, SSH setup, and firewall configuration.

## 👤 1. User Management

## 📌 Overview
This project demonstrates basic Linux user management using terminal commands.

## ⚙️ Steps Performed
- Created a user using useradd  
- Set password for the user  
- Verified user in system files  

## 🧪 Commands Used
- sudo useradd testuser  
- sudo passwd testuser  
- cat /etc/passwd | grep testuser  

## 📸 Screenshots
<img width="524" height="207" alt="Screenshot 2026-05-01 030535" src="https://github.com/user-attachments/assets/3eae7b3a-9a6a-4d73-9bac-aa39a14bdd09" />

## 📌 Outcome
Successfully created and managed Linux user accounts using command-line tools.


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
<img width="759" height="352" alt="Screenshot 2026-05-01 031550" src="https://github.com/user-attachments/assets/4ecdd2cf-025c-4f95-86ea-29d99d6bfc61" />
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
