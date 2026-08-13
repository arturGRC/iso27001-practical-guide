# Incident Scenario (Worked Example): Lost Clinician Tablet

**Supports:** Incident Management Procedure | Controls A.5.24–A.5.27 | Demonstrates Risk R-001 materializing

This is a fictional but realistic walkthrough of the Incident Management Procedure in `06. Procedures` applied end-to-end, showing how the generic procedure becomes a real, timed response.

---

## Timeline

**Day 1, 2:40 PM** — A home health nurse reports her agency-issued tablet was stolen from her vehicle during a patient visit in a parking lot.

**2:45 PM — Detect & Report.** Nurse calls the IT helpdesk per the Mobile Device & BYOD Policy ("report within 1 hour"). Incident logged as `INC-2026-014`, Severity: **High** (device may contain cached PHI for that day's patient roster of 8 patients).

**2:52 PM — Triage & Classify.** On-call IT confirms the tablet was MDM-enrolled and encrypted (control from Mobile Device Policy worked as designed). Severity held at High pending confirmation of remote wipe success.

**2:58 PM — Contain.** IT triggers remote wipe via MDM console. Device credentials (EHR session token) revoked immediately. Tablet's network access blocked at the EHR gateway.

**3:15 PM — Confirm containment.** MDM confirms wipe command executed successfully before the device went offline (device had briefly connected to a cell tower, giving the wipe command a window). Risk downgraded: no PHI was actually exfiltrated, but the incident remains open pending full investigation, because full-disk encryption plus a successful wipe reduces — but does not by itself eliminate — reporting obligations.

**Day 1, 4:30 PM — Eradicate & Recover.** New tablet provisioned and shipped overnight to the nurse; her EHR access re-enabled on the new device only after MFA re-enrollment.

**Day 2 — Notify (decision point).** Compliance Officer performs a HIPAA breach risk assessment (four-factor test): Was PHI actually accessed/acquired? Given confirmed encryption + confirmed successful remote wipe + police report filed, the Compliance Officer determines this **does not rise to a reportable breach** under HIPAA's low-probability-of-compromise standard — but documents the full four-factor analysis in writing regardless, because that documentation is itself the evidence an auditor or OCR investigator will ask for.

**Day 3 — Post-Incident Review.** Root cause discussed: the tablet was left visible on the passenger seat rather than in the (agency-provided) lockbox. Contributing factor: lockbox use wasn't reinforced in the last training cycle.

## Corrective Actions Raised (feeds into `07. Templates/corrective-action-report-template.md`)
| Action | Owner | Due Date |
|---|---|---|
| Add "visible device in vehicle" scenario to next quarterly security awareness refresher | Training Coordinator | 30 days |
| Audit lockbox distribution — confirm all 180 field clinicians actually have one | Clinical Ops Manager | 14 days |
| Re-verify MDM remote-wipe success rate across last 12 months of lost-device incidents (trend check) | IT Director | 30 days |

## Why this scenario matters for the ISMS
This single incident touches nearly every clause in the loop: **Clause 8** (the operational control — encryption + MDM — worked), **Clause 9** (the post-incident review is a form of evaluation), and **Clause 10** (three real corrective actions were raised). It also shows R-001 from the Risk Register moving from a theoretical score of 15 to a demonstrated, contained, low-impact event — the kind of evidence an auditor wants to see, because it proves the control actually functions under pressure, not just on paper.
