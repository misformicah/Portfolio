Problems Encountered and Resolutions

1. Wazuh Agent Not Showing Data
Problem

The Windows 11 endpoint appeared connected to Wazuh, but events were not appearing in the dashboard.

Troubleshooting
Verified Wazuh agent service was running.
Checked agent registration status on the Wazuh manager.
Reviewed Wazuh agent logs.
Confirmed agent and manager could communicate over the network.
Verified correct manager IP address configuration.
Resolution
Corrected agent configuration and restarted services.
Confirmed the Windows endpoint successfully registered and began sending logs.
Skills Demonstrated
Endpoint monitoring
Agent management
Log verification

2. Sysmon XML Configuration Would Not Load
Problem

Sysmon installation returned an error indicating the XML configuration file could not be opened.

Troubleshooting
Verified Sysmon executable location.
Verified XML file download.
Checked file path syntax.
Confirmed command prompt was running as administrator.
Resolution
Corrected file path and installation command.
Successfully installed Sysmon with the community configuration file.
Skills Demonstrated
Windows administration
Endpoint telemetry configuration

3. Sysmon Events Not Appearing in Wazuh
Problem

Sysmon was running locally but events did not immediately appear in Wazuh.

Troubleshooting
Verified Sysmon service status.
Generated test activity using PowerShell and file creation.
Examined Windows Event Viewer.
Searched Wazuh threat hunting dashboard for Sysmon event IDs.
Resolution
Confirmed Sysmon events were being collected through Windows Event Channels.
Verified Wazuh ingestion and alert generation.
Skills Demonstrated
Threat hunting
Event log analysis
Windows security monitoring

4. Confusion Between Windows Events and Sysmon Events
Problem

Many detections appeared in Wazuh, but it was unclear whether they originated from Sysmon or standard Windows logs.

Troubleshooting
Opened raw event details.
Reviewed provider names.
Checked Event IDs.
Compared Sysmon Operational logs against Windows Event Channel logs.
Resolution
Identified Sysmon events by:
Provider: Microsoft-Windows-Sysmon
Event IDs such as:
Event ID 1 (Process Creation)
Event ID 11 (File Creation)
Skills Demonstrated
Threat hunting
Log source validation

5. Vulnerability Detection Validation
Problem

Needed to verify Wazuh vulnerability detection functionality.

Troubleshooting
Examined vulnerability dashboard.
Reviewed vulnerability-detection logs.
Validated package inventory collection.
Resolution
Confirmed Wazuh identified active Windows vulnerabilities including:
CVE-2026-21513
CVE-2026-32077
Skills Demonstrated
Vulnerability management
CVE analysis

6. Suricata Installed but No Alerts Generated
Problem

Suricata was running but the Alerts tab remained empty.

Troubleshooting
Verified Suricata service status.
Verified ET Open rules downloaded successfully.
Examined Alerts tab.
Examined Logs View.
Findings
No alerts present.
No alert events present in eve.json.
Resolution

Continued investigation into logging and rule configuration.

Skills Demonstrated
IDS troubleshooting
Security monitoring validation

7. Suricata Logging Not Enabled
Problem

Logs View reported:

Log file does not exist

Troubleshooting
Examined Suricata logging configuration.
Reviewed EVE output settings.
Resolution

Enabled:

EVE JSON Logging
Alert logging
DNS logging
HTTP logging
TLS logging

After restarting Suricata, eve.json began collecting traffic.

Skills Demonstrated
IDS configuration
Security telemetry collection

8. Traffic Appeared in EVE but No Alerts Generated
Problem

eve.json contained traffic events but no alert events.

Troubleshooting
Searched eve.json for:
event_type: alert
Verified alert logging enabled.
Verified ET Open rules installed.
Examined Suricata startup logs.
Findings
Traffic was visible.
No signatures were firing.
Skills Demonstrated
IDS log analysis
Signature troubleshooting

9. Limited Rule Coverage
Problem

Suricata loaded only 666 signatures.

Troubleshooting
Examined Categories page.
Reviewed enabled rule categories.
Examined suricata.log startup messages.
Findings

Suricata reported:

666 signatures processed

Only a small number of rule categories were enabled:

emerging-scan.rules
ssh-events.rules
stream-events.rules
tls-events.rules
Resolution

Enabled additional rule categories including:

emerging-malware.rules
emerging-exploit.rules
emerging-policy.rules
emerging-attack_response.rules
emerging-shellcode.rules
emerging-info.rules

Applied changes and restarted Suricata.

Skills Demonstrated
Signature management
IDS tuning

10. Nmap Detection Validation
Problem

Initial Nmap scans generated no alerts.

Troubleshooting
Ran Nmap scans from Kali.
Verified traffic visibility.
Examined ARP tables.
Investigated network path.
Reviewed Suricata rule loading.
Generated additional test traffic.
Resolution

After enabling additional rule categories and reloading Suricata:

ET HUNTING alerts generated.
GPL ATTACK_RESPONSE alerts generated.
Nmap reconnaissance activity became detectable.
Skills Demonstrated
Adversary simulation
IDS validation
Detection engineering
Lessons Learned
Endpoint Visibility

Sysmon provides significantly more detailed telemetry than default Windows logging.

Detection Validation

A security tool being installed does not guarantee detections are functioning.

Rule Management

IDS effectiveness depends heavily on properly enabling and validating rule categories.

Log Analysis

Raw logs are often more useful for troubleshooting than dashboard summaries.

Threat Hunting

Investigating individual events helps validate data sources and detection coverage.

Security Operations

Building a functioning SOC lab requires:

Network monitoring
Endpoint monitoring
Vulnerability management
IDS management
Threat hunting
Troubleshooting and validation

