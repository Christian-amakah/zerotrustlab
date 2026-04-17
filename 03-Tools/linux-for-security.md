## Linux for Security-Command Line Fundamentals
Linux is widely used in cybersecurity for penetration testing, system administration, and security analysis.
Most security tools and environments (e.g., parrot, Kali Linux) are built on Linux systems.

## Objective
To demonstrate essential Linux commands used in cybersecurity for navigation, file management, and system analysis.

# Key Concepts
- File System- Structure used to store and organize files
- Permissions- Control who can read, write, or execute files
- Shell- Interface for interacting with the system via commands

## Essential Commands
# Navigation
- pwd
- ls
- cd

- pwd- Shows current directory
- ls- Lists files and directories
- cd- Changes directory 

# File Management
- touch file.txt
- cp file.txt backup.txt
- mv file.txt newfile.txt
- rm file.txt

# permissions
- chmod 755 file.sh
- ls -l

chmod- Modify file permissions
- ls -l - View permissions

# Viewing File Content
- cat file.txt
- less file.txt

# searching
- grep "password" file.txt
- find / -name file.txt

# Security Use Case
A security analyst may:

- Navigate system directories
- Search for sensitive files
- Check file permissions
- Identify misconfigurations

# Importance of Security
Linux knowledge is important for:

- Penetration testing
- Log analysis
- System hardening
- Incident response

Misconfigured permissions can lead to:
- Unauthorized access
- Privilege escalation

# Best practices (to watch out for)
- Restrict file permissions appropriately
- Avoid running commands as root unnecessarily
- Monitor system logs
- Keep systems updated

# NOTE
- Linux is fundamental to cybersecurity work
- Command-line skills enable deeper system control
- Understanding permissions is critical for security

# References 
Linux Documentation
