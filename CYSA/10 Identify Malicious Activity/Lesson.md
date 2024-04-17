Kill Chain
1. Reconnaissance
2. Weaponization
3. Delivery
4. Exploitation
5. Installation
6. Command and control
7. Actin and objective



        Adversary
Infrastructure   Capability
          Victim


SOAR: Security orchestration Automation and Response is designed to automate some of the routine tasks ordinarily performed by security personnel in response to a security incident. 

MUA: Mail User agent creates the initial header and forwards the message to MDA.

MDA: Mail Delivery Agent checks that the sender is authorized to issue messages from the domain; the MDA adds or amends its own header and then transmits the message to an MTA

MTA: Message Transfer Agent routes the message to the recipient, using DNS to locate the recipient's MTA. The message passes via one or more additional MTAs. 

 SPF: Sender Policy Framework, A DNS record identifying hosts authorized to send mail for the domain. 

 DKIM: Domain Key Identified Mail, a Cryptographic authentication mechanism for mail utilizing a public key published as a DNS record. 

DMARC: Domain-based message authentication, reporting, and conformance. This is a framework ensuring proper application of SPF and DKIM, utilizing a policy published as a DNS record. 
