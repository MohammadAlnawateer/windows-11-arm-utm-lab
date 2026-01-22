# Windows 11 ARM64 on macOS (UTM Lab)

This project documents setting up a Windows 11 ARM64 virtual machine on macOS using **UTM** and **QEMU**.  
The goal of this lab was to understand how ARM-based virtualization works on Apple Silicon Macs and to practice troubleshooting common installation issues.

---

## Lab Overview

- Host OS: macOS (Apple Silicon)
- Virtualization Tool: UTM (QEMU-based)
- Guest OS: Windows 11 ARM64
- Firmware: UEFI
- Disk Type: Virtual disk (QCOW2)
- Network: Shared network (virtio)

---

## What Was Done

- Created a new Windows 11 ARM virtual machine in UTM
- Booted the installer using UEFI firmware
- Configured and formatted the virtual disk during setup
- Completed Windows 11 installation without a product key
- Resolved network setup issues during the initial Windows setup
- Verified successful boot into the Windows 11 desktop

---

## Issues Encountered and Fixes

### Network Required During Setup
During the Windows 11 setup, the installer required an internet connection but no network adapter was detected.

**Solution:**
- Used the Windows setup bypass method to continue with limited setup
- Completed installation first, then confirmed network connectivity after reaching the desktop

---

## Skills Demonstrated

- Virtual machine setup and configuration
- ARM64 vs x64 architecture awareness
- UEFI boot process
- Windows OS installation and troubleshooting
- Basic virtualization networking concepts

---

## Screenshots

Screenshots of the installation steps and final desktop are included in the `screenshots/` folder.

---

## Why This Lab Matters

This lab demonstrates hands-on experience with modern virtualization on Apple Silicon, which is increasingly common in IT support and systems roles. It also shows practical problem-solving during OS deployment.

---

## Status

✔ Installation completed successfully  
✔ Windows 11 ARM64 running on macOS via UTM  
✔ Network connectivity verified
