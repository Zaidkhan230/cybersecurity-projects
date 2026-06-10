# cybersecurity-projects
# SOC Monitoring and Threat Detection Lab

Project Overview:
This project was created to understand how Security Operations Center (SOC) monitoring works in a real environment using virtual machines.  
A home lab was built using Ubuntu, Kali Linux, and Windows Server with Wazuh SIEM for monitoring security events and detecting suspicious activity.
The project includes monitoring failed login attempts, authentication logs, endpoint activity, and basic threat detection from both Linux and Windows systems.

# Step-by-Step Setup

Step 1 — Created Virtual Lab Environment
  Installed VMware Workstation and created the following virtual machines:

  - Ubuntu Linux
  - Kali Linux
  - Windows Server
All machines were connected in the same network for communication.

Step 2 — Installed Wazuh SIEM on Ubuntu
  Ubuntu machine was used as the central SIEM server.
  Installed:
  - Wazuh Manager
  - Wazuh Dashboard
  - Wazuh Indexer
The dashboard was used for monitoring alerts and security logs.

Step 3 — Connected Kali Linux to Ubuntu
  Kali Linux was connected to the Ubuntu Wazuh server through network communication.

  Performed:
  - Ping testing
  - SSH connection testing
  - Authentication monitoring
Generated failed SSH login attempts from Kali Linux to create security alerts.

 Step 4 — Monitored Linux Security Events
  Wazuh detected and monitored:

  - Failed SSH login attempts
  - Authentication failures
  - PAM login alerts
  - Suspicious login activity
Security alerts were visible in the Wazuh dashboard.

Step 5 — Installed Sysmon on Windows Server
  Installed Sysmon on Windows Server for endpoint monitoring and system activity logging.

  Monitored:
  - PowerShell activity
  - Process creation events
  - Login activity
  - Endpoint events

Step 6 — Connected Windows Logs to Wazuh
  Installed Wazuh Agent on Windows Server and connected it to the Ubuntu Wazuh server.
  Windows security logs were forwarded to the SIEM dashboard for centralized monitoring.

Step 7 — Generated Security Events
  Performed basic testing to generate alerts such as:
  - Failed login attempts
  - SSH authentication failures
  - PowerShell activity
  - Privilege escalation events
  - Endpoint monitoring alerts

Tools Used
  - Wazuh SIEM
  - Sysmon
  - Ubuntu Linux
  - Kali Linux
  - Windows Server
  - VMware Workstation
  - PowerShell

Security Monitoring Features
  - SIEM Monitoring
  - Log Analysis
  - Security Event Monitoring
  - Endpoint Monitoring
  - Authentication Monitoring
  - Threat Detection
  - MITRE ATT&CK Alert Mapping

Networking Concepts Used
  - TCP/IP
  - DNS
  - SSH
  - LAN Connectivity
  - Firewall Basics

Screenshots Included
  - Wazuh Dashboard
  - Security Events Page
  - Failed Login Alerts
  - Sysmon Installation
  - Wazuh Agent Connection
  - Kali Linux SSH Testing
  - Windows Endpoint Monitoring

Learning Outcome
  This project helped in understanding basic SOC operations, SIEM monitoring, Linux and Windows log monitoring, endpoint security monitoring, and security event analysis using a practical virtual lab setup.
