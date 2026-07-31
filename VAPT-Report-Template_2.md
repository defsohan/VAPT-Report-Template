# Vulnerability Assessment & Penetration Testing Report

## Document Control

| Field | Details |
|---|---|
| Client Name | [Client / Organization Name] |
| Project Name | [Engagement Name] |
| Prepared By | Sohan Sardar (CEH) |
| Report Date | [DD/MM/YYYY] |
| Classification | Confidential |
| Version | 1.0 |

---

## 1. Executive Summary

Brief, non-technical summary of the engagement — what was tested, when, and the overall security posture observed. Should be readable by a non-technical stakeholder (e.g. business owner, manager).

**Overall Risk Rating:** [Critical / High / Medium / Low]

**Summary of Findings:**

| Severity | Count |
|---|---|
| Critical | 0 |
| High | 0 |
| Medium | 0 |
| Low | 0 |
| Informational | 0 |

---

## 2. Scope of Engagement

| Item | Details |
|---|---|
| Target(s) | [URLs / IP ranges / applications tested] |
| Testing Type | [Black-box / Grey-box / White-box] |
| Testing Window | [Start date] – [End date] |
| Excluded from Scope | [Anything explicitly out of scope] |
| Authorization | Testing conducted under written authorization from [Client] dated [date] |

---

## 3. Methodology

Testing followed a structured approach aligned with industry-standard frameworks (e.g. OWASP Testing Guide, PTES):

1. **Reconnaissance** — passive and active information gathering
2. **Scanning & Enumeration** — identifying live hosts, open ports, services, technologies
3. **Vulnerability Analysis** — identifying potential weaknesses
4. **Exploitation** — validating vulnerabilities through controlled, safe exploitation
5. **Post-Exploitation** — assessing impact and potential for lateral movement (where in scope)
6. **Reporting** — documenting findings with evidence and remediation guidance

---

## 4. Risk Rating Methodology

Findings are rated using **CVSS v3.1** as a base, mapped to the following severity bands:

| CVSS Score | Severity |
|---|---|
| 9.0 – 10.0 | Critical |
| 7.0 – 8.9 | High |
| 4.0 – 6.9 | Medium |
| 0.1 – 3.9 | Low |
| 0.0 | Informational |

---

## 5. Findings Summary Table

| ID | Finding | Severity | CVSS | Status |
|---|---|---|---|---|
| VAPT-001 | [Finding title] | [Severity] | [Score] | Open |
| VAPT-002 | [Finding title] | [Severity] | [Score] | Open |

---

## 6. Detailed Findings

> Duplicate this block for each finding. See `Sample-Finding.md` for a filled example.

### VAPT-00X: [Finding Title]

| Field | Details |
|---|---|
| Severity | [Critical / High / Medium / Low] |
| CVSS v3.1 Score | [Score + vector string] |
| Affected Component | [URL / endpoint / host] |
| Status | Open |

**Description**
[What the vulnerability is, in technical terms]

**Evidence**
[Screenshots, request/response snippets, PoC steps — redact sensitive data before publishing anywhere]

**Impact**
[What an attacker could achieve by exploiting this]

**Remediation**
[Clear, actionable fix guidance — specific enough for a developer to implement]

**References**
[OWASP / CWE / CVE links if applicable]

---

## 7. Conclusion & Recommendations

Summary of overall posture and prioritized next steps — what to fix first, and any broader process recommendations (e.g. patch management, secure SDLC practices).

---

## 8. Appendix

**Tools Used:** [e.g. Burp Suite, Nmap, Nikto, sqlmap]

**Disclaimer:** This report is confidential and intended solely for [Client Name]. Testing was performed within the agreed scope and time window. Findings reflect the security posture at the time of testing only.
