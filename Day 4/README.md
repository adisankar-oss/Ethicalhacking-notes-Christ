

# 🖧 Computer Networking & Cybersecurity Basics

---

## 📡 What is a Computer Network?

A **computer network** is a collection of connected devices that communicate with each other to share data, applications, and resources.

### Common Types of Networks:

| Network Type | Description                                           |
| ------------ | ----------------------------------------------------- |
| **LAN**      | Local Area Network – within a building or campus.     |
| **WAN**      | Wide Area Network – spans across cities or countries. |
| **Internet** | The global interconnected network.                    |

---

## 🌐 Subnet – Why It Matters

A **subnet (subnetwork)** breaks a larger network into smaller, manageable sections.

### Benefits:

* Improves **security** by isolating parts of a network.
* Enhances **performance** through traffic control.
* Devices within a subnet can communicate **directly**.

---

## 🔢 IP Address Explained

An **IP address** is a unique number assigned to every device on a network.

### Versions:

| Type | Example       | Description                                      |
| ---- | ------------- | ------------------------------------------------ |
| IPv4 | `192.168.0.1` | 32-bit, older format, still widely used.         |
| IPv6 | `2001:db8::1` | 128-bit, newer, designed for future scalability. |

---

## 🆔 What is a MAC Address?

* **MAC (Media Access Control)** address is a **permanent identifier** for network hardware.
* Format: `AA:BB:CC:DD:EE:FF`
* Burned into the **network interface card (NIC)** during manufacturing.

---

## 📊 IPv4 vs IPv6 Comparison

| Feature       | IPv4           | IPv6                  |
| ------------- | -------------- | --------------------- |
| Bit Length    | 32-bit         | 128-bit               |
| Format        | `192.168.1.1`  | `2001:db8:1234::abcd` |
| Address Space | \~4.3 billion  | Virtually unlimited   |
| Security      | Optional IPSec | IPSec built-in        |

---

## 🔁 TCP vs UDP – Quick Comparison

| Feature     | TCP                                      | UDP                      |
| ----------- | ---------------------------------------- | ------------------------ |
| Connection  | Connection-oriented (3-way handshake)    | Connectionless           |
| Reliability | High (acknowledgements, retransmissions) | Low (no guarantees)      |
| Speed       | Slower                                   | Faster                   |
| Use Cases   | File transfers, emails                   | Online gaming, streaming |

---

## 🌐 Port Forwarding – What & Why?

**Port forwarding** allows external access to devices on a private network.

### Example:

* Access a home computer remotely using port `3389` (commonly used for RDP).

---

## 🔒 UAC (User Account Control)

A **Windows security feature** that prevents unauthorized system changes.

* Triggers a popup when apps need admin rights.
* Helps prevent malware from executing silently.

---

## 🔍 Information Gathering Styles

| Mode    | Description              | Tools/Examples         |
| ------- | ------------------------ | ---------------------- |
| Passive | No direct interaction    | Google, Shodan, WHOIS  |
| Active  | Direct probing of target | Nmap, ping, traceroute |

---

## 🛠️ Nmap – Powerful Network Scanner

**Nmap (Network Mapper)** is used by both hackers and system administrators to:

* Discover active hosts
* Identify open ports
* Detect OS and service versions

---

## ⚠️ Sample Cyber Attack Timeline

1. Attacker sends a phishing email with a `.zip` attachment.
2. User extracts and runs the `.exe` file using a password.
3. The malicious file opens a **reverse connection**.
4. **PowerShell scripts** are silently executed.
5. **UAC popups** appear repeatedly to gain admin access.
6. If user allows, the system becomes **fully compromised**.

> ⚠️ **Pro Tip:** Never run unknown executables, even from trusted contacts.

---

## 🔧 Nmap Command Breakdown

### Example Command:

```
nmap -Pn -A -sV -O -oN result.txt --script default -vv -p 1-1000 -sS -sT
```

| Flag       | Description                                        |
| ---------- | -------------------------------------------------- |
| `-Pn`      | Treat all hosts as up (skip pinging)               |
| `-A`       | Enable OS detection, version detection, traceroute |
| `-sV`      | Show service versions                              |
| `-O`       | Identify operating system                          |
| `-oN`      | Output results to a normal text file               |
| `--script` | Run default or specific Nmap scripts               |
| `-vv`      | Increase verbosity (more output detail)            |
| `-p`       | Scan specific ports (e.g., 1–1000)                 |
| `-sS`      | TCP SYN scan (stealthy)                            |
| `-sT`      | TCP connect scan (used if SYN fails)               |

---

## ✅ Summary

This guide covered essential concepts in networking, cybersecurity basics, and powerful tools like **Nmap**. Whether you're a beginner or brushing up for a certification or interview, understanding these topics builds a strong foundation.

---

