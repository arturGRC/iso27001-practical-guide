# Mobile Device & BYOD Policy — Hearthside Home Health

**Supports:** Controls A.6.7 (Remote Working), A.8.1 (User Endpoint Devices) | Addresses Risk R-001, R-009

| Document Control | |
|---|---|
| Document Owner | IT Director |
| Approved By | CISO / Compliance Officer |
| Version | 1.0 |
| Review Cycle | Annual |

## 1. Purpose
To protect PHI accessed or stored on devices used outside Hearthside's physical office, reflecting the reality that most clinical work happens in patients' homes.

## 2. Device Categories
| Category | Use Case | Security Baseline |
|---|---|---|
| Agency-issued laptop | Full EHR access, clinical documentation | Full-disk encryption, MDM-enrolled, EDR installed, auto-lock after 5 min |
| Agency-issued tablet | Field vitals capture, RPM device pairing | MDM-enrolled, app allow-listing, remote wipe capability |
| Clinician-owned BYOD (scheduling only) | View shift schedule, non-PHI logistics | No PHI permitted; app-level restriction enforced server-side; annual acknowledgement required |

## 3. Requirements
- **No PHI on personal devices.** BYOD devices are technically restricted from accessing the EHR clinical module — only the scheduling app, which contains no patient health data, is permitted
- Agency-issued devices require full-disk encryption before first EHR login (ties to Risk R-001)
- MFA is required for EHR access regardless of device (ties to Risk R-003)
- Lost or stolen devices must be reported within 1 hour of discovery to enable remote wipe — every hour of delay materially increases breach notification exposure under HIPAA
- Devices are re-imaged and access reverified before reassignment to a new clinician

## 4. Field-Specific Guidance
- Never leave an agency device visible in an unattended vehicle
- Use agency-provided mobile hotspot rather than unknown home Wi-Fi where patient vitals are being transmitted live
- Screen lock immediately when a visit is interrupted, even briefly

## 5. Enforcement
Non-compliance is addressed under the Acceptable Use Policy disciplinary process. Device compliance is checked as part of the quarterly access review (User Access Management Procedure).
