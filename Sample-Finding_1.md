# Sample Finding (for reference)

This shows how a finding from the template's Section 6 looks once filled in. Delete this file's content and replace with your own real findings when using the template — do not publish real client data.

---

### VAPT-001: SQL Injection in Login Form

| Field | Details |
|---|---|
| Severity | Critical |
| CVSS v3.1 Score | 9.8 (AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H) |
| Affected Component | `/login.php` — `username` parameter |
| Status | Open |

**Description**
The login form's `username` parameter does not sanitize user input before passing it into a SQL query, allowing an attacker to inject arbitrary SQL commands and bypass authentication or extract database contents.

**Evidence**
Submitting `admin' OR '1'='1' -- ` in the username field with any password returned an authenticated session for the `admin` account, confirming the injection.

**Impact**
An unauthenticated attacker could bypass login entirely, access any user account including administrative accounts, and potentially extract, modify, or delete the full contents of the underlying database.

**Remediation**
Use parameterized queries / prepared statements for all database interactions. Never concatenate user input directly into SQL strings. Apply input validation as a secondary control, and enforce least-privilege database accounts for the application layer.

**References**
- OWASP: A03:2021 – Injection
- CWE-89: SQL Injection
