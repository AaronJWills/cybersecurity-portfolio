# TryHackMe : Active Directory Basics

**Path:** Cyber Security 101
**Completed:** 22 March, 2026
**Difficulty:** Easy

##Overview
Basic concepts and functionality provided by Active Directory

## Key Skills Practised
- Active Directory management, OU's
- Group Policy
- Domain structure
- Security groups
- Kerberos Authentication

## Useful Commands / Tools
- Password reset via Powershell -   Set-ADAccountPassword username -Reset -NewPassword (Read-Host -AsSecureString -Prompt 'New Password') -Verbose
- Rest password on next logon -  Set-ADUser -ChangePasswordAtLogon $true -Identity username -Verbose

## Screenshots
<img width="838" height="177" alt="image" src="https://github.com/user-attachments/assets/5f19782e-97e8-4d31-94bf-cd6b15e0a11c" />

<img width="721" height="272" alt="image" src="https://github.com/user-attachments/assets/cc4750ad-2e55-440d-97cb-21b44f8192f6" />

<img width="706" height="303" alt="image" src="https://github.com/user-attachments/assets/f5526f38-5931-4e49-9a6e-9d59af951066" />

<img width="694" height="252" alt="image" src="https://github.com/user-attachments/assets/3d43831f-c56f-476c-b64b-fb017dfd2d99" />

<img width="744" height="310" alt="image" src="https://github.com/user-attachments/assets/18231cdf-e810-43b2-b91a-80fab3128b8c" />

## Takeaway for Security Roles
GPOs are distributed to the network via a network share called SYSVOL - C:\Windows\SYSVOL\sysvol\
Kerberos was  well explained (it's still complex!) and understood better by looking at these diagrams.  We always had problems with Kerberos tickets expiring for our SAP system, so this was quite helpful
Nicely explained domain/tree/forest diagram as well


