# Wazuh Installation Guide for Ubuntu Server

This guide provides step-by-step instructions for installing Wazuh on an Ubuntu Server.

## Prerequisites

- Ubuntu Server (20.04, 22.04, or 24.04)
- Root or sudo access
- Minimum 4GB RAM, 2 CPU cores (recommended for production)

## Installation Steps

### 1. Update and Upgrade System Packages

First, update the package lists and upgrade all installed packages:

```bash
sudo apt update
sudo apt upgrade -y
```

### 2. Download and run the Wazuh installation assistant.
```
sudo curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
```

## Message after : Installation finished
 - INFO: --- Summary ---
 - INFO: You can access the web interface https://<WAZUH_DASHBOARD_IP_ADDRESS>
    - User: ``admin``
    - Password: ``<ADMIN_PASSWORD>``
 - INFO: Installation finished.

## Note 
You can find the passwords for all the Wazuh indexer and Wazuh API users in the wazuh-passwords.txt file inside wazuh-install-files.tar. To print them, run the following command:
```
$ sudo tar -O -xvf wazuh-install-files.tar wazuh-install-files/wazuh-passwords.txt

````

- `` User: admin``
- ``  Password: G7wut6L?WIwQltQ29V6Av74EmQxC4H2d``
