# Project Summary

## Active Directory Home Lab

### Project Overview

The Active Directory Home Lab is a hands-on Windows Server 2022 project designed to simulate a small enterprise network. The primary objective was to gain practical experience deploying, configuring, and managing Microsoft Active Directory while developing skills commonly used by Systems Administrators, IT Support Specialists, and Cybersecurity professionals.

The environment was built entirely within VMware Fusion using a Windows Server 2022 Domain Controller and a Windows 11 Enterprise client. Throughout the project, enterprise services including Active Directory Domain Services (AD DS), DNS, Group Policy, SMB file sharing, NTFS permissions, and PowerShell automation were implemented and tested.

---

## Objectives

- Deploy a Windows Server 2022 Domain Controller.
- Install and configure Active Directory Domain Services (AD DS).
- Configure DNS for domain services.
- Create Organizational Units (OUs).
- Create and manage domain users and security groups.
- Join a Windows 11 workstation to the Active Directory domain.
- Configure and secure departmental file shares.
- Deploy and verify Group Policy Objects (GPOs).
- Automate common administrative tasks using PowerShell.
- Document the complete deployment process using GitHub.

---

## Technologies Used

### Operating Systems

- Windows Server 2022 Standard
- Windows 11 Enterprise Evaluation

### Virtualization

- VMware Fusion

### Microsoft Technologies

- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management
- SMB File Sharing
- NTFS Permissions
- Windows PowerShell

### Version Control

- Git
- GitHub

---

## Features Implemented

### Active Directory

- Installed Active Directory Domain Services.
- Created the **ruizlab.local** domain.
- Configured DNS.
- Created Organizational Units.
- Created domain users.
- Created security groups.

---

### Windows Client Administration

- Installed Windows 11 Enterprise.
- Renamed the workstation to **PC01**.
- Joined the workstation to the Active Directory domain.
- Verified domain authentication.

---

### File Server

Created departmental shared folders for:

- Finance
- HR
- IT
- Sales

Configured:

- Share Permissions
- NTFS Permissions

Verified:

- Authorized user access.
- Unauthorized access restrictions.

---

### Group Policy

Implemented a custom Group Policy Object that disabled access to the Windows Control Panel for users within the IT Organizational Unit.

Verified successful deployment using:

- `gpupdate /force`
- `gpresult /r`

---

### PowerShell Automation

Automated several administrative tasks including:

- Querying Active Directory users.
- Creating new user accounts.
- Managing security group membership.
- Disabling user accounts.
- Re-enabling user accounts.
- Exporting Active Directory reports to CSV.

---

## Challenges Encountered

During the project, several technical challenges were encountered and resolved, including:

- VMware installation and boot configuration.
- DNS configuration preventing successful domain joins.
- Group Policy troubleshooting.
- File share permission configuration.
- PowerShell syntax and cmdlet troubleshooting.
- Git and GitHub repository setup and synchronization.

Resolving these issues provided valuable troubleshooting experience and strengthened understanding of Windows Server administration.

---

## Skills Demonstrated

- Active Directory Administration
- Windows Server Administration
- DNS Configuration
- Group Policy Management
- User and Group Administration
- File Server Administration
- NTFS Permissions
- PowerShell Automation
- Windows Client Management
- Virtualization
- Git Version Control
- GitHub Documentation
- Troubleshooting
- Technical Documentation

---

## Lessons Learned

This project reinforced the importance of centralized identity management, proper permission assignment, and automation within enterprise environments. Building the environment from the ground up provided practical experience with Active Directory deployment, DNS, Group Policy, Windows administration, and PowerShell automation.

In addition to technical skills, documenting the project throughout development highlighted the importance of maintaining clear documentation, version control, and reproducible deployment processes.

---

## Future Improvements

Future enhancements to this environment may include:

- DHCP Server
- Windows Server Update Services (WSUS)
- Active Directory Certificate Services (AD CS)
- Group Policy security hardening
- Login scripts
- Drive mapping using Group Policy
- Backup and recovery solutions
- Multi-Domain Active Directory Forest
- Additional PowerShell automation scripts

---

## Conclusion

This project successfully demonstrates the deployment and administration of a Windows Active Directory environment using enterprise technologies commonly found in production networks. It provided practical experience in system administration, identity management, troubleshooting, and automation while reinforcing best practices for documentation and version control.

The completed project serves as a portfolio example of hands-on experience with Microsoft enterprise technologies and reflects skills applicable to entry-level IT, Systems Administration, Cloud Support, and Cybersecurity roles.