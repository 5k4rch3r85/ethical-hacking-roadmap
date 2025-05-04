[🏠 Home](../README.md) • [🧪 Labs](./) • [🗒️ Notes](../notes/)

# 🔎 Nmap & Netcat Usage

## 🧰 Nmap - Network Mapping

Nmap (Network Mapper) is a powerful open-source tool for network discovery and security auditing.

---

### 🔍 Common Commands

**1. Scan a subnet to discover live hosts:**
```bash
nmap -sn 192.168.1.0/24
```

**2. Perform a service and version scan on a host:**
```bash
nmap -sV 192.168.1.10
```

**3. Full aggressive scan (OS, version, script, traceroute):**
```bash
nmap -A 192.168.1.10
```

**4. Stealth SYN scan (quieter scan):**
```bash
nmap -sS -T4 -Pn 192.168.1.10
```

---

### 🔧 Explanation of Flags
- `-sS`: TCP SYN scan (stealth)
- `-sV`: Service version detection
- `-A`: Aggressive scan (includes OS detection and script scanning)
- `-T4`: Timing template (4 = faster scan)
- `-Pn`: Skip host discovery (assume host is up)
- `-sn`: Ping scan (host discovery only)

---

## 🧪 Netcat - The Hacker’s Swiss Army Knife

Netcat (nc) is used for reading/writing data across network connections.

---

### 🔌 Common Uses

**1. Set up a listener:**
```bash
nc -lvnp 4444
```

**2. Connect to a listener:**
```bash
nc 192.168.1.10 4444
```

**3. File transfer with Netcat**

**Receiver (on Kali):**
```bash
nc -lvnp 4444 > received.txt
```

**Sender (on Metasploitable):**
```bash
nc <kali_ip> 4444 < file.txt
```

---

## ✅ Practice

- [ ] Identify Metasploitable’s IP using `nmap -sn`
- [ ] Run a full service scan with `nmap -sV <ip>`
- [ ] Open a listener on Kali with Netcat
- [ ] Connect from Metasploitable back to Kali with Netcat
- [ ] Try sending a small file over Netcat between the systems

