// turbo-all
# /cso: Chief Security Officer Audit

Load identity: [persona-gstack-cso.md](file:///Users/kimjin/Library/CloudStorage/GoogleDrive-hongkimjin@gmail.com/My%20Drive/2026%20LLC/gStack-Antigravity/.antigravity/rules/persona-gstack-cso.md)

## Phase 1: Attack Surface mapping
1.  **Endpoints:** Grep for `get`, `post`, `put`, `delete` in `.js`, `.ts`, `.py`, `.rb`, `.go`.
2.  **Auth Boundaries:** Grep for `authenticate`, `authorize`, `jwt`, `cookie`, `session`.
3.  **Privileged Routes:** Grep for `admin`, `superuser`, `root`.

## Phase 2: OWASP Top 10 Audit
1.  **Injection:** Scan for `execute(`, `where("`, `raw(`, `system(`, `eval(`.
2.  **Auth Failures:** Check package versions for `npm audit` or `bundle audit`.
3.  **Config:** Check CORS and CSP headers in server configuration files.

## Phase 3: STRIDE Threat Model
1.  **Component Analysis:** For each major component (API, DB, UI), identify Spoofing, Tampering, and Elevation of Privilege risks.
2.  **Data Classification:** Categorize codebase data into Restricted, Confidential, or Internal.

## Phase 4: Security Posture Report
1.  **Findings:** List all findings with Sev >= MEDIUM and Confidence >= 8/10.
2.  **Exploit Scenario:** For each finding, provide a step-by-step attack path.
3.  **Remediation:** Present the top 5 findings with fix/mitigate/accept options.

## Disclaimer
Always include: **"This tool is not a substitute for a professional security audit."**
