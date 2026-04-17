# Cross-Site Scripting (XSS) - Security Analysis
Cross-Site Scripting (XSS) is a web application vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users.
These scripts are executed in the victim’s browser, making it possible to steal data or manipulate user sessions.

# How it works
Web applications that accept user input without proper validation may allow attackers to inject JavaScript code into pages.

Example:
<script>alert('XSS')</script>

If the application does not sanitize input, this script will execute in the browser of any user who views the page.

# Types of XSS
- Stored XSS:
Malicious script is saved on the server (e.g., in a database) and served to users later.

- Reflected XSS:
Script is reflected off a web server (e.g., via URL parameters) and executed immediately.

- DOM-Based XSS:
The vulnerability exists in client-side JavaScript rather than the server.

# Impact Analysis
XSS attacks can lead to:

Theft of session cookies
Account hijacking
Unauthorized actions on behalf of users
Defacement of web pages
Redirection to malicious websites

# How/ways to Prevent 
To prevent XSS vulnerabilities:

Validate and sanitize all user input
Encode output before rendering in the browser
Use Content Security Policy (CSP)
Avoid directly inserting user input into HTML/JavaScript
Use secure frameworks that automatically escape output

# How to Detect
You can detect XSS attacks using:
Manual testing with payloads
Browser developer tools
Automated scanners (e.g., Burp Suite)
Reviewing application code for unsafe DOM manipulation

# NOTES
XSS targets users, not the server directly
It exploits poor input handling and output rendering
It can compromise user data and sessions
Proper validation and encoding are critical defenses

# References
OWASP Top 10 – Cross-Site Scripting (XSS)
