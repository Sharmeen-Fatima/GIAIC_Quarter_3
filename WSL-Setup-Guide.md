# 🐧 WSL + Ubuntu + VS Code — Step-by-Step Setup Guide

> **Note:** This guide skips BIOS virtualization steps.  
> If you see an error like `0x80370102`, enable **Virtual Machine Platform** in Windows Features and ensure virtualization is turned on in BIOS.

---

## 🧩 Overview
This guide explains how to install and set up **WSL (Windows Subsystem for Linux)** with **Ubuntu**, connect it to **Visual Studio Code**, install **Git**, and run simple test files (Python, Bash, HTML).  
Just follow the steps in order — copy & paste the commands where shown.

---

## ⚙️ Prerequisites
- Windows 10 or later  
- Internet connection  
- Administrator access to Windows (to run PowerShell as Admin)

---

## Step 1 — Install WSL (Ubuntu) 📝
Open **PowerShell (Run as Administrator)** and run:

```powershell
wsl --install
```

---

## Step 2 — Setup Ubuntu user
1. Open **Start Menu → Ubuntu**
2. Wait for installation to finish.
3. When asked:
    - Username: lowercase, no spaces (example: sharmeen)
    - Password: 8–10+ characters (won’t show while typing)
After setup, you’ll see a prompt like:
```
sharmeen@DESKTOP-XXXX:~$
```
---

## Step 3 — Update the system 🧰
Run these commands inside Ubuntu terminal:
```
sudo apt update && sudo apt upgrade -y
```
Wait for it to finish (this updates your Linux system).

---
