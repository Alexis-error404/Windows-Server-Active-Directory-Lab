# Active Directory Deployment

Install Windows Server, configure a stable IP, install AD DS, and promote DC01 for a lab-only domain.

```powershell
Get-ADDomain
Get-ADForest
Get-Service NTDS,DNS
```

Verify AD Users and Computers and DNS. Capture role installation and healthy services without secrets.