Windows Event Log Analysis – Suspicious PowerShell Activity Investigation
Overview

This investigation analyzes Windows Event Logs to identify suspicious PowerShell activity that may indicate potential reconnaissance behavior.

During routine log review, PowerShell activity was identified within the Microsoft-Windows-PowerShell/Operational event log channel. Analysis focused on Event ID 4103 (PowerShell pipeline execution) and Event ID 4104 (PowerShell script block logging).

Further inspection revealed execution of the whoami command, which is commonly used to determine the current user context and privileges. The event metadata categorized this action as “Execute a Remote Command.”

Although the command itself is not malicious, enumeration commands such as whoami frequently appear during the reconnaissance phase of cyber attacks, making the activity relevant from a security monitoring perspective.

Key Findings

• PowerShell pipeline execution detected (Event ID 4103)
• Script block logging exposed executed commands (Event ID 4104)
• Enumeration command whoami executed during the PowerShell session
• Activity categorized as Execute a Remote Command
• Investigation classified the behavior as Suspicious – Requires Further Validation

Tools Used
Windows Event Viewer
Windows Event Logs
PowerShell Operational Logs
Investigation Focus
Windows Event Log Analysis
PowerShell Script Block Logging
Command Execution Investigation
Suspicious Activity Detection
