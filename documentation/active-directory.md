# Active Directory Lab

## Overview

This project demonstrates the deployment of a Windows Active Directory environment using Windows Server 2022 and a Windows 11 Enterprise client. The lab simulates a small business network by implementing centralized authentication, Organizational Units (OUs), security groups, domain-joined workstations, Group Policy, file sharing, and PowerShell administration.

---

## Lab Environment

| Component | Configuration |
|-----------|---------------|
| Hypervisor | VMware Fusion |
| Server OS | Windows Server 2022 Standard |
| Client OS | Windows 11 Enterprise Evaluation |
| Domain Name | ruizlab.local |
| Domain Controller | DC1 |
| Client Computer | PC01 |

---

## Organizational Unit Structure

```
ruizlab.local
│
├── Finance
├── HR
├── IT
│   ├── Users
│   └── Groups
├── Sales
├── Servers
├── Server Accounts
├── Workstations
└── PowerShell Lab
```

---

## Users Created

| Name | Username | Department |
|------|----------|------------|
| John Smith | jsmith | IT |
| Sarah Davis | sdavis | IT |
| Emily Brown | ebrown | Finance |
| Mike Johnson | mjohnson | HR |
| Lisa Garcia | lgarcia | Sales |
| Alex Rivera | arivera | PowerShell Lab |

---

## Security Groups

| Group | Purpose |
|---------|----------|
| IT Admins | Administrative users for the IT department |

---

## Domain Join Process

The Windows 11 client (PC01) was joined to the **ruizlab.local** domain by:

1. Configuring the DNS server to point to DC1.
2. Renaming the computer to PC01.
3. Joining the Active Directory domain.
4. Restarting the workstation.
5. Logging in using a domain account.
6. Verifying authentication using:

```
whoami
hostname
echo %USERDOMAIN%
```

---

## Skills Demonstrated

- Active Directory Domain Services (AD DS)
- DNS Configuration
- Organizational Unit Management
- User Administration
- Security Groups
- Domain Join
- Windows Server Administration