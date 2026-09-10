# NETWORKWALKS-EMMANUEL-V083-WK1-PM1-CYBERSECURITY-LAB-SETUP

# Cybersecurity Lab Setup - VMware & Kali Linux

## 📌 Project Overview
This repository documents the setup of a cybersecurity testing lab environment on my laptop using VMware. The lab is designed for practicing ethical hacking and penetration testing in a safe, isolated environment.

## 🖥️ Lab Architecture
*   **Hypervisor:** VMware Workstation Player
*   **Attacking Machine:** Kali Linux 2026.x
*   **Network Subnet:** 10.0.0.0/24
*   **Kali IP Address:** 10.0.0.2/24
*   **Gateway:** 10.0.0.1

## 🛠️ Configuration Steps
1. **VMware Setup:** Configured a custom NAT network (VMnet8) on the `10.0.0.0/24` subnet.
2. **Kali Linux:** Imported the VMware image and set a static IP of `10.0.0.2`.
3. **Network Fix:** Applied the `ipv4.dad-timeout 0` fix to resolve internet connectivity issues in Kali.
4. **Shared Folders:** Enabled VMware Shared Folders to mount the host machine's `/downloads` directory inside Kali.
5. **Clipboard & Drag/Drop:** Enabled Guest Isolation in VMware and installed `open-vm-tools-desktop` for seamless file transfer.

## 🚀 How to Use This Lab
1. Ensure VMware Workstation is installed.
2. Open the Kali VM and verify the IP address using `ip a`.
3. Verify internet access with `ping -c 4 8.8.8.8`.
4. Access shared files in `/mnt/hgfs/downloads`.

## 📸 Snapshots
*   `Clean Install - Network Configured` (Snapshot taken after successful ping test).
