# Windows Endpoint Monitoring Lab

Project Overview
  
  In this project, I worked on monitoring Windows endpoint activity using Wazuh SIEM and Sysmon in a virtual lab environment.
  The setup was done using Windows Server, Ubuntu Linux, and VMware Workstation. The main goal of this project was to understand how Windows security logs and endpoint activities are monitored inside a SOC environment.
  I connected the Windows machine to the Wazuh dashboard running on Ubuntu and monitored different security events like failed logins, PowerShell activity, authentication logs, and endpoint alerts.

Project Setup
Step 1 — Created the Windows Virtual Machine
  I created a Windows Server virtual machine using VMware Workstation and connected it to the same network as the Ubuntu Wazuh server.
  This helped in communication between both systems for monitoring and log collection.

Step 2 — Checked Network Connectivity
Before starting monitoring, I checked whether the Windows machine could communicate with the Ubuntu Wazuh server using ping testing.
This confirmed that both systems were connected properly.

Step 3 — Installed Sysmon
I installed Sysmon on the Windows machine for endpoint monitoring.
Sysmon was used to monitor:
  * Process activity
  * PowerShell usage
  * System events
  * Endpoint behavior
After installation, I verified that the Sysmon service was running successfully.

Step 4 — Installed Wazuh Agent
I installed the Wazuh agent on the Windows machine and connected it to the Ubuntu Wazuh SIEM server.
Once connected, the Windows logs started appearing inside the Wazuh dashboard.

Step 5 — Monitored Windows Security Events
After connecting the agent, I monitored different security events such as:
  * Failed login attempts
  * Authentication logs
  * PowerShell activity
  * Endpoint alerts
  * Windows security logs
The alerts were visible directly inside the Wazuh dashboard.

Tools Used
  * Wazuh SIEM
  * Sysmon
  * Windows Server
  * Ubuntu Linux
  * VMware Workstation
  * PowerShell

Concepts Covered
  * SIEM Monitoring
  * Endpoint Monitoring
  * Security Event Monitoring
  * Windows Log Monitoring
  * Authentication Monitoring
  * Threat Detection
  * PowerShell Monitoring

Screenshots Included
  * Sysmon Installation
  * Wazuh Agent Connection
  * Windows Security Events
  * Failed Login Alerts
  * Active Agent Status
  * Wazuh Dashboard Monitoring

What I Learned
  This project helped me understand how endpoint monitoring works in a SOC environment using Windows logs and SIEM tools. I also learned how security alerts are generated, monitored, and analyzed using Wazuh and Sysmon.
