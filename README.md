# Reviving-an-HP-EliteOne-Gen2-with-Linux-Mint-Overview
This project documents the process of reviving an outdated Windows 10 AIO PC (HP EliteOne Gen2) by installing Linux Mint Cinnamon and applying basic system hardening.

---

The goal was to:
- Preserve hardware usability
- Provide a familiar Windows-like experience
- Improve system security and performancent Cinnamon

## Hardware

- Model: HP EliteOne 800 G2
- Form Factor: All-in-One
- Touchscreen Enabled
- Legacy Windows 10 System

## Installation Process

### 1. Download Linux Mint
- Downloaded Linux Mint Cinnamon (.torrent)
- Used qBittorrent to retrieve the ISO file

### 2. Create Bootable USB
- Used Rufus to burn ISO to USB
- Ignored Windows "Repair USB" prompt to avoid corruption

### 3. BIOS Configuration
- Disabled Legacy Support
- Enabled Secure Boot
- Cleared Secure Boot Keys
- Confirmed BIOS changes using 4-digit verification code

Note:
Clearing secure boot keys allowed the Linux kernel to register itself and resolved the half-black screen issue commonly reported on HP EliteOne systems.

### 4. Installation
- Erased disk
- Installed Linux Mint
- Successful first full boot

## Post-Installation Configuration

### System Updates
- Switched to local mirror
- Ran system update via terminal

### Codecs Installation
- Installed multimedia codecs

### Firewall
- Enabled UFW firewall
- Verified firewall enabled at startup

### Touchscreen Verification
- Used xinput list to confirm touchscreen detection
- Used xinput test to verify input response

### Backup & Restore
- Configured Timeshift for system restore snapshots

## Results

- Smooth performance
- Fully functional touchscreen
- Secure boot compatibility achieved
- Improved system responsiveness
- User satisfaction: 10/10

## Screenshots

### BIOS Configuration
![BIOS Settings](screenshots/bios-settings.jpg)

### Secure Boot Keys Cleared
![Secure Boot](screenshots/secure-boot.jpg)

### Linux Mint Desktop
![Desktop](Linux-Mint-Home.jpg)

### Touchscreen Detection
![xinput list](touchscreen.jpg)

### Firewall Status
![Firewall](codecs-and-firewall.jpg)
