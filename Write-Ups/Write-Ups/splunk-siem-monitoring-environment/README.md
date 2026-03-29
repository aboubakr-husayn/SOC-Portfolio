Building a SOC Monitoring Environment Using Splunk SIEM
Overview

Security Operations Centers (SOC) rely on centralized monitoring platforms to detect suspicious activity, investigate incidents, and maintain visibility across enterprise environments. Security Information and Event Management (SIEM) solutions enable security teams to collect, index, and analyze logs from multiple systems in a centralized platform.

This investigation demonstrates the deployment of a SOC monitoring environment using Splunk Enterprise. The objective was to build a SIEM infrastructure capable of ingesting logs from both Linux and Windows systems and enabling centralized monitoring of security events.

The lab simulated how SOC teams collect logs from endpoints, forward them to a central SIEM platform, and perform security investigations using searchable log data.

Key Findings

• Splunk Enterprise successfully deployed as a centralized SIEM server
• Splunk Universal Forwarders installed on endpoint systems
• Linux system logs and Windows Event Logs successfully collected
• Logs transmitted to the SIEM server through port 9997
• Events indexed and searchable within the Splunk platform

Tools Used
Splunk Enterprise
Splunk Universal Forwarder
Linux Syslog
Windows Event Logs
Investigation Focus
SIEM Deployment
Log Collection Architecture
Endpoint Log Forwarding
Centralized Security Monitoring
Event Indexing and Search
SOC Monitoring Architecture
Component	Function
Splunk Enterprise	Log indexing and security event analysis
Universal Forwarder	Log collection from endpoints
Linux Syslog	Monitoring Linux system activity
Windows Event Logs	Monitoring Windows endpoint activity

This architecture simulates a basic SOC monitoring pipeline where endpoint logs are forwarded to a centralized SIEM server for indexing and analysis.

Skills Demonstrated
SIEM Deployment
Log Ingestion Configuration
SOC Monitoring Architecture
Security Log Analysis

## Full Investigation Report
The complete technical investigation report with detailed steps, screenshots, and configuration details is available in the document included in this repository.
➡ splunk-siem-monitoring-environment, write-up.docx
