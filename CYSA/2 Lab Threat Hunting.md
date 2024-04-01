CMD command
Netstat is used to view current network connections and their status
- n forces number only to be displayed instead of hostnames
- o displays the associated process ID
- limits the display to the selected protocol in this case TCP
```
netstat -nop tcp
```

CMD Command
Tasklist to veiw all currently active processes
-fI is used to apply a filter to the output. The filter syntax must be in quotes and includes a filter name. 
```
tasklist:
```

Powershell command
Type: display a field. 
```
type outfile.txt
```
Linux
netstat similar to windows
- n forces numbers only  to be displayed instead of hostnames
- p displays the PID and process/program name
- --protocol=inet limits the display to only  IPv4 protocols.
```
netstat -np --protocol=inet
```





```
netstat -np --protocol=inet
```
