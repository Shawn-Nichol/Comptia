# Configuring Centralized logging
- Enabled windows event collector service on source computer
- Configured the firewall for remote log access on the source computer
- Windows remote management service on the collector computer
- Event Viewer Subscription

# Search logs with Regex (linux)
- Searched for Ipv4 addresses from a log file using grep and regex
- Learned how to use stacked grep searches.

- o  is used to show the matching string rather than the whole line
- Pforces grep to accept the Perl-compatible regular expression format rather than the basic format
```
grep -oP '[0-9]' kern.log
```

You can get a group of numbers by adding an astrix
```
grep -oP '[0-9]*' kern.log
```

add a dot to the search
```
grep -oP '[0-9]*\.' kern.log
```

search for any digit (d)
```
grep -oP '\d+\.\d+\.\d+' kern.log
```

Limit the digit groups to 1,2, 3 digits only with a pattern repeater
```
grep -oP 'd{1,3}\.\d{1,3}\.\d{1,3}' kern.log
```

Simplify regex by using a second-level pattern repeater
```
grep -oP '(\d{1,3}\.){3}\d{1,3}' kern.log
```

capture the output into a file
```
grep -oP '(\d{1,3}\.){3}\d{1,3}' kern.log > outputfile.txt
```

view the output in less viewer
```
grep -oP '(\d{1,3}\.){3}\d{1,3}' kern.log | less
```

line counter
```
grep -op '(\d{1,3}\.){3}\d{1,3}' kern.log | wd -l
grep 172.16.0.254 kern.log | wc -l
```

View enteries through less 
```
grep 172.16.0.254 kern.log --color=always | more
```

exclude occurrrences of of ruser
- v  inverts the matching result so that only lines without rusers are sent to the second grep  command to serach on user
```
grep -v ruser auth.log.1 | grep user
```

```
grep -v ruser auth.log.1 | grep -P 'user \w+' | grep sudo
grep -v ruser auth.log.1 | grep -P 'user \w+' | grep sudo | grep 'session opened'
grep -v ruser auth.log.1 | grep -P 'user \w+' | grep sudo | grep 'session opened' | wc -l
```

