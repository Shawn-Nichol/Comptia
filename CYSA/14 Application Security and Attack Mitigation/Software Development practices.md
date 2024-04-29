Secure development practices refer to a set of guidelines and procedures designed to ensure the security of software applications by emphasizing security throughout the software development life cycle. 


SSDLC: Secure Software Development Life Cycle, A method of system development that incorporates security controls in every phase of the system's lifecycle. 

Broken Authentication: A software vulnerability where the authentication mechanism allows an attacker to gain entry, such as displaying cleartext credentials, using weak session tokens, or permitting brute force. 

Input Validation: Any technique used to ensure that the data entered into a field or variable in an application is handled appropriately by that application. 

Output Encoding: Coding methods to sanitize output created from user input. 

Parameterized queries: A technique that defends against SQLi by incorporating placeholders in a SQL query

Buffer Overflow: An attack in which data goes past the boundary of the destination buffer and begins to corrupt adjacent memory. This can allow the attacker to crash the system or execute arbitrary code. 

Heap Overflow: A software vulnerability where input is allowed to overwrite memory locations within the area of a process's memory allocation used to store dynamically sized variables. 

Integer Overflow: An attack in which a computed result is too large to fit in its assigned storage space, which may lead to crashing or data corruption and may trigger a buffer overflow. 

ASLR: Address Space Layout Randomization, A technique that randomizes where components in a running application are placed in memory to protect against buffer overflows. 






Session Management Best practices for Secure sessions
- Use Secure Sessions; session IDs should be randomly generated, long, and difficult to guess to prevent guessing or brute-forcing session IDS
- Use secure cookies; and HTTPS only. Cookies do not contain sensitive information and expire after a responsible time.
- Session timeouts
- Strong Password Policy
- MFA
- Access controls: Restrict access to sensitive resources and prevent unauthorized access.
- Protect against session hijacking and fixation, which involves stealing or manipulating a user's session ID. Developers must utilize secure session IDs and implement secure cookie-handling practices. 

# On-Path Attack:
An attack is when an attacker intercepts communications between two endpoints to capture their traffic.

How
On-path attacks are accomplished via several methods, but common techniques include ARP spoofing and DNS spoofing.

Defend
using encryption communication such as HTTP and VPN. 

# Password SSpraying and Credential Stuffing
Online Password attack describes a direct interaction with the authentication service - a web login form or VPN gateway, when the attacker typically submits passwords using a pre-compiled list. Online attacks are noisy meaning clear evidence appears in logs and packet captures as rapid password failures. 

Password Spraying: Describes when an attacker chooses predetermined passwords and tries them for multiple user accounts. 

Credential Stuffing: Describes the use of credentials stolen from one source and trying them against multiple other sources. 

Defend
 Strong passwords, account lockouts, and MFA are effective against these attacks. 

# SQL Injection
An attack that injects a database query into the input data directed at a server by accessing the client side of the application.


# Directory Traversal
An application attack that allows access to commands, files, and directories that may or may not be connected to the web document root directory. 

# Cross-Site Scripting
A malicious script hosted on an attacker's site or coded in a link injected onto a trusted site is designed to compromise clients browsing the trusted site, circumventing the browser's security model of trusted zones. 

Reflected XSS; bounces off the web server when the link is clicked

Persistent XSS is when malicious code is injected into a web application's database, which is then executed by all future visitors who view the infected page. Persistent XSS attacks are particularly dangerous data and can also be used to gain unauthorized access to web application databases. 

# File inclusion
A web application vulnerability that allows an attacker either to download a file from an arbitrary location on the host file system or to upload an executable or script file to open a backdoor. 

# Session Hijacking: 
A type of spoofing attack where the attacker disconnects a host and then replaces it with his or her own machine, spoofing the original host's IP addresses. 

# Cross-Site Request Forgery
A malicious script hosted on the attacker's site can exploit a session started on another site in the same browser. 

# Server-side Request Forgery
An attack where an attacker takes advantage of the trust established between the server and the resource it can access, including itself. 


# Attack mitigation checklist
Security Misconfiguration: Perform regular vulnerability assessments and pen tests, secure default settings, and use configuration management tools. Ensure that patches are updated regularly, restrict access to configuration interfaces, monitor and log configuration changes, and use regular skills. 
