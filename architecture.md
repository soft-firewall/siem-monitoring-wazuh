# System Architecture

## Overview

This document explains the architecture of the Wazuh SIEM project.

## Components

### Ubuntu Server
Main operating system hosting the SIEM environment.

### Wazuh Manager
Processes logs and security events.

### Wazuh Indexer
Stores and organizes security data.

### Wazuh Dashboard
Displays real-time alerts and monitoring.

## Workflow

Ubuntu Server → Wazuh Manager → Wazuh Indexer → Wazuh Dashboard → Security Alerts
