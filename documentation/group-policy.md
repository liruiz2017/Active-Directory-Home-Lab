# Group Policy

## Overview

This lab demonstrates the creation and deployment of Group Policy Objects (GPOs) within Active Directory.

---

## Policy Created

**Disable Control Panel**

The policy prevents users in the IT Organizational Unit from opening the Windows Control Panel.

---

## Scope

The Group Policy Object was linked to:

- IT Organizational Unit

---

## Verification

Policies were refreshed using:

```
gpupdate /force
```

Policy application was verified using:

```
gpresult /r
```

---

## Results

The policy successfully applied to domain users within the IT OU.

Users attempting to open Control Panel received an administrator restriction message.

---

## Skills Demonstrated

- Group Policy Management
- OU Linking
- Policy Verification
- Windows Administration