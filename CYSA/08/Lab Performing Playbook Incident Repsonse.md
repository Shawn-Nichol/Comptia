# Powerhsell

Change the current directory to the root of C, then searches all sub-folders for the file heavyloade.exe
```
cd c:\; Get-ChildItem -Path "C:\" -Recurse -File -ErrorAction SilentlyContinue | Where-Object { $_.Name -eq "HeavyLoad.exe" }.
```

Create a file that stores the hash of the exe
```
get-filehash -Path "C:\Users\HeavyLoad.exe" -Algorithm SHA256 > HeavyLoad-Hash.txt
```

Display txt file in powershell
```
type HeavyLoad-Hash.txt
```

Obtain the owner of the file
```
(Get-Acl -Path "C:\Users\HeavyLoad.exe").Owner
```

Create zip file
```
Compress-Achrive -Path "C:\Users\HeavyLoad.exe", C:\Users\HeavyLoad-Hash.txt" -DestinationPath "C:\HeavyLoad.zip"
```

delete files and then overwrite three times. (System Internals)
```
sdelete -p 3 C:\Users\HeavyLoad*
```


