---
toc: True
layout: post
data: setup
title: Tools and Equipment Setup - Individual Guide
description: My journey through setting up tools and equipmet.
categories: ['DevOps']
author: Adya Shipekar
permalink: /tools/blog
breadcrumb: True 
---

## Overview

In Sprint 1, we learned how to set up the basic tools and equipment and implement basic functions of VSCode to run our repositories. Here's a brief explanation of how I set up my computer to successfully run the tools necessary in CSSE:

**_NOTE: This setup is for WINDOWS computers only. If you are running your tools on a Mac or Kasm, the process may differ._**

---


### Step 1: Create Accounts


1. **Slack** – Sign up at [slack.com](https://slack.com) using a personal email. The CSSE workspace link can be found on the Open Coding Society pages.
2. **GitHub** – Create an account at [github.com](https://github.com). Choose a strong username and password (and be sure to remember these!)
3. **OpenCS** – Register on the OpenCS platform so that you can be signed in/out of class.


---


### Step 2: Install VS Code


Download and install **Visual Studio Code** from [code.visualstudio.com](https://code.visualstudio.com/).


- Install recommended extensions:
- *Python*
- *GitHub Pull Requests and Issues*
- *Jupyter Notebooks* (you will need this in future projects)


---


### Step 3: Fork the Repository


1. Go to your GitHub account.
2. Go to Open-Coding-Society student repository and click **Fork** to fork the student repo.
3. This fork will serve as your personal workspace.


---


### Step 4: Set Up WSL


1. Open **PowerShell** as Administrator.
2. Run:
```powershell
wsl --install
```
3. Restart your system.
4. Open WSL (Ubuntu by default).
5. Update your packages:
```bash
sudo apt update && sudo apt upgrade -y
```


---


### Step 5: Clone Repo in WSL


Inside your WSL terminal:


```bash
cd ~
git clone https://github.com/<your-username>/<your-forked-repo>.git
cd <your-forked-repo>
```


---


### Step 6: Open VS Code from WSL


In your WSL terminal:


```bash
code .
```


This will launch VS Code connected to your WSL environment.


---


### Step 7: Run `make`


Many projects include a **Makefile**. To build or run tasks:


```bash
make
```


If there are specific targets:


```bash
make test
make run
```


---


✅ Congratulations! You now have Slack, GitHub, OpenCS, VS Code, and WSL all set up. You’ve forked and cloned your project, and successfully run `make` inside WSL. 🚀