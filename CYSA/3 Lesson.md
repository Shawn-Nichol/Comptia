# Windows Registry
HKEY_LOCAL_MACHINE (HKLM) database governs system-wide settings
HKEY_USERS database includes settings that apply to individual user profiles, such as desktop personalization. 
HKEY_CURRENT_USER is a subset of HKEY_USERS with the settings for logged-in users.


The registry database is stored in binary files called hives. A hive comprises a single file, a .LOG file, and a .SAV file.

.LOG: containing a transaction log
.SAVE: a copy of the key as it was at the end of the setup

The system hive also has an .ALT backup file. 

Most of these files are stored in the C:\WindowsSYSTEM32\Config\ folder, but the hive file for each user profile (NTUSER>DAT) is stored in the folder holding the user profile.

Windows Registry files stored
SAM: Security Accounts Manager stores username information for accounts used on the current computer
Security: Linked to the security database of the domain the current user is logged onto. 
Software: Contains settings for software and the Windows OS
System: contains settings for drivers and file systems
Default: Contains settings for LocalSystem account profile. 

Physical segmentation: Involves separating different network zones using separate switches, routers, and cabling

Virtual segmentation: Involves using software to create virtual networks within an existing network, allowing different types of traffic to be separated and isolated. 

Logical Segmentation: Involves using software to create logical divisions within a single network using virtual LANs or VLANs. 

Secure Access Service Edge is a networking and security architecture that provides secure access to cloud applications and services while reducing complexity. It combines security services like firewall, identity and access management, and secure web gateway with networking services such as SD-WAN.


PAM: Privileged Access Management, Policies, procedures, and support software for managing accounts and credentials with administrative permissions. 

Federation: A process that provides a shared login capability across multiple systems and enterprises. It essentially connects the identity management services of multiple systems.

Open ID: An identity federation method that enables users to be authenticated on cooperating websites by a third-party authentication service.

SAML: Security Assertion Markup Language, an XML-based data form used to exchange authentication information between a client and a service. 

SOAP: Simple Object Access Protocol, an XML-based web services protocol that is used to exchange messages. 

Shibboleth: an identity federation method that provides SSO capabilities and enables websites to make informed decisions for access to protected online resources. 

Trust Model: IN PKE a description of how users and different CAAs exchange information and certificates. 

CASB: Cloud Access Security Broker, Enterprise management software designed to mediate users' access to cloud services across all types of devices. 


# Data Loss Prevention
Policy server - configure classification confidentiality, privacy rules, and policies, and log incidents and compile reports
Endpoint Agents - To enforce policy on client computers even when they are not connected to the network
Network Agents - To scan communications at network borders and interface with web and messaging servers to enforce policy.


Remediation
Alert Only - copying is allowed, but the management system records an incident and may alert the admin.
Block - The user is prevented from copying the original file but retains access
Quarantine - Access to the original file is denied to the user. This could be accomplished by encrypting the file in place or by moving it to a quarantine area in the file system. 
Tombstone - The original file is quarantined and replaced with one describing the policy violation and how the user can re-release it. 

# Public Key Infrastructure
PKI - Framework for certificate authorities, digital certificates, software, services, and other cryptographic components deployed for the purpose of validating subject identities. 

SSL - Secure Socket Layer, The original obsolete version of the security protocol now developed as TLS

# Logging levels
Debug:
INFO:
Warning: indicate potential problems
Error: indicates a serious problem
Critical: used to indicate a critical problem

Syslog, uses eight logging levels
0 Emergency: system unstable
1 Alert Immediate Action required
2 Critical condition
3 Error: Error condition
4 Warning: Warning condition
5: Notice: normal but significant condition
6: Information: information message
7: Debug


Summary
- Cloud platforms enable unprecedented levels of flexibility
- Hardening software and OS help reduce the surface of its attack.
- Identity and access management tools enforce access controls
- Enriched log data provides near real-time insight into network activities. 
