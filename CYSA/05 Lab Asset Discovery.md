Perform ping sweep
perform SYn scan top 100
Capture Nmap results into files
evaluated the results of Nmap scan output files
Identify services on open ports
OS identification
script scan

Display the standard syntax for nmap
```
nmap | less
```

Ping Sweep
- sn: disables port scanning and only sends ICMP echo-request to each IP address. 
- nmap 
```
nmap 10.1.16.0/24 -sn -oN server_assets_pingsweep.nmap
```

-iL this tag specifies a list of target IP addresses or hostnames to scan
-F tells Nmap to perform a fast scan, which means it will only scan the most common 100 ports
-sS specifies that nmap should use a TCP SYN scan
-oA tells Nmap to output the scan results in three formats: XML, grepable, and regular.
```
nmap -iL targets.txt -F -sS -oA assets_fast_port_scan
```

nmap: -v or --vv 
- verbose or Very verbose, which may cause Nmap to produce more output while performing complex and involved operations. 
ressing the space bar will also provide some feedback when the command is running.


-sV nmap performs version detection on the target ports. It tries to determine the version of service running on the port by analyzing the response received. 
-oN specifies the normal output format for nmap, 
