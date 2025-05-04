[🏠 Home](../README.md) • [🧪 Labs](../labs/README.md) • [🗒️ Notes](README.md)

# 🔍 Nmap Scanning Basics

## 🎯 Objective
Identify open ports and services on a target machine using Nmap.

## 🔧 Tools Used
- Nmap

## 🪜 Common Scans
1. Quick scan:
    ```
    nmap 172.21.175.100
    ```

2. Version detection:
    ```
    nmap -sV 172.21.175.100
    ```

3. Aggressive scan:
    ```
    nmap -A 172.21.175.100
    ```

4. Scan specific ports:
    ```
    nmap -p 21,22,80,443 172.21.175.100
    ```

## 🧠 Notes
- Use `-oN scan.txt` to save results.
- Always start with light scans, escalate as needed.

---
