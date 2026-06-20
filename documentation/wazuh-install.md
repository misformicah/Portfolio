Contents:

Purpose

Centralized log collection and threat detection.

Installation
  Ubuntu server installation
  Wazuh installation method
  Dashboard access
  Initial login
Agent Configuration
  Windows agent installation
  Agent registration
  Manager connection
Validation
  Agent appears in dashboard
  Logs received

Wazuh (4.14) was installed onto the Ubuntu Server (24.04) and configured to monitor the Windows 11 Enterprise VM and KAli Linux VM. Troubleshooting was done during installation with initial compatability issues, lack of storage space, and network timeout issues. Ubuntu Server was downgraded from 26 to 24.04, storage allocation for the VDI was increased to 60GB, and network timeout was resolved by disabling hardware checksum offloading in the pfSense dashboard
