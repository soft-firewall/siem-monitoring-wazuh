**SIEM using Wazuh on Ubuntu Server**

**1. Project Overview**

This project focuses on building a **Security Information and Event Management (SIEM) system** using Wazuh on Ubuntu Server.\
The objective is to create a real-time cybersecurity monitoring environment that detects suspicious activities, collects system logs, and generates alerts to improve an organization’s security posture.

The system simulates a SecOps environment where security events are monitored and analyzed in real time.

**2. Problem Statement**

Organizations face increasing cybersecurity threats due to delayed threat detection and lack of centralized monitoring systems.\
Manual log monitoring is inefficient and often fails to detect suspicious activities in time, which can lead to data breaches, financial loss, and operational disruption.

This project aims to reduce uncertainty in threat detection by implementing a SIEM system that provides real-time monitoring and automated alerts.

**3. Objective**

The main objective of this project is to configure a SIEM system using Wazuh on Ubuntu Server to monitor system activities and detect potential security threats.

**Goals**

- Set up Ubuntu Server in a virtual environment
- Install and configure Wazuh SIEM
- Enable SSH-based remote access
- Monitor system logs and security events
- Generate real-time alerts
- Create a working cybersecurity monitoring prototype

**4. Tools and Technologies Used**

**Operating System**

- Ubuntu Server

**SIEM Platform**

- Wazuh

**Virtualization**

- VirtualBox

**Remote Access**

- Termius

**Additional Tools**

- Sublime Text
- SSH
- Web Browser
- Network Configuration

**5. System Architecture**

The system follows a simple cybersecurity monitoring architecture.

Ubuntu Server acts as the main system where Wazuh is installed and configured.\
Wazuh collects system logs and security events, processes them through the indexer, and displays alerts on the dashboard.

**Workflow**

Ubuntu Server

`     `↓

Wazuh Manager

`     `↓

Wazuh Indexer

`     `↓

Wazuh Dashboard

`     `↓

Security Alerts

This architecture allows real-time monitoring and threat detection.

**6. Step-by-Step Implementation**

**Step 1: Install Ubuntu Server**

Ubuntu Server was installed using VirtualBox to create a virtual environment.

Steps:

- Download Ubuntu Server ISO
- Create a new virtual machine
- Allocate RAM and storage
- Install Ubuntu Server
- Create username and password

Ubuntu was successfully installed and running.

**Step 2: Update System**

The system was updated to ensure all packages were current.

Command used:

sudo apt update && upgrade -y

This ensures system stability and security.

**Step 3: Install SSH**

SSH was installed to allow remote access.

Command:

sudo apt install openssh-server -y

Service started using:

sudo systemctl start ssh

sudo systemctl enable ssh

Ubuntu Server was now accessible remotely.

**Step 4: Connect using Termius**

Termius was used to connect to Ubuntu Server via SSH.

Steps:

- Get IP address using hostname -I
- Create host in Termius
- Enter IP, username, and password
- Connect to server

SSH connection was successfully established.

**Step 5: Install Wazuh**

Wazuh SIEM was installed using the official installation script.

Command:

curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh

sudo bash wazuh-install.sh -a -i

This installed:

- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard
- Security components

The installation process configured the SIEM system.

**7. Real-Time Monitoring**

After installation, Wazuh provides:

- log monitoring
- threat detection
- system analysis
- real-time alerts
- dashboard visualization

Security events are displayed on the dashboard.

**8. Expected Output**

The system produces:

- Ubuntu Server running
- SSH connection via Termius
- Wazuh installed
- Dashboard accessible
- Security alerts visible

This confirms successful SIEM deployment.

**9. Use Case**

The system is designed for mid-sized enterprises that need real-time cybersecurity monitoring.

**Before SIEM**

- manual log monitoring
- delayed threat detection
- security uncertainty

**After SIEM**

- real-time alerts
- centralized monitoring
- improved security posture

This improves SecOps efficiency.

**10. Learning Outcomes**

After completing this project, the following skills are gained:

- Linux server setup
- SIEM configuration
- SSH networking
- cybersecurity monitoring
- log analysis
- real-time threat detection

This builds practical cybersecurity experience.

**11. Conclusion**

The project successfully demonstrates how Wazuh SIEM can be deployed on Ubuntu Server to create a real-time cybersecurity monitoring system.

The system enhances threat detection, improves visibility, and strengthens the overall security posture of an organization.

This prototype can be extended into a full SecOps monitoring environment.

