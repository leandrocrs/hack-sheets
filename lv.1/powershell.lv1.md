```
# getting services 
Get-Service 
 
# you can use pipelines, like bash, to repass the output from last command to next one 
Get-Service | Where-Object Status -eq 'Running' 
 
# TIP: You can use <TAB> to autocomplete some command. Alternative: use command "ise" to open the ISE Gui Powershell editor. 
 
# Get all services, filter only the "Running" services, format to display only name and displayName, export to a CSV file  
Get-Service | Where-Object Status -eq 'Running' | Select-Object Name,DisplayName | Export-Csv C:\all-running-services.csv 
 
# get a list of all available commands in powershell and installed modules 
Get-Command 
 
# get a list of avaiable verbs on the system 
Get-Verb 
 
# Get services from another machine. OBS: maybe require another user account 
Get-Service -ComputerName <computername> 
 
# alias for Get-Service 
Gsv 
 
# getting-help from how use help system, sending output to more command, which brakes in screens 
Get-help | more 
 
# getting help with a specific command 
Get-Help <pattern to list commands or specific command> 
 
# show me how to do something 
Get-Help <specific command> -Examples 
 
# I want to see in browser 
Get-Help <specific command> -Online 
 
# learn about something 
Get-Help *about* 
```