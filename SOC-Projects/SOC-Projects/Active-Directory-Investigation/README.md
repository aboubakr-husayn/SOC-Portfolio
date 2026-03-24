# Active Directory Compromise Investigation

## Overview
This project presents a SOC-style investigation into a potential compromise of an Active Directory (AD) environment. The investigation focuses on how attackers obtain initial access using compromised credentials and how that access can be used to enumerate the domain.

## Investigation Focus
The investigation analyzes:

- Initial access through credential compromise
- Authentication abuse (NTLM / LDAP)
- Network-based credential attacks
- Internal Active Directory enumeration

## Key Concepts Demonstrated

- Credential-based attacks
- NTLM / NetNTLM authentication abuse
- LLMNR / NBT-NS poisoning
- Domain enumeration techniques
- Active Directory structure analysis

## Impact
The investigation shows that even low-privileged credentials can expose significant information about:

- Domain users
- Organizational Units
- Group permissions
- Domain-joined systems

This information enables attackers to plan privilege escalation and lateral movement.

