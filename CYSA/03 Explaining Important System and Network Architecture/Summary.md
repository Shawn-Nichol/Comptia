System hardening is the process of making a host or app configuration secure by reducing its attack surface. This is done by running only necessary services, installing monitoring software to protect against malware and intrusion, and establishing a maintenance schedule to ensure the system is patched to be secure against software exploits. 


CASB: Cloud access security Broker, Enterprise management software designed to mediate users' access to cloud services across all types of devices. 

Federation: A process that provides a shared login capability across multiple systems and enterprises. It essentially connects the identity management services of multiple systems. 

Forward Proxy: A server that mediates the communication between a client and another server. It can filter and often modify communications as well as provide caching services to improve performance.

OpenID: An identity federation method that enables the users to be authenticated on cooperating websites by a third-party authentication services. 
Out-of-band mechanism: Use a communication channel that is different than the one currently being used. 

PKI: Public Key Infrastructure, framework of certificate authorities, digital certificates, software, services, and other cryptographic components deployed for the purpose of validating subject identities. 

In-band authentication: Use of a communication channel that is the same as the one currently being used. 

Microservices is a software architecture in which solution components are conceived as highly decoupled services that are not dependent on a single platform technology. 

PAM: Privileged Access Management, Policies, procedures, and support software for managing accounts and credentials with administrative permission. 

Application Virtualization is a software delivery model in which the code runs on a server and is streamed to a client. 

Reverse Proxy: A proxy server that protects servers from direct contact with client requests. 

SAML: Security Assertion Markup Language, An XML-based data format used to exchange authentication information between a client and a service. 

Shibboleth: An identity federation method that provides SSO capabilities and enables websites to make informed authorization decisions for access to protected online resources. 

SOAP: Simple Object Access Protocol, An XML-based web service protocol that is used to exchange messages. 

SASE: Secure Access Service Edge, A networking and security architecture that provides secure access to cloud applications and services while reducing complexity. It combines security services like firewall, identity and access management, and secure web gateway with networking services such as SD-WAN

SDN: Software Defined Network, APIs and compatible hardware/virtual appliances allowing for programmable network appliances and systems. 

Serverless: A software architecture that runs functions within virtualized runtime containers in a cloud rather than on dedicated server instances. 

VPC: Virtual Private Cloud, A private network segment made available to a single cloud consumer on a public cloud. 

# Win Registry
The Windows registry is a database for storing OS device and software application configuration information. It is comprised of a set of five root keys that contain computer and user databases. 

HKLM Database: Governs system-wide settings
HKEY_USERS database: includes settings that apply to individual user profiles such as desktops. 
HKEY_CURRENT_USER: is a subset of HKEY_USERS for the logged-in user. 

The registry database is stored in binary files called hives. Hives comprise a single file LOG, SAV, ALT (Backup)

Win Registry files stored in C:\Windows\System32\Config

Sub key | Description
SAM | Security Accounts Manager stores username information for accounts used  on the current computer
Security | Linked to the security database of the domain the current user is logged into.
SOFTWARE | Contains settings for software and Windows OS.
DEFAULT | Contains settings for the LocalSystem account profile. 


# Network functions
CLould plane: Makes decisions about how traffic should be prioritized and secured, and where it should be switched

Data plane: Handles the actual switching and routing of traffic and the imposition of ACL for security. 

Management plane: Monitors traffic conditions and network status. 


# DLP Examples
Blocking use of external Media

Print Blocking: Preventing the printing of sensitive information or controlled documents. This particularly imporant in the healthcare industry. 

RDP Blocking: RDP allows for data to be copied and pasted from the session. 

Clipboard privacy controls: Limiting access to the clipboard and preventing sensitive data from being placed on the clipboard for use elsewhere. 

Restricted Virtual Desktop Infrastructure: Incorporating CLP features within the underlying DI infrastructure to protect all virtual desktops and govern how data is used and shared in the environment

Data Classification blocking: Use metadata or other mechanisms to tag data with its classification in order to limit how it can be accessed and used. 

# Logging Levels
Debug: Used for debugging purposes. 
INFO: Used for informative messages
Warning: used to indicate a potential problem
Error: Used to indicate a serious problem
Critical: Used to indicate a critical problem. 

Syslog uses eight logging levels
0 Emergency: System is unusable
1 Alert: Immediate action required
2 Critical: critical conditions
3 Error: Error condition
4 Warning warning conditions
5 Notice: Normal but significant conditions
6 Information: Information message
7 Debug: Message helpful for debugging. 
