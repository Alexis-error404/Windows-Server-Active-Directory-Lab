# NIST Risk Management Framework (RMF) + POA&M Project

## Purpose
This project simulates how a GRC / RMF analyst would move a small Windows Server and Active Directory environment through the NIST Risk Management Framework and track weaknesses using a Plan of Action and Milestones (POA&M).

> **Portfolio disclaimer:** This is a simplified educational simulation and not an official federal authorization package.

# RMF Lifecycle

## 1. Prepare
### Objective
Establish context and readiness for managing security and privacy risk.

### Lab Activities
- Define the system boundary.
- Identify the Windows Server domain controller and joined clients.
- Identify administrator and user roles.
- Document expected system functions.
- Establish risk assumptions.

## 2. Categorize
### Example Security Impact
For this lab, the system is treated as a simplified **Moderate-impact** environment for training purposes.

Security objectives considered:
- Confidentiality
- Integrity
- Availability

## 3. Select Controls
Example NIST SP 800-53 controls selected:
- AC-2 Account Management
- AC-6 Least Privilege
- IA-2 Identification and Authentication
- IA-5 Authenticator Management
- AU-2 Event Logging
- AU-6 Audit Record Review
- CM-2 Baseline Configuration
- CM-6 Configuration Settings
- SI-2 Flaw Remediation
- IR-4 Incident Handling

## 4. Implement Controls
Examples:
- Configure password policy through Group Policy.
- Configure account lockout settings.
- Restrict privileged group membership.
- Enable Windows auditing.
- Establish patch procedures.
- Document incident response actions.

## 5. Assess Controls
Assessment methods include:
- Examine configuration screenshots.
- Interview the “system owner” (simulated).
- Test expected security behavior.
- Compare implementation against control requirements.
- Record findings and evidence.

## 6. Authorize
A real authorization decision would be made by an Authorizing Official based on:
- Security assessment results
- System Security Plan (SSP)
- POA&M
- Residual risk
- Other authorization package evidence

For this project, authorization is simulated as:

**Decision: Conditional Authorization for Training Purposes**

Condition: Critical and high-risk findings must have documented remediation milestones.

## 7. Monitor
Continuous monitoring activities:
- Review privileged access.
- Review security logs.
- Track patch status.
- Review open POA&M items.
- Reassess major configuration changes.
- Update risk register.

# Sample POA&M

| ID | Weakness | Related Control | Risk | Planned Remediation | Owner | Target | Status |
|---|---|---|---|---|---|---|---|
| POAM-001 | MFA not implemented for privileged access | IA-2 | Critical | Deploy MFA for administrative access | Security Admin | 30 days | Open |
| POAM-002 | Dormant accounts may remain enabled | AC-2 | High | Create quarterly access review and disable inactive accounts | System Admin | 45 days | In Progress |
| POAM-003 | Log review process not documented | AU-6 | Critical | Establish weekly security log review and escalation procedure | Security Analyst | 30 days | Open |
| POAM-004 | Patch tracking is informal | SI-2 | Critical | Establish monthly patch cycle and exception tracking | System Admin | 30 days | Open |
| POAM-005 | Incident response procedure missing | IR-4 | High | Write incident response playbook and conduct tabletop exercise | Security Lead | 60 days | Open |

# Sample SSP Content

## System Name
HomeLab Active Directory Environment

## System Description
A virtualized Windows Server environment used to provide Active Directory authentication, centralized account management, Group Policy and lab-based administration.

## System Boundary
- Windows Server domain controller
- Windows client endpoints
- Virtual network supporting the lab
- Administrative accounts used to manage the environment

## Security Responsibilities
**System Owner:** Defines system mission and accepts operational responsibility.

**System Administrator:** Implements and maintains technical controls.

**Security / GRC Analyst:** Assesses controls, documents risk, manages findings and tracks remediation.

**Authorizing Official:** Simulated role responsible for accepting residual risk.

# Evidence Package Structure

```
GRC/
├── NIST-800-53-Security-Assessment.md
├── Risk-Register.md
├── RMF-POAM-Project.md
└── evidence/
    ├── AC-2-account-review.png
    ├── AC-6-privileged-groups.png
    ├── IA-5-password-policy.png
    ├── AU-2-audit-policy.png
    └── SI-2-update-status.png
```

Screenshots can be added later from the live lab without exposing real credentials, names, IP addresses, tokens, or other sensitive information.

# Skills Demonstrated
- NIST RMF lifecycle
- POA&M development
- SSP concepts
- NIST SP 800-53 control mapping
- Risk assessment
- Security authorization concepts
- Continuous monitoring
- Remediation tracking
- GRC documentation

## Interview Talking Point
“I built a simulated RMF package around my Windows Server and Active Directory lab. I defined the system boundary, selected controls, assessed gaps, created a POA&M, documented SSP-style system information, and established continuous-monitoring activities. It gave me practical experience connecting technical configuration to governance and risk decisions.”
