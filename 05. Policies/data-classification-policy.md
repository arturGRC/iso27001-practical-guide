# Data Classification Policy

**Supports:** Control A.5.12, A.5.13

| Document Control | |
|---|---|
| Document Owner | [CISO] |
| Version | 1.0 |
| Review Cycle | Annual |

## 1. Purpose
To ensure information is classified and handled according to its sensitivity and value to the organization.

## 2. Classification Levels
| Level | Definition | Example | Handling |
|---|---|---|---|
| Public | No harm if disclosed | Marketing material | No restrictions |
| Internal | Limited harm if disclosed externally | Internal memos, org charts | Employees only |
| Confidential | Significant harm if disclosed | Contracts, financials, source code | Need-to-know, encrypted at rest |
| Restricted | Severe harm — legal/regulatory exposure | Customer PII, health data, credentials | Encrypted, access logged, DLP enforced |

## 3. Labeling
All documents and data stores must be labeled with their classification. Systems storing Restricted data require additional controls (encryption, access logging, DLP) per the Access Control and Backup Policies.

## 4. Handling Requirements
Handling requirements (storage, transmission, disposal) scale with classification level — see full handling matrix maintained by [CISO].
