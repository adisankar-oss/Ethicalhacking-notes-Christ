
📁 Introduction to Git & Cloning
Git is a version control system that helps developers track code changes and collaborate efficiently.
To copy a remote repository (e.g., from GitHub) to your local machine, use:
git clone <repository-URL>

This creates a local copy, allowing offline development.

🛡️ Two Types of Malware Analysis
1. Static Analysis
Analyzing a file without executing it. Focus areas include:

File type (.exe, .apk)
Metadata
Embedded strings
Code structure (via disassemblers)

This method is safe since the malware doesn't run.
2. Dynamic (Runtime) Analysis
Involves running the file in a controlled environment to observe its behavior:

File and system changes
Network activity
Resource usage


🏝️ Sandbox
A sandbox is an isolated virtual environment used in dynamic analysis to safely execute and study suspicious files (.exe, .apk, etc.) without harming the host system.

⚙️ ATS Software
ATS (Advanced Threat Simulation) tools are used to:

Detect sophisticated threats
Simulate attack scenarios
Analyze malware behavior

These are typically used in advanced cybersecurity setups.

🐧 Linux Commands for Cybersecurity
📂 Basic File & Directory Commands

ls: List directory contents
cd: Change directory
pwd: Show current path
mkdir: Create a new folder
rmdir: Delete an empty folder
cp: Copy files or directories
mv: Move or rename files/folders
man: Open manual for any command
echo: Display text in terminal
chmod: Change file permissions
clear: Clear terminal screen


🔸 Note: Linux is case-sensitive (e.g., File.txt ≠ file.txt)


📜 Creating Files
To create an empty file:
touch hacker.txt

View details with:
ls -lh


-l: Long listing (shows permissions, owner, etc.)
-h: Human-readable file sizes (e.g., KB, MB)


🔐 File Permission Basics
Every file has permissions for:

Owner (creator)
Group (other users in the same group)
Others (everyone else)

Change permissions using:
chmod [permissions] [filename]

Example:
chmod 755 hacker.txt

Means:

Owner: read, write, execute
Group: read, execute
Others: read, execute



