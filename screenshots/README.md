## Lab Architecture

<img width="952" height="877" alt="pfsense-dashboard" src="https://github.com/user-attachments/assets/55e2bf27-03d0-4663-9bec-bb8f662de308" />

pfSense acts as the firewall and network gateway.
Windows 11 is the monitored endpoint.
Kali Linux is used to generate attack traffic.
Wazuh serves as the SIEM and detection platform.
Suricata provides network intrusion detection.

## Wazuh Agent Deployment

<img width="1022" height="662" alt="Wazuh-agents" src="https://github.com/user-attachments/assets/9e5997c7-1e65-487b-a745-4a395d4e8854" />

Successfully enrolled the Windows 11 endpoint and Kali Linux into Wazuh and verified agent communication.


## Sysmon Integration

<img width="1027" height="662" alt="threat-hunting-sysmon" src="https://github.com/user-attachments/assets/0408f625-9bd3-4a71-8039-66dda1af704d" />


Installed Sysmon with a community configuration to enhance Windows telemetry collection. Wazuh ingests Sysmon events for process creation, file creation, registry activity, and PowerShell monitoring.

## Threat Detection

<img width="942" height="802" alt="threat-detection" src="https://github.com/user-attachments/assets/b70d335f-743f-4325-8856-cb5260393920" />

Wazuh detected suspicious activity and mapped events to MITRE ATT&CK techniques for investigation.

## Wazuh Dashboard

<img width="1010" height="654" alt="wazu-dashboard" src="https://github.com/user-attachments/assets/c08fe26d-e872-4649-a03e-cec2a509c93b" />

Centralized visibility into endpoint events, alerts, vulnerabilities, and threat hunting data.

## Suricata IDS Detection

<img width="932" height="717" alt="Suricata-IDS-alert" src="https://github.com/user-attachments/assets/105d9449-485b-4cf0-acde-64c3e22cdf8a" />

Deployed Suricata IDS on pfSense and generated alerts from network reconnaissance activity. Verified rule loading, logging, and alert generation after troubleshooting rule category configuration. Used nmap from Kali VM to simulate discovery attack on Windows VM.


