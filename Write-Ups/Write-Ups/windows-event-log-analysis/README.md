Windows Event Log Analysis – Suspicious PowerShell Activity Investigation
Executive Summary

Windows Event Logs provide critical visibility into system activity and are widely used by Security Operations Center (SOC) analysts to investigate potential security incidents.

During routine log review, PowerShell activity was identified within the Microsoft-Windows-PowerShell/Operational event log channel. PowerShell logging provides detailed visibility into executed commands and is an important source of forensic evidence during incident investigations.

Initial analysis identified Event ID 4103 as the earliest PowerShell operational event. Further investigation focused on Event ID 4104, which captures PowerShell script block execution and reveals commands executed during a PowerShell session.

Log filtering revealed the command whoami, which is commonly used to identify the currently logged-in user and associated privileges. The event metadata categorized this action as “Execute a Remote Command.”

Although the command itself is not malicious, enumeration commands such as whoami frequently appear during the reconnaissance phase of cyber attacks, making this activity relevant from a security perspective.

This investigation demonstrates how Windows event log analysis can help SOC analysts reconstruct system activity and identify potentially suspicious behavior.
