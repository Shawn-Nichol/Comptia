# Windows Registry
HKEY_LOCAL_MACHINE (HKLM) database governs system wide settings
HKEY_USERS database includes setting that apply to individual user profiles, such as desktop personalization. 
HKEY_CURRENT_USER is a subset of HKEY_USERS with the settings for logged-in user.


The registry database is stored in binary files called hives. A hive comprises a single file, a .LOG file and a .SAV file

.LOG: containing a transaction log
.SAVE: a copy of the key as it was at the end of setup

The system hive also hasss an .ALT backup file. 

Most of these files are stored in the C:\WindowsSYSTEM32\Config\ folder, but the hive file for each user profile (NTUSER>DAT) is stored in the folder holding the user profile.

Windows Registry files stored
SAM: Security Accounts Manager stores username information for accounts used on the current computer
Security: Linked to the security database of the domain the current user is logged onto. 
Software: Contains settings for software and the windows OS
System: contains settings for drivers and file systems
Default: Contains settings for LocalSystem account profile. 

Physical segmentation: Involves separating different network zones using separate switches, routers and cabling

Virtual segmentation: Invloves using softare to create virtual networks within an existing network allowing different types of traffic to be separted and isolated. 

Logical Segmenation: Invloves using software to create logical divisions within a single network using virtual LANs or VLANs. 

Secure Access Service Edge: A netowrking and security architecture that provides secure access to cloud applications and services while reducing complexity. It combines security servcies like firewall, identity and access management and secure web gatgeway with networking services such as SD-WAN





