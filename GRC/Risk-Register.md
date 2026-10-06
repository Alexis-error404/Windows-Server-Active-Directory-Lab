# Cybersecurity Risk Register — Active Directory Lab

## Purpose
This risk register demonstrates how technical weaknesses can be translated into business risk, prioritized, assigned treatment decisions, and tracked to remediation.

> **Portfolio disclaimer:** Risks and ratings are simulated for a home-lab environment.

## Scoring Method
- Likelihood: 1 (Rare) to 5 (Almost Certain)
- Impact: 1 (Minimal) to 5 (Severe)
- Risk Score = Likelihood × Impact

### Rating Bands
- 1–4: Low
- 5–9: Moderate
- 10–14: High
- 15–25: Critical

## Risk Register

| ID | Risk | Likelihood | Impact | Score | Rating | Related Control | Treatment | Status |
|---|---|---:|---:|---:|---|---|---|---|
| R-001 | Privileged account compromise due to lack of MFA | 4 | 5 | 20 | Critical | IA-2 | Mitigate | Open |
| R-002 | Excessive Domain Admin privileges | 3 | 5 | 15 | Critical | AC-6 | Mitigate | Open |
| R-003 | Dormant user accounts remain enabled | 3 | 4 | 12 | High | AC-2 | Mitigate | In Progress |
| R-004 | Security events are not consistently reviewed | 4 | 4 | 16 | Critical | AU-6 | Mitigate | Open |
| R-005 | Systems fall behind on security patches | 3 | 5 | 15 | Critical | SI-2 | Mitigate | Open |
| R-006 | Weak or inconsistent security configuration | 3 | 4 | 12 | High | CM-6 | Mitigate | In Progress |
| R-007 | Incident response steps are undocumented | 3 | 4 | 12 | High | IR-4 | Mitigate | Open |

## Detailed Risk Example — R-001

### Risk Statement
If privileged accounts rely solely on passwords, then stolen credentials could allow an attacker to gain administrative access, resulting in unauthorized changes, data exposure, or disruption.

### Inherent Risk
Likelihood: 4  
Impact: 5  
Score: 20 — Critical

### Existing Controls
- Password authentication
- Account lockout policy
- Administrative group restrictions

### Treatment Plan
Implement multi-factor authentication for privileged accounts and remote administrative access.

### Target Residual Risk
Likelihood: 2  
Impact: 5  
Residual Score: 10 — High

### Risk Owner
System / Security Administrator

## Detailed Risk Example — R-004

### Risk Statement
If security logs are collected but not routinely reviewed, suspicious authentication or administrative activity may remain undetected.

### Treatment Plan
- Enable appropriate audit categories.
- Establish a weekly review process.
- Centralize logs where feasible.
- Define alert thresholds for repeated failed logons and privileged changes.

## Risk Treatment Options
A GRC analyst commonly documents one of four treatments:
- **Mitigate** — reduce likelihood or impact through controls.
- **Accept** — management knowingly accepts the residual risk.
- **Transfer** — shift some risk through contract/insurance/third party.
- **Avoid** — stop the activity creating the risk.

## Skills Demonstrated
- Risk identification
- Risk scoring
- Inherent vs. residual risk
- Risk treatment
- Control mapping
- Business-focused risk statements
- Remediation tracking

## Interview Talking Point
“I created a cybersecurity risk register for my Active Directory lab and mapped technical findings to business-readable risk statements. I scored likelihood and impact, identified associated NIST controls, selected treatment strategies, and documented expected residual risk.”
