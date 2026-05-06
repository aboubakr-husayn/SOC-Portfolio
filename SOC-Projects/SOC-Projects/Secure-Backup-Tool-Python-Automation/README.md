# Secure Backup Tool | Python Automation Project

## Project Overview

The Secure Backup Tool is a Python automation project designed to create secure and verifiable file backups using ZIP compression, SHA-256 integrity verification, and persistent logging.

The project was developed step-by-step, starting from a simple folder exploration script and evolving into a complete backup solution capable of compressing files, generating cryptographic hashes, and maintaining an audit trail of all backup operations.

---

## Project Objectives

- Scan and list files inside a target directory
- Create automated timestamped ZIP backups
- Generate SHA-256 hashes for integrity verification
- Detect backup corruption or tampering
- Maintain persistent backup logs for auditing purposes

---

## Tools & Technologies

- Python
- pathlib
- shutil
- zipfile
- hashlib
- logging
- Visual Studio Code

---

## Project Stages

### Stage 1 — Folder Explorer

A folder exploration script (`explore.py`) was created to:

- Scan all files and directories
- Display file names and file sizes
- Calculate total folder size
- Verify folder structure before backup operations

---

### Stage 2 — Initial Backup System

The first backup version implemented:

- Automated folder backups
- Timestamped backup naming
- Backup directory creation using Python

---

### Stage 3 — ZIP Compression & SHA-256 Hashing

The backup system was upgraded to include:

- ZIP archive compression
- SHA-256 cryptographic hashing
- Integrity verification using `.sha256` files

This stage improved both security and storage efficiency.

---

### Stage 4 — Final Version with Logging

The final implementation added:

- Persistent logging using Python’s `logging` module
- Backup metadata recording
- Timestamped audit logs
- File count and backup size tracking
- SHA-256 hash logging

All backup activities are recorded inside `backup_log.txt`.

---

## Security Features

### SHA-256 Integrity Verification

The tool generates a SHA-256 hash for every backup archive.

This provides:

- Integrity verification
- Tamper detection
- Corruption detection
- Audit trail creation

Any modification to the backup archive changes the SHA-256 hash completely.

---

## Features Implemented

- Automated ZIP backup creation
- Timestamped backup naming
- SHA-256 hash generation
- Companion `.sha256` file creation
- Persistent backup logging
- File count reporting
- Backup size tracking

---

## Python Concepts Demonstrated

- File handling
- Directory traversal
- ZIP compression
- Cryptographic hashing
- Logging systems
- Automation scripting
- Modular development

---

## SOC & Security Relevance

This project demonstrates practical cybersecurity and automation concepts related to:

- Backup integrity verification
- Secure automation
- File monitoring
- Audit logging
- Basic security controls
- Security-focused scripting

---

## Full Project Report

📄 [Download Full Report](https://github.com/aboubakr-husayn/SOC-Portfolio/blob/main/SOC-Projects/SOC-Projects/Secure-Backup-Tool-Python-Automation/Secure%20Backup%20Tool%20project.docx)

---

## Conclusion

This project demonstrates how Python can be used to automate secure backup operations while ensuring integrity verification through SHA-256 hashing and maintaining a persistent audit trail using logging.

The implementation highlights practical scripting, automation, and security-focused development skills relevant to cybersecurity and IT operations.
