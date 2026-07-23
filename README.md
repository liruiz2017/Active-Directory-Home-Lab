# Active Directory Home Lab

## Overview

This project demonstrates the deployment and administration of a Windows Active Directory environment using **Windows Server 2022** and **Windows 11 Enterprise** in **VMware Fusion**. The lab simulates a small business network by implementing centralized authentication, Organizational Units (OUs), security groups, Group Policy Objects (GPOs), shared folders, NTFS permissions, and PowerShell automation.

The goal of this project was to gain hands-on experience with technologies commonly used by Windows System Administrators, IT Support Specialists, Cloud Engineers, and Cybersecurity professionals.

---

# Technologies Used

## Operating Systems

- Windows Server 2022 Standard
- Windows 11 Enterprise Evaluation

## Microsoft Technologies

- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management
- SMB File Sharing
- NTFS Permissions
- Windows PowerShell

## Virtualization

- VMware Fusion

## Version Control

- Git
- GitHub

---

# Lab Environment

| Component | Configuration |
|-----------|---------------|
| Hypervisor | VMware Fusion |
| Server OS | Windows Server 2022 Standard |
| Client OS | Windows 11 Enterprise Evaluation |
| Domain Name | ruizlab.local |
| Domain Controller | DC1 |
| Client Computer | PC01 |

---

# Project Objectives

- Deploy a Windows Server 2022 Domain Controller
- Install Active Directory Domain Services
- Configure DNS
- Create Organizational Units
- Create domain users
- Create security groups
- Join Windows 11 to the domain
- Configure departmental file shares
- Configure NTFS permissions
- Deploy Group Policy
- Automate administrative tasks with PowerShell
- Document the project using GitHub

---

# Features Implemented

## Active Directory

- Installed Active Directory Domain Services (AD DS)
- Created the **ruizlab.local** domain
- Configured DNS
- Created Organizational Units
- Created domain users
- Created security groups
- Verified successful domain authentication

---

## Windows Client Administration

- Installed Windows 11 Enterprise
- Renamed workstation to **PC01**
- Joined workstation to the Active Directory domain
- Verified successful domain login

---

## File Server

Created departmental shared folders for:

- Finance
- HR
- IT
- Sales

Configured:

- Share Permissions
- NTFS Permissions

Verified:

- Authorized user access
- Unauthorized access restrictions

---

## Group Policy

Created and deployed a custom Group Policy Object that disables the Windows Control Panel for users within the IT Organizational Unit.

Verified using:

- `gpupdate /force`
- `gpresult /r`

---

## PowerShell Automation

Completed administrative tasks using the Active Directory PowerShell module.

Tasks included:

- Query Active Directory users
- Create users
- Add users to security groups
- Disable user accounts
- Enable user accounts
- Export Active Directory reports to CSV

---

# Repository Structure

```text
Active-Directory-Home-Lab/
│
├── README.md
├── documentation/
│   ├── active-directory.md
│   ├── day1-journal.md
│   ├── day2-journal.md
│   ├── file-server.md
│   ├── group-policy.md
│   ├── lessons-learned.md
│   ├── powershell.md
│   ├── project-summary.md
│   ├── screenshots.md
│   └── troubleshooting.md
│
├── screenshots/
│   ├── active-directory/
│   ├── file-server/
│   ├── group-policy/
│   └── powershell/
│
└── diagrams/
```

---

# Documentation

This repository contains detailed documentation for every stage of the project, including:

- Active Directory deployment
- File Server configuration
- Group Policy implementation
- PowerShell automation
- Troubleshooting
- Lessons learned
- Daily project journal
- Screenshot walkthrough
- Project summary

---

# Skills Demonstrated

- Windows Server Administration
- Active Directory Administration
- DNS Configuration
- Group Policy Management
- User & Group Administration
- Windows Domain Management
- File Server Administration
- NTFS Permissions
- SMB File Sharing
- PowerShell Automation
- VMware Virtualization
- Git Version Control
- GitHub Documentation
- Troubleshooting

---

# Lessons Learned

Building this environment from the ground up provided valuable experience with enterprise Windows administration. Throughout the project, I gained hands-on experience deploying Active Directory, configuring DNS, managing users and groups, implementing Group Policy, securing file shares, and automating administrative tasks with PowerShell.

In addition to strengthening my technical skills, this project reinforced the importance of documentation, troubleshooting, and version control when managing enterprise environments.

---

# Future Improvements

Future enhancements may include:

- Windows Server Update Services (WSUS)
- Active Directory Certificate Services (AD CS)
- DHCP Server
- Login Scripts
- Drive Mapping with Group Policy
- Group Policy Security Hardening
- Backup and Recovery
- Multi-Domain Forest
- Additional PowerShell automation

---

# Author

**Luis Ruiz**

Bachelor of Science in Information Technology

CompTIA Security+ (In Progress)

AWS SysOps Administrator Associate (In Progress)

---

# License

This project is intended for educational and portfolio purposes.