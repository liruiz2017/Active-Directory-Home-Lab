# Screenshot Walkthrough

This document provides an explanation of each screenshot included in the Active Directory Home Lab project. The screenshots demonstrate the deployment, configuration, testing, and administration of a Windows Server 2022 Active Directory environment.

---

# Active Directory

## 01 - Server Manager Initial Configuration

![Server Manager](../screenshots/active-directory/01-server-manager-initial-configuration.png)

**Description**

This screenshot shows the initial Windows Server 2022 installation before Active Directory Domain Services (AD DS) was installed. Server Manager was used to verify the server configuration and prepare the server for promotion to a Domain Controller.

**Skills Demonstrated**

- Windows Server Administration
- Server Manager
- Initial Server Configuration

---

## 02 - Domain Controller Configured

![Domain Controller](../screenshots/active-directory/02-domain-controller-configured.png)

**Description**

The Windows Server 2022 system was successfully promoted to a Domain Controller for the **ruizlab.local** domain. Active Directory Domain Services and DNS were installed and configured.

**Skills Demonstrated**

- Active Directory Domain Services
- DNS
- Domain Controller Deployment

---

## 03 - Organizational Unit Structure

![OU Structure](../screenshots/active-directory/03-ou-structure.png)

**Description**

Organizational Units (OUs) were created to organize users, computers, and administrative resources by department. This structure allows policies and permissions to be managed efficiently.

**Skills Demonstrated**

- Organizational Units
- Active Directory Administration
- Enterprise Organization

---

## 04 - User Account Creation

![User Created](../screenshots/active-directory/04-user-created.png)

**Description**

Department user accounts were created within Active Directory Users and Computers. These accounts are used for authentication and centralized user management.

**Skills Demonstrated**

- User Administration
- Identity Management
- Active Directory

---

## 05 - Finance Security Group

![Security Group](../screenshots/active-directory/05-finance-security-group.png)

**Description**

Security groups were created to simplify permission management by assigning permissions to groups instead of individual users.

**Skills Demonstrated**

- Security Groups
- Role-Based Access Control (RBAC)
- Active Directory Administration

---

## 06 - First Domain Login

![Domain Login](../screenshots/active-directory/06-first-domain-user-login.png)

**Description**

The Windows 11 workstation successfully authenticated to the Active Directory domain using domain credentials.

**Skills Demonstrated**

- Domain Authentication
- Windows 11 Domain Join

---

## 07 - Domain Login Verification

![Verification](../screenshots/active-directory/07-domain-login-verification.png)

**Description**

Commands including `whoami`, `hostname`, and `echo %USERDOMAIN%` verified that the workstation was authenticated to the **ruizlab.local** domain.

**Skills Demonstrated**

- Authentication Verification
- Windows Command Line
- Active Directory

---

## 08 - Workstation Organizational Unit

![Workstation OU](../screenshots/active-directory/08-workstation-ou.png)

**Description**

The Windows 11 workstation (PC01) was moved into the Workstations Organizational Unit to allow centralized administration and Group Policy deployment.

**Skills Demonstrated**

- Computer Object Management
- Organizational Units
- Active Directory Administration

---

# File Server

## 01 - Shared Folders Created

![Shared Folders](../screenshots/file-server/01-shared-folders-created.png)

**Description**

Departmental shared folders were created for Finance, HR, IT, and Sales to simulate a production file server.

**Skills Demonstrated**

- Windows File Server
- SMB Shares
- Shared Folder Administration

---

## 02 - HR Access Denied

![Access Denied](../screenshots/file-server/02-hr-access-denied.png)

**Description**

An unauthorized user attempted to access the HR shared folder and correctly received an Access Denied message.

**Skills Demonstrated**

- NTFS Permissions
- Access Control
- Security Validation

---

## 03 - IT Share Access Success

![IT Share](../screenshots/file-server/03-it-share-access-success.png)

**Description**

An authorized user successfully accessed the IT shared folder, confirming that share and NTFS permissions were configured correctly.

**Skills Demonstrated**

- File Sharing
- Permission Management
- Windows Server Administration

---

# Group Policy

## 01 - GPO Linked

![GPO Linked](../screenshots/group-policy/01-domain-security-policy-linked.png)

**Description**

A Group Policy Object was created and linked to the IT Organizational Unit.

**Skills Demonstrated**

- Group Policy
- Organizational Units

---

## 02 - Disable Control Panel Policy

![Disable Control Panel](../screenshots/group-policy/02-disable-control-panel-gpo-linked.png)

**Description**

A custom Group Policy was configured to prevent users from opening the Windows Control Panel.

**Skills Demonstrated**

- Group Policy Configuration
- Windows Administration

---

## 03 - GPResult Verification

![GPResult](../screenshots/group-policy/03-gpresult-policy-verification.png)

**Description**

The `gpresult` command confirmed that the workstation successfully received the applied Group Policy.

**Skills Demonstrated**

- Group Policy Verification
- Windows Command Line

---

## 04 - GPUpdate Success

![GPUpdate](../screenshots/group-policy/04-gpupdate-success.png)

**Description**

The `gpupdate /force` command refreshed Group Policy settings without requiring a reboot.

**Skills Demonstrated**

- Group Policy Management
- Windows Administration

---

## 05 - Control Panel Blocked

![Blocked](../screenshots/group-policy/05-control-panel-blocked.png)

**Description**

The workstation displayed the expected restriction message, verifying that the Group Policy was successfully enforced.

**Skills Demonstrated**

- Policy Enforcement
- Windows Security

---

# PowerShell

## 01 - Query Active Directory Users

![Query Users](../screenshots/powershell/01-active-directory-powershell-user-query.png)

**Description**

PowerShell was used to retrieve Active Directory user accounts using the Active Directory module.

**Skills Demonstrated**

- PowerShell
- Active Directory Automation

---

## 02 - Create User

![Create User](../screenshots/powershell/02-create-user-with-powershell.png)

**Description**

A new Active Directory user account was created using the `New-ADUser` cmdlet.

**Skills Demonstrated**

- User Provisioning
- PowerShell Automation

---

## 03 - Add User to Security Group

![Group Membership](../screenshots/powershell/03-add-user-to-security-group.png)

**Description**

The new user was added to the IT Admins security group using PowerShell.

**Skills Demonstrated**

- Group Administration
- PowerShell

---

## 04 - Disable User Account

![Disable User](../screenshots/powershell/04-disable-user-account.png)

**Description**

The user account was disabled using the Active Directory PowerShell module.

**Skills Demonstrated**

- Account Management
- PowerShell

---

## 05 - Enable User Account

![Enable User](../screenshots/powershell/05-enable-user-account.png)

**Description**

The previously disabled account was re-enabled to verify administrative account management.

**Skills Demonstrated**

- User Administration
- PowerShell Automation

---

## 06 - Export Active Directory Report

![Export CSV](../screenshots/powershell/06-export-ad-user-report.png)

**Description**

Active Directory user information was exported to a CSV report for administrative reporting and auditing.

**Skills Demonstrated**

- Reporting
- PowerShell
- Active Directory