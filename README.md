# SIEM using Wazuh on Ubuntu Server
Overview

This project demonstrates the deployment of a Security Information and Event Management (SIEM) system using Wazuh on Ubuntu Server.
The system is designed to monitor system activity, detect potential threats, and provide real-time security alerts through a centralized dashboard.
The goal is to simulate a real-world Security Operations Center (SOC) environment and build practical cybersecurity monitoring skills.

Problem Statement

Modern organizations struggle with:

*delayed threat detection

*scattered system logs

*lack of centralized monitoring

*slow incident response

Without a SIEM system, security threats often go unnoticed until damage is already done.
This project builds a real-time monitoring solution to improve visibility and threat detection.

Objective
*Install Ubuntu Server in a virtual environment
*Configure Wazuh SIEM
*Enable SSH remote access
*Monitor system logs and security events
*Generate real-time alerts
*Build a working cybersecurity monitoring prototype

Tech Stack
Operating System
 *Ubuntu Server
SIEM Platform
 *Wazuh
Virtualization
 *VirtualBox
Remote Access
 *Termius
Tools
 *Linux Terminal
 *SSH
 *Web Browser
 *GitHub
 
System Architecture
Ubuntu Server
      ↓
Wazuh Manager
      ↓
Wazuh Indexer
      ↓
Wazuh Dashboard
      ↓
Security Alerts

The Wazuh SIEM collects logs, processes them, and displays security alerts in real time.

Installation Steps
1. Install Ubuntu Server
Download ISO and install using VirtualBox.
Update system:
sudo apt update
sudo apt upgrade -y

2. Install SSH
sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh

Get IP address:
ip a

3. Install Wazuh
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh
sudo bash wazuh-install.sh -a

This installs:
Wazuh Manager
Wazuh Indexer
Wazuh Dashboard

Access Dashboard
After installation:
https://<server-ip>
Login credentials will be generated during installation.

Expected Output
*Ubuntu Server running
*Wazuh SIEM installed
*SSH remote access working
*Security dashboard accessible
*Real-time monitoring enabled

Project Structure
cybersecurity-siem-wazuh
│
├── README.md
├── installation-guide.md
├── architecture.md
├── screenshots
│   ├── ubuntu-install.png
│   ├── wazuh-install.png
│   ├── dashboard.png

Use Case
This project can be used by:
*cybersecurity students
*SOC analysts
*beginners in SIEM
*organizations learning threat monitoring
It demonstrates how to deploy a basic security monitoring environment.

Learning Outcomes
*Linux server setup
*SIEM deployment
*SSH networking
*Log monitoring
*Security alert analysis
*SOC fundamentals

Future Improvements
Add endpoint agents
Simulate cyber attacks
Integrate threat intelligence
Create automated alerts
Build incident response workflow

Author
Tanisha
Cybersecurity Student

License
This project is for educational and research purposes.
