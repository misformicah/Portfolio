# Home SOC Lab

## Overview

This repository documents my virtualized Security Operations Center (SOC) home lab built to develop hands-on experience in cybersecurity monitoring, threat hunting, vulnerability management, and incident response.

The environment consists of pfSense, Kali Linux, Ubuntu Server running Wazuh, and a Windows 11 Enterprise endpoint configured with Sysmon for advanced telemetry collection.

## Lab Architecture

<img width="745" height="678" alt="network-diagram-1 0" src="https://github.com/user-attachments/assets/e9fb4fef-33b3-4e7f-9a98-e7be66ea469e" />


## Technologies Used

* Wazuh SIEM
* Sysmon
* pfSense
* Suricata
* pfBlockerNG
* Kali Linux
* Ubuntu Server
* Windows 11 Enterprise
* VirtualBox

## Current Capabilities

### Network Security

* pfSense firewall management
* Internal network segmentation
* DHCP services
* Suricata IDS/IPS
* pfBlockerNG threat intelligence filtering

### Endpoint Monitoring

* Wazuh agent deployment
* Windows event log collection
* Sysmon telemetry collection
* Process creation monitoring
* File creation monitoring
* Registry activity monitoring
* Network connection monitoring

### Threat Detection

* MITRE ATT&CK mapped detections
* Sysmon-based alerting
* Threat hunting through Wazuh
* Event correlation and analysis

### Vulnerability Management

* Endpoint vulnerability detection
* CVE identification and tracking
* CVSS-based risk assessment
* Operating system vulnerability monitoring

## Current Lab Status

Completed:

* pfSense deployment
* Suricata deployment
* pfBlockerNG deployment
* Kali Linux deployment
* Ubuntu Server deployment
* Windows 11 Enterprise deployment
* Internal network configuration
* DHCP configuration
* Wazuh deployment
* Wazuh agent deployment
* Sysmon deployment
* Sysmon log collection
* Vulnerability detection
* Threat hunting dashboard validation

In Progress:

* PowerShell logging
* File Integrity Monitoring (FIM)
* Custom detection engineering

Planned:

* Atomic Red Team testing
* Attack simulation scenarios
* Incident response playbooks
* pfSense log ingestion into Wazuh

## Skills Demonstrated

* SIEM Administration
* Threat Hunting
* Log Analysis
* Vulnerability Management
* Detection Engineering
* Network Security Monitoring
* Firewall Administration
* IDS/IPS Configuration & Management
* Linux Administration
* Windows Security Monitoring
* Incident Investigation
* MITRE ATT&CK Analysis
* Virtualization
* Security Operations (SOC)

## Sample Findings

* Sysmon Event ID 1: Process Creation
* Sysmon Event ID 11: File Creation
* Windows Service Configuration Changes
* CVE Detection Through Wazuh Vulnerability Scanner
* MITRE ATT&CK Technique Mapping

## Future Goals

Continue expanding the lab to simulate real-world enterprise security operations, validate detections using Atomic Red Team, and develop practical incident response workflows.
