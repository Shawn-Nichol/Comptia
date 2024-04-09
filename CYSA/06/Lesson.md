SCAP: Security Content Automation Protocol, A NIST framework that outlines various accepted practices for automating vulnerability scanning.

# SCAP Languages
OVAL: Open Vulnerability and Assessment Language, An XML schema maintained by MITRE, for describing system security state and querying vulnerability reports and information

ARF: Asset Reporting Format. As the name suggests, ARF helps to correlate report formats to assess information independently from any specific application or vendor product for consistency and interoperability. 

EXXCF: Written in XML, XXCCDF provides a consistent and standardized way to define benchmark information as well as configuration and security checks to be performed during an assessment. 

# SCAP Identification Schemes
CPE: Common Platform Enumeration, Scheme for identifying hardware devices, operating systems, and applications developed by MITRE. 

CVE: Common Vulnerabilities and Exposures, a Scheme for identifying vulnerabilities developed by MITRE and adopted by NIST.

CCE: Common Configuration Enumeration, Scheme for provisioning secure configuration checks across multiple sources developed by MITER and adopted by NIST. 


# CVSS Scoring Calculation
1. Identify the threat agent.
2. Identify the affected systems. This includes identifying the product name and type of system
3. Assign a score based on impact
4. Identify the probability of the threat agent accessing the system.
5. Calculating the overall CVSS score.

CVSS Vector string: A string that provides more context around the scoring metrics used to calculate the overall CVSS score. The string is broken into fields that include the vulnerability identifier, the impact, the environmental concerns, and the additional information. 

# Vulnerability Scan results
False Positive: When a Vulnerability scan incorrectly indicates that a vulnerability or misconfiguration is present when it is not.

True Positive: When a vulnerability scan correctly identifies a vulnerability. 

False Negative: When a vulnerability scan incorrectly identifies that a vulnerability does not exist. 

True Negative: A vulnerability scan that correctly indicates that a system or device does not have a vulnerability. 

# Vulnerability score factors
Availability of patches: 
Impact of Vulnerability: 
Level of sophistication of threat actors: The likelihood a threat actor can exploit a vulnerability. 
Asset value: 
Weaponization: Assesses the likelihood that an attacker will be able to weaponize a vulnerability to achieve their objectives. 
Exploitability: A vulnerability with high exploitability is more likely to be targeted by an attacker and therfore requires urgent attention. conversely, a vulnerability with low explooitability may be less urgent as it is less likely to be exploited. 
