# PowerShell Automation

## Overview

This lab demonstrates the use of the Active Directory PowerShell module to automate administrative tasks.

---

## Module Used

```powershell
Import-Module ActiveDirectory
```

---

## Tasks Completed

- Query Active Directory users
- Create a new user
- Add a user to a security group
- Disable a user account
- Enable a user account
- Export Active Directory users to CSV

---

## Cmdlets Used

| Task | Cmdlet |
|------|---------|
| List Users | Get-ADUser |
| Create User | New-ADUser |
| Add User to Group | Add-ADGroupMember |
| View Group Members | Get-ADGroupMember |
| Disable Account | Disable-ADAccount |
| Enable Account | Enable-ADAccount |
| Export Report | Export-Csv |

---

## Example Commands

```powershell
Get-ADUser -Filter *

New-ADUser

Add-ADGroupMember

Disable-ADAccount

Enable-ADAccount

Export-Csv
```

---

## Skills Demonstrated

- Active Directory Automation
- User Management
- Group Management
- PowerShell Scripting
- Administrative Reporting