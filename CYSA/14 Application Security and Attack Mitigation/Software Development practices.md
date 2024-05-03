SSDLC: Software Development Lifecycle, a process for developing software that emphasizes security through the development lifecycle. Helping mitigate security risks at every stage of the software development lifecycle. 


BufferOverlow: A buffer overflow is a software vulnerability that where a program attempts to write more data to a buffer than it can hold, causing excess data to overflow into adjacent memory space. 

Integer overflow: is a type of software vulnerability that occurs when a program tries to store an integer value larger than the maximum value that the data type can hold, causing the value to wrap around to a lower value or overflow into adjacent memory space. 

Broken authentication refers to an app that fails to restrict access to protected resources. 
- No requirement for passwords
- Vulnerable password reset mechanism
- Exposure of credentials or authorization tokens.
- Session hijacking

Input validation: any technique used to ensure that the data entered into a field or variable in an application is handled appropriately by that application

Output encoding: a defensive technique that assumes that input validation may have failed or that it might not have been possible to sanitize input. 


Parameterized queries: defend against code injectino attacks and insecure obejct references. This a type of output encoding. 
# Types of attacks
On-Path Attack: The attacker intercepts communication between two endpoints to capture their traffic. 

On-path attacks are accomplished by
- ARP Spoofing
- DNS Spoofing

Defend by using encrypted communication such as HTTPS or VPN


## Password attacks
Password Spraying: an attacker chooses predetermined passwords and tries them for multiple user accounts. An attacker may be able to collect a list of usernames from a poorly protected directory

## Credential stuffing
Use of credentials stolen from one source and trying them against multiple other sources. 





# OWASP Testing
1. Information Gathering
2. Configuration and Deployement Management
3. Identity Management testing
4. Input validation Testing
5. Testing for Error Handling and logging
6. Testing for cryptography
7. Business Logic testing
8. Client-side testing
9. Testing for web services
10. Test for Mobile security. 
