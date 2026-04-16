<p align="center">
  <img src="assets/banner.png" alt="The Abandoned Gate Banner" width="80%"/>
</p>

<h1 align="center">🚪 The Abandoned Gate</h1>

<p align="center">
  A web exploitation CTF challenge focused on insecure file upload leading to RCE and privilege escalation.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Category-Web%20Exploitation-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Exploit-File%20Upload%20RCE-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Difficulty-Medium-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Platform-Docker-blue?style=for-the-badge" />
</p>

---

## 📌 Challenge Overview

**The Abandoned Gate** is a deliberately vulnerable web application designed for CTF practice.

It simulates a real-world scenario where:
- A file upload feature is misconfigured
- Remote code execution is possible
- Privilege escalation leads to full system compromise

---

## 🎯 Objectives

1. 🔍 Locate the hidden file upload functionality (Abandoned Gate)
2. 📤 Upload a malicious PHP payload
3. 💣 Trigger Remote Code Execution (RCE) and obtain a reverse shell
4. ⬆️ Escalate privileges to root access

---

## ⚙️ Requirements

- Docker installed  
  👉 https://docs.docker.com/get-started/get-docker/

---

## 📥 Installation

### Clone Repository
```bash
git clone https://github.com/PkTheHacker10/ctf-dev.git
cd ctf-dev
````

---

## 🚀 Setup Guide

### ⚡ Method 1: Automated Setup

```bash
cd challenge
sudo ./setup.sh
```

---

### 🛠 Method 2: Manual Setup

```bash
cd challenge/web
sudo docker build -t abandoned-gate .
sudo docker run -d --name ctf-gate abandoned-gate
```

---

## 🌐 Accessing the Challenge

Find container IP:

```bash
sudo docker exec ctf-gate ifconfig
```

Then open in browser:

```
http://container-ip
```

---

## 🧹 Stop & Remove Container

```bash
sudo docker stop ctf-gate
sudo docker rm ctf-gate
```

---

## 📖 Walkthrough

A full solution guide is available in:

```
WALKTHROUGH.md
```

---

## ⚠️ Disclaimer

This project is for **educational and ethical hacking practice only**.

Do not deploy in production or attack unauthorized systems.

---

## 🏴 Happy Hacking 🚪
