Perform ping sweep
perform SYn scan top 100
Capture Nmap results into files
evaluated the results of Nmap scan output files
Identify services on open ports
OS identification
script scan


Nmap tags used
- sn: disables port scanning and only sends ICMP echo-request to each IP address. 
-sS specifies that Nmap should use a TCP SYN scan
-sV nmap performs version detection on the target ports. It tries to determine the version of the service running on the port by analyzing the response received.
- O enables OS detection attempts to determine the  target OS based on characteristics
- iL this tag specifies a list of target IP addresses or hostnames to scan
-F tells Nmap to perform a fast scan, which means it will only scan the most common 100 ports
-p- Scans all ports
-p1- Scans all ports
-p 1-65535
--banner enables version detection, which attempts to determine the version of the service running on the target port. 
-sV
-v or --vv verbose or Very verbose, which may cause Nmap to produce more output while performing complex and involved operations.
-oN specifies the normal output format for Nmap, 
-oA output scan results to three files (.nmap, .gnamp, .XML)
-oG output to greable
-oX output to XML
-oS output to samba-style.
 
ressing the space bar will also provide some feedback when the command is running.
Display the standard syntax for nmap
```
nmap | less
```

Ping Sweep
```
nmap 10.1.16.0/24 -sn -oN server_assets_pingsweep.nmap
```


```
nmap -iL targets.txt -F -sS -oA assets_fast_port_scan
```





