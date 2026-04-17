# Nmap-Networking Scanning Enumeration
Nmap (Network Mapper) is an open-source tool used for network discovery and security auditing.
It helps identify active hosts, open ports, running services, and potential vulnerabilities.

# Objective
To understand how Nmap is used in real-world scenarios for reconnaissance and to analyze
exposed services from a security perspective.

# Key Note
- Port Communication endpoint (e.g., 80 for HTTP)
- Open Port Accepting connections
- Closed Port No active service
- Filtered Port Blocked by firewall

# Common Commands
- Basic scan:
nmap 192.168.1.1

- Service version Detection:
nmap -sV 192.168.1.1

- OS Detection:
nmap -o 192.168.1.1

- Aggressive Scan:
nmap -A 192.168.1.1

# Scan Scenario
- Target: Local test environment (e.g., 192.168.1.1)
- Purpose: Identify open ports and running services

Note: Sample results are used for demonstration purposes.

Sample Findings:
- Port       State        Service         Version
- 22           open         SSH            OpenSSH 7.6
- 80           open         HTTP           Apache 2.4
- 443          open         HTTPS           Nginx 

# Analysis
Port 22 (SSH)- Remote access service; potential target for brute-force attacks
Port 80 (HTTP)-Web server, possible exposure to vulnerabilities like XSS or SQL Injection
Port 443 (HTTPS)- Encrypted service, should be checked for SSL/TLS misconfiguration

# Security Implications
Open ports increase attack surface
Exposed services may contain vulnerabilities
Misconfigurations can lead to unauthorized access

# Recommendations
Restrict access to sensitive ports (e.g., SSH)
Keep services updated and patched
Use firewalls to limit exposure
Monitor network traffic for suspicious activity

# NOTE
Nmap is essential for reconnaissance and enumeration
It reveals critical information about target systems
Understanding scan results is as important as running the scan.

# References
Nmap Official Documentation
