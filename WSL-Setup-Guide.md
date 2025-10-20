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

## Step 4 — Install Git 🌱
Check if Git exists:
```
git --version
```
If not installed:
```
sudo apt install git -y
```
Then configure it with your GitHub name and email:
```
git config --global user.name "Sharmeen Fatima"
git config --global user.email "sharmeenfatima67@gmail.com"
```
Check configuration:
```
git config --list
```

---
## 💻 Step 5 — Install Visual Studio Code
1. Install VS Code from the official site if not already installed.
2. Open VS Code in Windows.

---

## 🔌 Step 6 — Install WSL Extension
1. In VS Code → open Extensions tab.
2. Search: WSL (Publisher: Microsoft)
3. Install it — description should say:
   ***“Open any folder in the Windows Subsystem for Linux (WSL) and take advantage of Visual Studio Code's full feature set.”***

---
## 🌐 Step 7 — Connect VS Code with Ubuntu
1. Click the >< (Open Remote Window) icon in bottom-left corner.
2. Choose Connect to WSL → Ubuntu
3. VS Code will open a new window with status:
   **💚 WSL: Ubuntu**
