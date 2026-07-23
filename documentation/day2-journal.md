# Day 2 Journal

## Objective

Expand the Active Directory environment by implementing Group Policy, file sharing, and PowerShell automation.

---

## Tasks Completed

### Group Policy
- Created a custom Group Policy Object (Disable Control Panel).
- Linked the policy to the IT Organizational Unit.
- Verified policy application using:
  - gpupdate /force
  - gpresult /r
- Confirmed users in the IT OU could no longer access Control Panel.

---

### File Server

- Created departmental shared folders:
  - Finance
  - HR
  - IT
  - Sales
- Configured Share Permissions.
- Configured NTFS Permissions.
- Verified authorized access to the IT share.
- Verified unauthorized users received an "Access Denied" message when attempting to access the HR share.

---

### PowerShell Automation

Completed several Active Directory administrative tasks using PowerShell:

- Listed all Active Directory users.
- Created a new user (Alex Rivera).
- Added the user to the IT Admins security group.
- Disabled the user account.
- Re-enabled the user account.
- Exported Active Directory users to a CSV report.

---

## Challenges

During PowerShell automation, I initially used an incorrect cmdlet parameter while creating a new user, which generated an error. After reviewing the syntax, I corrected the command and successfully created the account.

I also attempted to use an incorrect cmdlet when re-enabling the user account. After identifying the correct Active Directory cmdlet, the account was successfully re-enabled.

---

## Skills Practiced

- Group Policy Management
- File Server Administration
- NTFS Permissions
- Share Permissions
- Active Directory PowerShell Module
- Windows Server Administration
- Troubleshooting

---

## Reflection

Today's work expanded the Active Directory lab beyond basic user management into enterprise administration. Implementing Group Policy, configuring file shares, and automating tasks with PowerShell provided hands-on experience with technologies commonly used by Windows System Administrators. These exercises reinforced the importance of centralized management, access control, and automation in enterprise IT environments.