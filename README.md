# Windows IT Support Lab

A hands-on Windows 11 Pro laboratory built in Oracle VirtualBox to simulate real-world Help Desk and IT Support tasks. 

This project demonstrates practical experience with Windows administration, user account management, NTFS permissions, PowerShell, networking, and troubleshooting through 17 simulated support tickets. 

The goal of this lab was to strengthen the technical skills commonly required for entry-level IT Support and Help Desk positions while developing clear technical documentation and troubleshooting practices. 

---

# Table of Contents

- [Project Overview](#project-overview)
- [Skills Demonstrated](#skills-demonstrated)
- [Lab Environment](#lab-environment)
- [Administrative Tools Used](#administrative-tools-used)
- [Help Desk Tickets Completed](#help-desk-tickets-completed)
- [Lab Walkthrough](#lab-walkthrough)
- [Project Structure](#project-structure)
- [Commands Used](#commands-used)
- [Learning Outcomes](#learning-outcomes)
- [Future Improvements](#future-improvements)
- [Acknowledgements](#acknowledgements)

---

## Project Overview:

The objective of this lab was to gain practical experience performing common Windows administration tasks encountered in Help Desk and IT Support roles.

The lab was built using a Windows 11 Pro virtual machine in Oracle VirtualBox and focused on practical system administration rather than theory. Throughout the project, I completed 17 simulated support tickets covering user management, permissions, networking, troubleshooting, PowerShell, and system maintenance. 

---

## Skills Demonstrated

### Windows Administration

- Local User and Group Management
- Password Reset and Recovery
- User Account Administration
- Administrator Permissions

### File System Administration

- NTFS Permissions
- Shared Folder Configuration

### Troubleshooting

- Event Viewer
- Windows Services
- Device Manager
- Task Manager
- Disk Management

### Networking

- IP Configuration
- Network Connectivity Testing
- DNS Lookup
- Basic Network Diagnostics

### Command Line

- PowerShell
- Command Prompt

### System Maintenance

- Windows Update
- System Information

---

## Lab Environment

| Component | Details |
| ----------------|-----------|
| Host Operating System | Windows 11 |
| Guest Operating System | Windows 11 Pro |
| Virtualization Software | Oracle VirtualBox |
| Memory | 4096 MB |
| Processors | 2 |
| Graphics Controller | VBoxSVGA|
| Video Memory | 128 MB |
| 3D Acceleration | Disabled |

---

### Administrative Tools Used

- Computer Management
- Local Users and Groups
- Event Viewer
- Services
- Device Manager
- Task Manager
- Disk Management
- PowerShell
- Command Prompt
- Windows Update
- System Information

---

### Help Desk Tickets Competed

| Ticket | Description | Status |
| -------- | --------------- | :-------: |
| 001 | Local User Creation | ✅|
| 002 | Password Reset | ✅|
| 003 | Disable / Enable User Account | ✅|
| 004 | Add User to Administrators Group | ✅|
| 005 | Rename user Account | ✅|
| 006 | Delete User Account | ✅|
| 007 | Configure NTFS Permissions | ✅|
| 008 | Configure Shared Folder | ✅|
| 009 | Investigate Event Viewer Logs | ✅|
| 010 | Manage Windows Services | ✅|
| 011 | Review Installed Hardware | ✅|
| 012 | Monitor System Performance | ✅|
| 013 | Examine Disk Management | ✅|
| 014 | PowerShell Administration | ✅|
| 015 | Network Diagnostics | ✅|
| 016 | Review System Information | ✅|
| 017 | Windows Update | ✅|

--- 

## Lab Walkthrough

Below are representative Help Desk tickets completed during this project. Additional screenshots for every ticket are available in the `screenshots/` directory.

---

### Ticket 001 – Local User Creation

Created multiple local user accounts using **Computer Management → Local Users and Groups** to simulate employee accounts used throughout the lab. 

**Skills Demonstrated**

- User Management
- Computer Management
- Local Accounts

**Screenshots**

```text
screenshots/Ticket-001-Local-User-Creation/
├── creating_employee1.png
├── creating_manager1.png
└── showing_new_users.png
```

---

### Ticket 007 – Configure NTFS Permissions

Configured NTFS permissions by granting standard users read-only access while allowing administrators full control.  

**Skills Demonstrated**

- NTFS permissions
- Folder Security
- Windows File System Administration

**Screenshots**

```text
screenshots/Ticket-007-Configure-NTFS-Permissions/
├── default_permission_of_folder.png
├── showing_users_permissions.png
└── showing_administrator_permission.png
```

---

### Ticket 009 – Investigate Event Viewer Logs

Reviewed Application and System logs to identify informational, warning, and error events. 

**Skills Demonstrated**

- Event Viewer
- Log Analysis
- Troubleshooting

**Screenshots**

```text
screenshots/Ticket-009-Investigate-Event-Viewer-Logs/
├── system_error_log.png
├── system_information_log.png
├── system_warning_log.png
├── application_information_log.png
├── application_error_log.png
└── application_warning_log.png
```

---

### Ticket 014 – PowerShell Administration

Used PowerShell to retrieve local users, local groups, and administrator group membership.

**Commands**

```powershell
Get-LocalUser
Get-LocalGroup
Get-LocalGroupMember Administrators
```
**Screenshots**

```text
screenshots/Ticket-014-PowerShell-Adminitration/
├── powershell_Get-LocalUser.png
├── powershell_Get-LocalGroup.png
└── powershell_Get_LocalGroupMember_Administrators.png
```

---

### Ticket 015 – Network Diagnostics

Performed basic network troubleshooting using Command Prompt. 

**Commands**

```cmd
hostname 
whoami 
ipconfig 
ping google.com 
tracert google.com 
nslookup google.com 
```

**Screenshots**

```text
screenshots/Ticket-015-Network-Diagnostics/
├── command_hostname_whoami_ipconfig.ong
├── command_ping_google_com.png
├── command_tracert_google_com.png
└── command_nslookup_google_com.png
```

---

### Ticket 017 – Windows Update

Verified Windows Update configuration and checked for available updates.

**Skills Demonstrated**

- Windows Maintenance
- Operating System Updates

**Screenshots**

```text
screenshots/Ticket-017-Windows-Update/
└── Window_11_Pro_windows_update.png
```

---

## Project Structure

```text
Windows-IT-Lab/
│
├── README.md
├── LAB-NOTES.md
├── TROUBLESHOOTING.md
├── LICENSE
├── .gitignore
│
├── screenshots/
    ├── Ticket-001-Local-User-Creation/
    ├── Ticket-002-Password-Reset/
    ├── Ticket-003-Disable-Enable-User-Account/
    ├── …
    └── Ticket-017-Windows-Update/

```

---

## Commands Used

### PowerShell

```powershell
Get-LocalUser
Get-LocalGroup
Get-LocalGroupMember Administrators
```

### Command Prompt

```cmd
hostname 
whoami 
ipconfig 
ping google.com
tracert google.com
nslookup google.com
```

---

## Learning Outcomes

This project strengthened my practical experience with Windows administration by completing common Help Desk tasks in a virtual environment. I gained experience with user account management, permissions, PowerShell, networking, troubleshooting, and documenting technical work in a structured and repeatable way. 

---

## Future Improvements

Future enhancements for this lab include:

- Active Directory Domain Services
- Group Policy Management
- Windows Server Administration
- Microsoft 365 Administration
- Remote Desktop Configuration
- Windows Security Policies

---

## Acknowledgements

This project was created as part of my personal IT portfolio to develop practical Windows administration skills and prepare for entry-level IT Support and Help Desk positions. 

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details. 
