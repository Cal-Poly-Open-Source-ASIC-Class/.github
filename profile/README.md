# Open Source ASIC Class

# Docker Installation
- [Windows](#windows-install)
- [Mac](#mac-install)
- [Linux](#linux-install)

## Windows Install
Everything we do in this class on Windows will be done in [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). Install it from PowerShell using `wsl --install` and set up a username/password.


Install [Docker Desktop](https://www.docker.com/products/docker-desktop/). Once set up, enable WSL integration so that your WSL instances can access docker.

![alt text](docker.png)

## Mac Install

### Step 1: Install Docker
Install [Docker](https://www.docker.com/products/docker-desktop/). 

After installation open Docker from your mac, make an account and ensure the software is running.

### Step 2: Install and Setup XQuartz
Ensure XQuartz is Installed and Running:

1. Install XQuartz from https://www.xquartz.org/. Launch XQuartz after installation. Configure XQuartz to Allow Network Connections:
2. Go to XQuartz > Preferences > Security. Uncheck the option Authenticate connections. Check the option Allow connections from network clients.
3. Restart XQuartz for the changes to take effect.

## Linux Install

Install [Docker](https://www.docker.com/products/docker-desktop/) with your preferred package manager. For example:
`sudo apt install docker` 
