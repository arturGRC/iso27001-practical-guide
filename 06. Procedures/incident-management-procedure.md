# Incident Management Procedure

**Supports:** Incident Response Policy | Controls A.5.24-A.5.27

## 1. Purpose
Operational steps for detecting, responding to, and closing information security incidents.

## 2. Procedure
1. **Detect & Report** — Incident identified (by monitoring, employee report, or third party) and logged via Security Incident Form
2. **Triage & Classify** — Severity assigned (Critical/High/Medium/Low) based on impact and data sensitivity involved
3. **Contain** — Immediate actions to limit spread/damage (isolate host, disable account, block IP)
4. **Eradicate** — Remove root cause (patch, remove malware, close vulnerability)
5. **Recover** — Restore affected systems from clean backups; verify integrity before returning to production
6. **Notify** — Legal/CISO assess regulatory and contractual notification obligations (e.g., breach notification within 72 hours under GDPR)
7. **Post-Incident Review** — Root cause analysis and lessons-learned session within [5 business days] of closure; corrective actions logged in `08. Records/Corrective Actions`

## 3. Severity & Response Time Targets
| Severity | Initial Response | Resolution Target |
|---|---|---|
| Critical | 15 min | 4 hours |
| High | 1 hour | 24 hours |
| Medium | 4 hours | 5 days |
| Low | 1 business day | 15 days |

## 4. Records
All incidents logged in `08. Records/Incident Logs`, closed incidents summarized quarterly for Management Review.
