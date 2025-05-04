# 📡 Telnet Login with Default Credentials

## 🎯 Objective
Gain access to Metasploitable using default Telnet credentials.

## 🔧 Tools Used
- Telnet client (built into Kali)

## 🪜 Steps
1. Connect to the target:
    ```
    telnet 172.21.175.100
    ```

2. Try default creds:
    ```
    Username: msfadmin
    Password: msfadmin
    ```

3. Validate shell access:
    ```
    whoami
    uname -a
    ```

## 🧠 Notes
- No exploit required — this demonstrates the risk of weak/default credentials.
---
