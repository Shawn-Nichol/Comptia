Preventivie controls: Attempt to stop an unwanted activity from taking place

In share, Select security, remove permissions to dedicated folder to block unathorized user access to server devices. 

# Detective controls. 
Records a log each time an event takes places. 


Enabled DLP on folder and sub folder. By  enagbled local Seucrity policy

- File Explorer: Local Security policy
- Local Policies
- Audit Policy
- Audit Object accesss
- Success and Failure

- Select Folder
- Properties
- Security
- Advanced
- Auditing
- add
- Select a principle
- Name Everyone
- Replace all child object auditing setting

Now you can Even Viewer will record files being deleted form this folder. 
Event ID 4660: object deletion, does not contain the actual object deleted
Event ID 4663: contains the object deleted information

# directive Conrol
Provides insturction to direct a user towards more compliant behavior. 

Used the  following powershell commands to create a banner when user is logging into the computer. 
```
$BannerText = "This computer system is the property of the CySA+ Online Lab. It is for authorized use only. By using this system, all users acknowledge notice of, and agree to comply with, the Acceptable Use Policy (AUP). Unauthorized or improper use of this system may result in administrative disciplinary action, civil charges/criminal penalties, and/or other sanctions as set forth in the AUP. By continuing to use this system, you indicate your awareness of and consent to these terms and conditions of use. If you are physically located in the European Union, you may have additional rights per the GDPR. Visit the website gdpr-info.eu for more information."

New-ItemProperty -Path "HKLM:\Software\Microsoft\Windows\CurrentVersion\Policies\System" -Name "legalnoticecaption" -Value "Authorized Use Only" -PropertyType "String" -Force | Out-Null

New-ItemProperty -Path "HKLM:\Software\Microsoft\Windows\CurrentVersion\Policies\System" -Name "legalnoticetext" -Value $BannerText -PropertyType "String" -Force | Out-Null
```


# Corrective control 
Acorrective control is intended to detect when something is in a less secure or less desirable state, then attemtps to return to the more secure or more desriable state. 

System internal "notmyfault" crashes the computer

Powershell instructions
```
"This is important" | Set-Content notes.txt.
Get-FileHash ./notes.txt -Algorithm SHA256 | Select-Object -ExpandProperty Hash | Set-Content ./hash.txt.
```
This command adds to the notes file. 
```
echo blah >> notes.txt.
```
This command calculates the hash of notes and compares it the value stored in the hash.txt. Since the file has changed an error message is displayed
```
if((Get-FileHash ./notes.txt -Algorithm SHA256).Hash -eq (Get-Content ./hash.txt)) {Write-Host "The file is correct."} else {Write-Host "The file has changed. Corrective action should be initiated."}.
```
