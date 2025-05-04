[🏠 Home](../README.md) • [🧪 Labs](../labs/) • [🗒️ Notes](../notes/)

# 🐉 Installing Kali Linux via Virtual Machine

This guide walks you through installing Kali Linux using a virtual machine for a safe, isolated ethical hacking environment.

---

## 🧰 What You’ll Need

- A virtualization platform:
  - [VirtualBox (Free)](https://www.virtualbox.org/)
  - [VMware Workstation Player (Free for non-commercial)](https://www.vmware.com/products/workstation-player.html)
  - [Hyper-V (Built-in on Windows Pro)](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/about/)

- Kali Linux ISO or prebuilt VM image:
  - [Download Kali Linux](https://www.kali.org/get-kali/)

---

## 🎬 Video Guides

### VirtualBox
- [How to Install Kali Linux on VirtualBox - YouTube](https://www.youtube.com/watch?v=J6N2YwMwWRM)

### VMware
- [Install Kali Linux on VMware Player - YouTube](https://www.youtube.com/watch?v=xGJAvlLCEtE)

### Hyper-V
- [Install Kali Linux in Hyper-V on Windows 11 - YouTube](https://www.youtube.com/watch?v=aVSTv6NoSkM)

---

## 🧭 Step-by-Step: VirtualBox Example

### 1. Install VirtualBox
Download and install VirtualBox from the official site: https://www.virtualbox.org/

### 2. Download Kali VM Image
Go to: https://www.kali.org/get-kali/
Choose **“Virtual Machines”** > Select your hypervisor (OVA for VirtualBox)

### 3. Import the OVA File
- Open VirtualBox
- Go to **File > Import Appliance**
- Select the downloaded `.ova` file and proceed through the wizard

### 4. Modify VM Settings (optional)
- Set memory: 2048 MB or more
- CPU: 2 cores minimum
- Enable Network Adapter: Bridged or NAT

### 5. Start the VM
- Boot up the Kali machine
- Default credentials:
  - Username: `kali`
  - Password: `kali`

---

## ⚙️ Step-by-Step: ISO Install Method

For full installation:

### 1. Download Kali ISO
https://www.kali.org/get-kali/

### 2. Create New VM
- Open your virtualization software
- Create a new VM
- Attach Kali ISO as the boot disk

### 3. Go Through Installation Wizard
- Choose language, keyboard, and location
- Configure user account and password
- Partition the disk (Guided is fine for beginners)
- Wait for installation to complete
- Reboot and log in

---

## 🔐 Post-Install Checklist

- 🔄 Update system:
```bash
sudo apt update && sudo apt upgrade
```

- 👤 Change default password:
```bash
passwd
```

- 🔧 Install VirtualBox Guest Additions (if needed):
```bash
sudo apt install virtualbox-guest-x11
```

---

## 📂 Save Point

This is your base ethical hacking lab VM — snapshot it before installing tools or launching attacks.

