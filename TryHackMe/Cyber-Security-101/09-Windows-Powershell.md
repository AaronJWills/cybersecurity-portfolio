# TryHackMe : Windows Powershell
https://tryhackme.com/room/windowspowershell

**Path:** Cyber Security 101
**Completed:** 27 March, 2026
**Difficulty:** Easy

##Overview
Powershell basics

## Key Skills Practised
- Navigating and working with files
- Piping, Filtering and sorting data
- System and network information
- Real-Time System Analysis 
- Scripting

## Useful Commands / Tools
- Get-Command to show all available cmdlets 
- Get-Alias - shows all alternative shortcut names for cmdlets, eg cd, dir
- Standard Powershell syntax - Cmdlets -Property "pattern*"
Examples - get-help *cmdlets* -examples
- Get-ChildItem
- Set-Location -Path "path"
- New-Item (could be file or directory) 
- Copy-Item
- Move-Item
- Get-Content - display contents of file, like type or cat
eg. Get-ChildItem | Sort-Object Length -Descending | Select-Object -First 1
- Select-String - for finding text in files
- Get-ComputerInfo - even more handier than the systeminfo CMD command
- Get-LocalUser, Get-NetIPConfiguration, Get-NetIPAddress
- Get-Process, Get-Service, Get-NetTCPConnection, Get-FileHash
- To see any hidden streams attached to a file - eg Get-Item -Path "folder\file" -Stream *
- Invoke-Command for running scripts and commands remotely 
eg. Invoke-Command -FilePath c:\scripts\test.ps1 -ComputerName Server01
- Invoke-Command -ComputerName Server01 -Credential Domain01\User01 -ScriptBlock {Command}

## Screenshots


## Takeaway for Security Roles

