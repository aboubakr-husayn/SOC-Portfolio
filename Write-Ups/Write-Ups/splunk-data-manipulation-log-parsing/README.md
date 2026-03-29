Splunk Data Manipulation – Log Parsing and Data Processing
Overview

Security Information and Event Management (SIEM) platforms such as Splunk rely on properly structured log data to enable efficient searching, correlation, and investigation. When logs are not correctly parsed during ingestion, security analysts may struggle to analyze events or detect suspicious activity.

This investigation focuses on improving Splunk’s ability to process raw log data through parsing and configuration techniques. Several SIEM engineering tasks were performed, including event breaking, multi-line log handling, sensitive data masking, and custom log ingestion.

The lab demonstrates how SOC teams structure incoming log data to ensure it can be efficiently analyzed and used for security monitoring and threat detection.

Key Findings

• Custom Splunk application (DataApp) created for log ingestion
• Sample log events generated using a Python script
• Automated log ingestion configured using inputs.conf
• Event breaking implemented using props.conf
• Sensitive information protected using SEDCMD data masking

Tools Used
Splunk Enterprise
Splunk Configuration Files
Python (Log Generation Script)
Linux Environment
Investigation Focus
Log Ingestion Configuration
Event Breaking and Parsing
Multi-line Log Handling
Sensitive Data Masking
SIEM Log Processing
Skills Demonstrated
SIEM Data Engineering
Log Parsing and Processing
Splunk Configuration Management
Security Log Preparation for Analysis

## Full Investigation Report
The complete technical investigation report with detailed configuration steps, screenshots, and log parsing examples is available in the document included in this repository.
➡ splunk-data-manipulation-log-parsing write-up.docx
