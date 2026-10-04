# Windows Server & Active Directory Enterprise Lab

**Windows Server • Active Directory • GPO • PowerShell • Help Desk**

## Project Summary
Build an enterprise-style Microsoft domain and demonstrate the identity, policy, file-access, automation, and troubleshooting tasks expected in IT support and systems-administration roles.

This repository is structured as a portfolio project: architecture, implementation, validation, security considerations, troubleshooting, and screenshot evidence are documented so the work can be reproduced and discussed in a technical interview.

## Architecture
```text
Windows Clients
      |
 Active Directory Domain
      |
 +----+-------+---------+
 |            |         |
AD DS        DNS       DHCP
 |
OUs / Users / Groups
 |
GPO + File Permissions
```

## Core Skills
- Windows Server
- AD DS
- DNS
- DHCP
- Group Policy
- NTFS
- SMB
- PowerShell
- IAM
- Help Desk

## Project Documentation
1. [Server And Domain Design](docs/01-server-and-domain-design.md)
2. [Active Directory Deployment](docs/02-active-directory-deployment.md)
3. [Users Groups And Ous](docs/03-users-groups-and-ous.md)
4. [Dns And Dhcp](docs/04-dns-and-dhcp.md)
5. [Group Policy](docs/05-group-policy.md)
6. [File Server And Permissions](docs/06-file-server-and-permissions.md)
7. [Powershell Administration](docs/07-powershell-administration.md)
8. [Helpdesk Scenarios](docs/08-helpdesk-scenarios.md)
9. [Screenshot Evidence](images/README.md)

## Validation Standard
For every major component I document:
1. **Purpose** — why the component exists.
2. **Configuration** — how I deployed it.
3. **Validation** — commands/tests proving it works.
4. **Troubleshooting** — likely failure points and diagnostic steps.
5. **Security** — how access and exposure are reduced.
6. **Evidence** — sanitized screenshots of the completed work.

## Portfolio Safety
No real passwords, secrets, API tokens, private keys, product keys, recovery codes, personal data, or sensitive public-facing configuration should be committed.

## What This Project Demonstrates
Rather than only listing technologies on a résumé, this lab provides evidence of planning, implementation, administration, documentation, troubleshooting, and security-minded decision making.

## Author
**Alexis Wiscovitch** — [@Alexis-error404](https://github.com/Alexis-error404)
