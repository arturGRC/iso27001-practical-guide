# PHI Data Classification Policy — Hearthside Home Health

**Supports:** Controls A.5.12, A.5.13 | HIPAA Privacy & Security Rule

| Document Control | |
|---|---|
| Document Owner | Compliance Officer |
| Approved By | CISO |
| Version | 1.0 |
| Review Cycle | Annual |

## 1. Purpose
General-purpose data classification (Public/Internal/Confidential/Restricted) is insufficient on its own for a HIPAA Covered Entity — this policy adds a PHI-specific layer on top of the base Data Classification Policy.

## 2. Classification Layer for Health Data
| Level | Definition | Example | Required Controls |
|---|---|---|---|
| PHI — Restricted | Individually identifiable health information | Diagnosis, treatment notes, vitals from RPM devices, insurance ID linked to a named patient | Encryption at rest & in transit, access logging, MFA, minimum-necessary access, BAA required for any third party touching it |
| De-identified Health Data | PHI with identifiers removed per HIPAA Safe Harbor | Aggregate outcomes reporting for quality metrics | Standard Confidential handling; no BAA required if truly de-identified |
| Operational — Internal | Business data with no patient linkage | Staffing schedules, mileage logs | Standard Internal handling |

## 3. Minimum Necessary Standard
Access to PHI — Restricted data is granted only to the extent needed for the specific job function (e.g., a scheduler sees appointment times but not clinical notes). Enforced through EHR role-based access, reviewed quarterly.

## 4. Business Associate Agreements (BAAs)
Any third party classified as touching PHI — Restricted data (billing vendor, telehealth platform, RPM device vendor, cloud host) must have a current, signed BAA before data is shared. Tracked in the Supplier Register (`12. Third-Party Risk`) with a BAA status column.

## 5. Retention & Disposal
PHI is retained per state medical records retention requirements (typically 7-10 years, longer for minors) and securely destroyed thereafter (cross-shredding for paper, certified wipe/destruction for electronic media) — see Asset Management Policy.
