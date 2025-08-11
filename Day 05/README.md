📚 Day 05 – Cybersecurity Concepts
🔌 1. Ports – Network Entry Points
Definition:
A port is like a numbered gateway that allows data to enter or leave a system over a network.

Why Important in Security?
Attackers often scan ports to find open services to target.

Port Categories:

Type	Range	Purpose	Example
Well-Known Ports	0 – 1023	Standard services	HTTP (80), FTP (21)
Registered Ports	1024 – 49151	Applications & custom services	MySQL (3306)
Dynamic/Private Ports	49152 – 65535	Temporary client-side communications	Web browser sessions

📁 2. Port 21 – File Transfer Protocol (FTP)
Purpose: Enables file transfers over TCP/IP.

Security Weaknesses:

Sends usernames & passwords in plain text.

Prone to sniffing and brute-force attacks.

Safer Alternatives:
FTPS (over SSL/TLS) or SFTP (over SSH).

👤 3. Low-Privilege Account
Definition: User account with limited system rights.

Security Benefit:

Restricts damage if compromised.

Enforces the Principle of Least Privilege.

Example in Linux:
guest or a standard user without sudo.

🐧 4. Linux User Types
Root User:
Full control over the system.
Regular User:
Used for everyday tasks; restricted access.

Security Note:
Attackers often aim to escalate privileges from regular → root.

Check Users:

bash
Copy
Edit
who
w
cat /etc/passwd
🚀 5. Privilege Escalation
Definition:
Gaining more permissions than originally assigned.

Types:

Vertical: User → Admin/Root

Horizontal: One user → Another user’s account

Common Methods:

Misconfigured sudo rules

Kernel vulnerabilities

Weak file permissions

Services running with root privileges

⏱ 6. watch Command
Function: Runs a command repeatedly and updates output automatically.

Example:

bash
Copy
Edit
watch -n 1 who
(Shows logged-in users every second.)

Security Use:
Monitor logins, file changes, or network status in real time.

🛡 7. Security Operations Center (SOC)
Definition:
A centralized team that continuously monitors, detects, and responds to cyber threats.

Core Functions:

Monitoring: Logs, user activities, network flows

Incident Response: Containing and mitigating attacks

Threat Hunting: Searching for hidden risks

Tools: SIEM, IDS/IPS, packet analyzers.

💻 8. TryHackMe
What It Is:
An interactive platform for learning cybersecurity hands-on.

Purpose:
Practice penetration testing, security analysis, and hacking techniques in virtual labs.

In Class:
Used for exercises like enumeration, exploitation, privilege escalation, and post-exploitation.

