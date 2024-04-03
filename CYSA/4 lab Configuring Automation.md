# automate iptables IP restrictions
Create a script to create firewall rules form a threat feed
auomtated the IP blocking script
adjusted the script to address rule duplicates. 

Add IP table rules
```
iptables -A INPUT -s 5.134.128.0/19 -j DROP
```
Show IP table rules
```
iptables -S
```

0 : The minute when the job should run.
1 : The hour when the job should run (1 AM).
* : The day of the month when the job should run (every day).
* : The month when the job should run (every month).
* : The day of the week when the job should run (every day of the week).
/bin/bash : specifies that the job should be run using the Bash shell
/root/ip_block.sh : the path to the script that should be executed.
```
echo "0 1 * * * /bin/bash /root/ip_block.sh" | crontab -
```

view scheduled tasks
```
crontab -l
```

# Automate malware removal based on threat feed
Viewed a simulated mawlare threat feed
viewed and edited a script to use IoC observables from the threat feed to remove malware
Execute the malware removal script, confirmed its operation and scheduled it to run daily. 


# Automation ob block DNS resolution based on threat feed. 
crafted a script to update the etc hosts file to block malicious DNS name resolution
Tested the DNS resolution of the malicous FQDN and confirmed the blocking protection
