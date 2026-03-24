# Lateral Movement & Privilege Escalation Investigation

## Overview

This project simulates a post-compromise scenario in an Active Directory environment, focusing on how attackers perform lateral movement and expand their access within a network.

The investigation analyzes common techniques attackers use after initial access, including credential reuse, remote execution, and pivoting through compromised hosts.

## Investigation Focus

The analysis explored:

- Lateral movement techniques inside Active Directory
- Remote command execution using PsExec
- Authentication mechanisms (NTLM and Kerberos)
- Pivoting techniques using SSH tunneling
- Credential reuse across systems

## Key Techniques Analyzed

### Remote Execution (PsExec)

Attackers can remotely execute commands on target systems by:

- Connecting via SMB (Port 445)
- Uploading a service binary
- Executing commands through remote services

### Authentication Abuse

The investigation examines:

- NTLM authentication reuse
- Kerberos ticket-based authentication

These mechanisms can enable attackers to authenticate across systems once credentials are compromised.

### Network Pivoting

Attackers may use compromised hosts to access restricted systems by creating tunnels that bypass network restrictions.

## SOC Analyst Perspective

To mitigate these risks, organizations should:

- Restrict administrative privileges
- Monitor abnormal lateral movement
- Detect unusual SMB, RDP, or WinRM activity
- Monitor PsExec usage
- Implement network segmentation

## Full Investigation Report

[Download Full Investigation Report](./lateral-movement-investigation.odt)
