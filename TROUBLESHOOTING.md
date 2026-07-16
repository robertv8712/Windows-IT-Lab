# Windows IT Lab - Troubleshooting

## Overview

This document records the major issues encountered while building the Windows IT Support Lab and the steps taken to diagnose and resolve them.

The purpose of this document is to demonstrate troubleshooting, problem-solving, and documentation skills commonly used in IT Support environments. 

> **Note:** Not every issue was resolved on the first attempt. This document includes both unsuccessful troubleshooting steps and the final solutions to accurately reflect the troubleshooting process. 

---

## Issue 1 – Incorrect Installation Media

### Problem: 

When starting the virtual machine, Oracle VirtualBox booted into the Ubuntu installer (GNU GRUB) instead of the Windows installation.

### Cause

The Ubuntu ISO was still attached as the virtual optical drive.

### Resolution

1. Opened **VirtualBox Settings**.
2. Navigated to **Storage**.
3. Removed the Ubuntu ISO.
4. Attached the Windows 11 ISO.
5. Restarted the virtual machine.

### Result:

The Windows 11 installer loaded successfully.

---

## Issue 2 – Insufficient Disk Space During Installation

### Problem

During Windows installation, VirtualBox suspended the virtual machine and displayed a disk full error.

### Cause

The host computer did not have enough available storage to continue installing Windows.

### Resolution

1. Deleted unnecessary files from the host computer.
2. Moved large files to external storage.
3. Freed additional disk space.
4. Recreated the virtual machine after sufficient storage became available. 

### Result 

Windows installation completed successfully.

---

## Issue 3 – Slow Windows Installation Performance

### Problem 

The Windows installation progressed very slowly and remained at a certain percentage for an extended period. 

### Cause

Limited system resources and storage performance while installing Windows inside a virtual machine. 

### Resolution

1. Verified the installation was still progressing.
2. Allowed the installation to continue without interruption
3. Later, recreated the virtual machine on the laptop’s internal SSD after freeing approximately 30 GB of storage. 

### Result

Windows installed successfully and overall performance improved. 

---

## Issue 4 – Windows Setup Required a Microsoft Account

### Problem

During Windows 11 setup, the installer required a Microsoft account before installation could continue.

### Attempted Solution

1. Opened Command Prompt using **Shift + F10**.
2. Ran:

```cmd
OOBE\BYPASSNRO
```

The command did not resolve the issue, and Windows Setup continued to require a Microsoft account.

### Resolution

1. Powered off the virtual machine.
2. Opened **VirtualBox Settings**.
3. Disabled the virtual machine’s **Network Adapter**.
4. Started the virtual machine again.
5. Completed Windows Setup using a local account without connecting to the internet.

### Result

Windows Setup completed successfully using a local account.

---

## Issue 5 – VirtualBox Critical Error After Initial Setup

### Problem

Immediately after completing Windows Setup, VirtualBox displayed a critical error and stopped the virtual machine.

### Cause

The exact cause could not be confirmed. The error occurred immediately after Windows completed its initial setup while the virtual machine’s network adapter was disabled. 

### Resolution

1. Closed the virtual machine.
2. Re-enabled the virtual machine’s **Network Adapter**.
3. Started the virtual machine again.

### Result

Windows booted normally and continued operating without additional critical errors. 

---

## Issue 6 – Virtual Machine Storage Management

### Problem

The completed virtual machine occupied a significant amount of storage on the host computer.

### Cause

The Windows virtual disk required considerably more storage than expected.

### Resolution

1. Moved the virtual machine to a USB 3.1 flash drive.
2. Updated the virtual machine location in Oracle VirtualBox.
3. Verified that the virtual machine booted successfully from its new location.

### Result

Recovered storage space on the host computer while maintaining a fully functional virtual machine. 

---

## Lessons Learned

This project provided practical experience troubleshooting issues commonly encountered while building and maintaining Windows virtual machines. 

Key lessons included:

- Managing VirtualBox storage devices
- Configuring Windows installation media
- Resolving storage limitations
- Diagnosing VirtualBox startup issues
- Working with Windows local accounts
- Managing virtual machine files
- Documenting troubleshooting procedures

---

## Summary

All identified issues were successfully resolved, allowing the Windows 11 Pro virtual machine to function correctly and enabling completion of all 17 simulated Help Desk tickets.

This project strengthened my troubleshooting, documentation, and problem-solving skills while providing practical experience with Windows administration in a virtualized environment.