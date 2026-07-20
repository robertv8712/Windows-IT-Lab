# Windows IT Lab - Lab Notes

## Project Information

| Item | Details |
| ------ | --------- |
| Project | Windows IT Support Lab |
| Purpose | Practice Windows administration and Help Desk tasks |
| Project Type | Personal IT Support Lab |
| Host Operating System | Windows 11 |
| Guest Operating System | Windows 11 Pro |
| Virtualization Software | Oracle VirtualBox |
| Documentation | README.md, LAB-NOTES.md, TROUBLESHOOTING.md |

---

## Lab Objectives

The purpose of this project was to gain practical experience with Windows administration by simulating common Help Desk and IT Support tasks in a Windows 11 Pro virtual machine. 

The lab focused on user account management, file permissions, networking, troubleshooting, PowerShell, and system maintenance while documenting each completed task. 

---

## Virtual Machine Configuration

| Setting | Value |
|---------|-------|
| Guest OS | Windows 11 Pro |
| Memory | 4096 MB | 
| Processors | 2 |
| Graphics Controller | VBoxSVGA |
| Video Memory | 128 MB |
| 3D Acceleration | Disabled |

---

## User Accounts Created

| Username | Account Type | Purpose |
|----------|--------------|---------|
| employee1 | Standard User | Simulated employee account |
| employee2 | Standard User | Simulated employee account | 
| manager1 | Administrator | Simulated manager account |

---

## Work Performed

Completed all 17 simulated Help Desk tickets covering:

### Windows Administration

- Local User Creation
- Password Reset
- Disable and Enable User Accounts
- Add User to Administrators Group
- Rename User Account
- Delete User Account

### File System Administration

- Configure NTFS Permissions
- Configure Shared Folder 

### TroubleShooting 

- Investigate Event Viewer Logs
- Manage Windows Service
- Review Installed Hardware
- Monitor System Performance
- Examine Disk Management

### Command Line Administration

#### PowerShell

- Retrieve local users
- Retrieve local groups
- View administrator group membership

#### Command Prompt

- View hostname
- View current user
- Display IP configuration
- Test network connectivity
- Trace network route
- Perform DNS lookup

### System Maintenance

- Review System Information
- Check Windows Update 

---

## Administrative Tools Used

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

## Commands used

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

## Challenges Encountered

Several technical issues were encountered while building the virtual machine environment. 

These included:

- Incorrect installation media attached to the virtual machine
- Limited storage space during Windows installation
- Slow Windows installation performance 
- Windows setup requiring a Microsoft account
- VirtualBox critical error after setup
- Moving the virtual machine to external USB storage

Detailed troubleshooting steps and resolutions are documented in 
**TROUBLESHOOTING.md**.

---

## Skills Gained

Through this project, I gained practical experience with:

- Windows 11 Administration
- Help Desk Procedures
- User Account Management
- NTFS Permissions
- Shared Folder Configuration
- PowerShell Administration
- Command Prompt Utilities
- Network Diagnostics
- Windows Troubleshooting
- Virtual Machine Administration
- Technical Documentation

---

## Project Outcome

Successfully built a Windows 11 Pro virtual machine and completed all 17 simulated Help Desk tickets. 

This project strengthened my understanding of Windows administration, troubleshooting, PowerShell, networking, and documentation practices commonly used in entry-level IT Support and Help Desk roles.
