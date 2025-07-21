# 🛡️ Cybersecurity Notes - Day 2

## 🗓️ Topic: Setting Up Kali Linux on VirtualBox + Kali Tool Overview

---

## 1️⃣ Booting Kali Linux on VirtualBox

### 🔧 Prerequisites
- **VirtualBox** installed
- **Kali Linux ISO** or OVA file downloaded from [https://www.kali.org](https://www.kali.org)

---

### 🖥️ Step-by-Step Setup

1. **Open VirtualBox**
   - Click on `New` to create a new virtual machine.

2. **Configure Virtual Machine**
   - **Name**: Kali Linux
   - **Type**: Linux
   - **Version**: Debian (64-bit)

3. **Memory Allocation**
   - Recommended: **2 GB (2048 MB)** or more.

4. **Hard Disk**
   - Create a **Virtual Hard Disk now**.
   - Recommended size: **20 GB** or more (Dynamically allocated).

5. **Attach Kali ISO**
   - Go to **Settings → Storage**.
   - Click on the empty CD icon and **choose a disk file** (select Kali ISO).

6. **Boot VM**
   - Start the VM → Select `Graphical Install` or `Live Boot`.

7. **(Optional) Install Kali**
   - Follow on-screen instructions to install Kali on the virtual disk.
   - Set username and password for access.

---

## 2️⃣ Tools Demonstrated in Kali Linux

### 🔍 2.1 Categories of Tools

| Category        | Example Tools           | Description                                  |
|----------------|-------------------------|----------------------------------------------|
| **Information Gathering** | `nmap`, `whois`, `dnsenum` | Collect data about target systems/networks. |
| **Vulnerability Analysis** | `nikto`, `OpenVAS`          | Scan systems for known vulnerabilities.      |
| **Web Application Testing** | `Burp Suite`, `OWASP ZAP` | Intercept and analyze HTTP requests/responses. |
| **Exploitation Tools** | `Metasploit`, `msfvenom`     | Launch exploits against vulnerable systems.  |
| **Password Attacks** | `Hydra`, `John the Ripper`     | Brute-force login credentials.               |
| **Wireless Attacks** | `aircrack-ng`, `reaver`       | Target Wi-Fi networks for testing.           |

---

### 🧪 2.2 Demonstrations Done

1. **nmap**
   - Used for scanning local IP to find open ports and services.
   - Command:
     ```bash
     nmap -sS 192.168.x.x
     ```

2. **whois**
   - Used for domain information.
   - Command:
     ```bash
     whois example.com
     ```

3. **Burp Suite**
   - GUI tool to intercept, modify, and analyze web traffic.
   - Used in proxy with browser to test web app vulnerabilities.

4. **Metasploit Framework**
   - Launched from terminal using:
     ```bash
     msfconsole
     ```

5. **Hydra**
   - Used for dictionary attacks on login services like FTP, SSH, etc.
   - Example:
     ```bash
     hydra -l admin -P passwords.txt ftp://192.168.x.x
     ```

---

## 📝 Summary

- Kali Linux was successfully booted and explored using VirtualBox.
- Various pre-installed tools were introduced under different categories.
- Basic demonstrations gave insight into scanning, information gathering, and password attack techniques.

---

> ✅ **Next Steps**: Practice using basic commands and explore GUI tools like Burp Suite and Zenmap.

> 💡 Tip: Always run tools in **legal environments** like test labs or virtual networks.

---

