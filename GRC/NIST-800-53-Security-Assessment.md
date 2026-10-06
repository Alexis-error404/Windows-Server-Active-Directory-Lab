# NIST SP 800-53 Security Assessment — Active Directory Lab

## Purpose
This project demonstrates how I would assess a Windows Server / Active Directory environment using selected NIST SP 800-53 Rev. 5 security controls.

> **Portfolio disclaimer:** This is a home-lab simulation created for educational and career-development purposes. It is not an official assessment of a production organization.

## Environment in Scope
- Windows Server domain controller
- Active Directory Domain Services
- Domain user and administrator accounts
- Group Policy Objects (GPOs)
- Windows client systems joined to the domain

## Assessment Method
For each control, I:
1. Identified the security objective.
2. Reviewed the lab configuration.
3. Defined expected evidence.
4. Recorded a simulated assessment result.
5. Documented risk and remediation actions.

## Control Assessment Matrix

| Control | Control Area | Expected Evidence | Assessment Result | Risk | Recommended Action |
|---|---|---|---|---|---|
| AC-2 | Account Management | AD user/account inventory, disabled account evidence | Partially Implemented | Stale accounts may retain access | Establish account review cadence and disable inactive accounts |
| AC-6 | Least Privilege | Privileged group membership, admin role assignments | Partially Implemented | Excessive privileges increase impact of compromise | Reduce Domain Admin membership and use dedicated admin accounts |
| IA-2 | Identification & Authentication | Authentication configuration, MFA evidence | Not Implemented in lab | Password compromise can lead to unauthorized access | Implement MFA for privileged and remote access |
| IA-5 | Authenticator Management | Password/GPO policy | Implemented with Improvement Needed | Weak password settings increase credential risk | Enforce stronger password and lockout settings |
| AU-2 | Event Logging | Windows audit policy and event logs | Partially Implemented | Security-relevant events may not be captured | Enable advanced audit policy categories |
| AU-6 | Audit Record Review | Defined log-review procedure | Not Implemented | Suspicious activity may go undetected | Create recurring log review and alert process |
| CM-2 | Baseline Configuration | GPO baseline/configuration documentation | Partially Implemented | Configuration drift may weaken security | Document and periodically validate secure baseline |
| CM-6 | Configuration Settings | Security-related GPO settings | Partially Implemented | Inconsistent settings can expose systems | Standardize GPO security settings |
| SI-2 | Flaw Remediation | Patch/update evidence | Partially Implemented | Unpatched vulnerabilities may be exploitable | Define patch cycle and track remediation |
| IR-4 | Incident Handling | Incident response procedure | Not Implemented | Response may be delayed or inconsistent | Establish incident triage, containment and recovery workflow |

## Example Finding — AC-2 Account Management

### Condition
The environment does not currently have a formally documented recurring account review process.

### Risk
Dormant or unnecessary accounts may remain enabled and could be abused by an unauthorized user.

### Evidence
- Active Directory Users and Computers account inventory
- Account status review
- Group membership review
- Last-logon information

### Recommendation
- Review user and privileged accounts every 90 days.
- Disable accounts that no longer have a business need.
- Document approval for privileged account creation.
- Separate normal user and administrative accounts.

### Residual Risk
Low to Moderate after the review process and disablement controls are implemented.

## Example Finding — AC-6 Least Privilege

### Condition
Privileged access should be limited to accounts that require administrative functions.

### Risk
Excessive administrative permissions increase the potential impact of credential compromise.

### Recommendation
- Maintain minimal membership in privileged AD groups.
- Use separate administrative credentials.
- Periodically review Domain Admins and other privileged groups.
- Document business justification for privileged access.

## Evidence Collection Checklist
- [ ] Screenshot of Domain Admins membership
- [ ] Screenshot of password policy GPO
- [ ] Screenshot of account lockout settings
- [ ] Screenshot of advanced audit policy
- [ ] Screenshot of Windows Event Viewer security logs
- [ ] Screenshot of disabled test account
- [ ] Screenshot of relevant GPO configuration

## Skills Demonstrated
- NIST SP 800-53 control interpretation
- Security control assessment
- Evidence collection
- Gap analysis
- Risk identification
- Remediation recommendations
- Active Directory security
- Technical-to-business risk communication

## Interview Talking Point
“I used my Active Directory lab as the system under assessment. I selected relevant NIST 800-53 controls, identified the evidence I would expect, documented gaps, assigned risk, and created remediation recommendations. The goal was to practice the same thought process used in GRC, RMF and security control assessment work.”
