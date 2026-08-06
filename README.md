# Enterprise Active Directory Deployment & Security Audit

> A hands-on enterprise Active Directory deployment built using Windows Server 2022, featuring Organizational Unit (OU) design, Group Policy Object (GPO) hardening, PowerShell administration, Windows 11 domain integration, and a security assessment using Kali Linux.

---

## Project Overview

This project demonstrates the end-to-end deployment and administration of an Enterprise Active Directory environment in a virtualized lab.

The objective was to simulate a real-world corporate network where users, departments, and systems are centrally managed through Microsoft's Active Directory Domain Services (AD DS). The project focuses on implementing enterprise administration practices, configuring security policies, automating administrative tasks through PowerShell, and validating the environment from a security perspective using Kali Linux.

Unlike a basic Active Directory setup, this project emphasizes organizational structure, security hardening, administrative efficiency, and documentation to reflect enterprise-level practices.

---

# Project Objectives

- Deploy Windows Server 2022 as an Active Directory Domain Controller.
- Configure a new Active Directory Forest and Domain.
- Design Organizational Units (OUs) representing enterprise departments.
- Create and manage domain users and security groups.
- Join Windows 11 client machines to the domain.
- Configure Group Policy Objects (GPOs) for centralized administration.
- Perform PowerShell-based administration and auditing.
- Conduct a security assessment using Kali Linux.
- Document the complete deployment process.

---

# Lab Environment

| Component | Details |
|------------|---------|
| Hypervisor | VMware Workstation |
| Server Operating System | Windows Server 2022 |
| Client Operating System | Windows 11 |
| Security Testing Machine | Kali Linux |
| Domain Services | Active Directory Domain Services (AD DS) |
| Management Tools | Group Policy Management Console, Active Directory Users & Computers, PowerShell |
| Networking | Virtual Network |

---

# Enterprise Architecture

The project consists of the following virtual infrastructure:

```
                    Internet
                        │
                Virtual Network
                        │
        ┌─────────────────────────┐
        │ Windows Server 2022     │
        │ Domain Controller        │
        │ DNS Server               │
        │ Active Directory         │
        └──────────┬───────────────┘
                   │
      ┌────────────┴────────────┐
      │                         │
 Windows 11 Client 1      Windows 11 Client 2
      │                         │
      └────────────┬────────────┘
                   │
               Kali Linux
          Security Assessment
```

---

# Active Directory Structure

The Active Directory environment was organized using Organizational Units (OUs) to simulate an enterprise hierarchy.

```
abc.local
│
├── Domain Controllers
│
└── ABC-Technologies
    │
    ├── Security
    │
    ├── IT
    │
    └── Cloud Operations
```

This hierarchy enables:

- Department-based management
- Simplified administration
- Delegation of administrative privileges
- Group Policy targeting
- Scalable enterprise management

---

# Features Implemented

## Active Directory Deployment

- Installed Active Directory Domain Services (AD DS)
- Promoted server to Domain Controller
- Configured new forest
- Configured DNS
- Verified domain functionality

---

## Organizational Unit (OU) Management

Created enterprise Organizational Units representing different departments.

Example:

- Security
- IT
- Cloud Operations

This organizational structure enables centralized administration and policy enforcement.

---

## User Management

Configured multiple domain users representing different departments.

Tasks performed include:

- User creation
- Department assignment
- Password configuration
- Account management
- Administrative verification

---

## Windows Client Integration

Two Windows 11 virtual machines were successfully joined to the Active Directory domain.

Verified:

- Domain authentication
- User logon
- Group Policy application
- Centralized management

---

## Group Policy Hardening

Implemented centralized security policies using Group Policy Objects (GPOs).

Examples include:

- Password Policy
- User Restrictions
- Administrative Controls
- Centralized Configuration Management

Group Policies ensure consistent security configuration across domain-joined systems.

---

## PowerShell Administration

PowerShell was extensively used for administrative verification and automation.

Examples include:

```powershell
Get-ADDomain

Get-ADOrganizationalUnit

Get-ADUser

Get-ADGroup
```

PowerShell simplifies enterprise administration while providing repeatable management operations.

---

## Security Assessment

A Kali Linux virtual machine was used to perform basic security validation against the deployed Active Directory environment.

Activities included:

- Host discovery
- Network enumeration
- Service identification
- Security verification

The objective was to understand the security posture of the deployed environment from an attacker's perspective.

---

# Technologies Used

- Windows Server 2022
- Active Directory Domain Services
- DNS
- Organizational Units
- Group Policy Objects (GPO)
- PowerShell
- Windows 11
- VMware Workstation
- Kali Linux

---

# Skills Demonstrated

This project demonstrates practical experience in:

- Enterprise Active Directory Administration
- Windows Server Deployment
- Organizational Unit Design
- User Administration
- Domain Management
- PowerShell Administration
- Group Policy Management
- Windows Administration
- Security Hardening
- Virtualization
- Documentation
- Network Administration
- Security Assessment Fundamentals

---

# Screenshots

Project screenshots are available inside the **screenshots/** directory.

They include:

- Domain Controller Configuration
- Organizational Unit Creation
- User Management
- PowerShell Administration
- Windows Client Domain Join
- Group Policy Configuration
- Kali Linux Assessment

---

# Documentation

Complete project documentation is available in the **documentation/** directory.

The documentation includes:

- Deployment Procedure
- Architecture
- Configuration Steps
- Security Configuration
- Administrative Tasks
- Validation Process

---

# Learning Outcomes

Through this project I gained practical experience in:

- Enterprise Windows Administration
- Active Directory Deployment
- Organizational Unit Design
- Group Policy Management
- PowerShell Administration
- Windows Domain Architecture
- Enterprise Security Concepts
- Security Validation Techniques
- Technical Documentation

---

# Future Improvements

Potential enhancements include:

- Windows Server Update Services (WSUS)
- File Server Deployment
- DHCP Configuration
- Print Server
- BitLocker Management
- LAPS Implementation
- Microsoft Defender Policies
- SIEM Integration
- Microsoft Entra ID Hybrid Join
- Azure Active Directory Integration
- Security Monitoring
- Domain Backup Strategy

---

# Repository Structure

```
enterprise-active-directory-security-audit
│
├── documentation/
├── screenshots/
├── scripts/
├── assets/
└── README.md
```

---

# Disclaimer

This project was developed in a controlled virtual lab environment strictly for educational and learning purposes.

No production systems or third-party infrastructure were targeted during the security assessment.

---

# Author

**Abhinav Banerjee**

BCA Student | Cybersecurity Enthusiast

Specializing in:

- Windows Administration
- Active Directory
- Networking
- Cybersecurity
- Security Operations
- PowerShell

---

If you found this project interesting, feel free to connect with me on LinkedIn or explore my other repositories.
