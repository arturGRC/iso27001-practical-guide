# Example Project — Healthcare Home

A fully worked case study applying this toolkit to a fictional **home health and community care provider**. Every clause of ISO 27001 is populated with sector-realistic content so you can see the framework in motion, not just in the abstract.

> All names, patient data, and figures below are fictional and for illustration only.

## Organization Profile

**Hearthside Home Health** delivers in-home nursing, physical therapy, and remote patient monitoring (RPM) to ~4,200 patients across a regional service area, supported by 180 mobile clinicians, a 40-person corporate office, a cloud-hosted Electronic Health Record (EHR) platform, and a telehealth video platform. Hearthside is a HIPAA Covered Entity in the US and pursues ISO 27001 certification to satisfy payer and health-system partner security requirements alongside HIPAA.

## Why home healthcare is a distinctive ISMS scope

Unlike an office-based SaaS company, Hearthside's risk profile is defined by **information leaving the building**: PHI travels on clinician laptops into patients' homes, connects over unmanaged home Wi-Fi, and is captured by connected medical devices (RPM blood pressure cuffs, glucose monitors) that were never designed with enterprise security in mind. This example project shows how the standard's generic requirements translate into a mobile, health-data-heavy operating reality.

## What's in this folder

| File | Clause/Control | Shows |
|---|---|---|
| `01-context-of-organization.md` | Clause 4.1 | Healthcare-specific external issues (HIPAA, payer requirements, medical device threats) |
| `02-interested-parties.md` | Clause 4.2 | Patients, HHS/OCR, payers, referring hospitals as stakeholders |
| `03-scope-document.md` | Clause 4.3 | A realistic scope boundary — what's in vs. explicitly excluded |
| `04-risk-register.csv` | Clause 6.1 | 10 sector-specific risks, fully scored and treated |
| `05-statement-of-applicability-excerpt.csv` | Clause 6.1 | How Annex A controls get justified for a mobile health workforce |
| `06-mobile-device-and-byod-policy.md` | A.6.7, A.8.1 | A policy addressing clinician-owned and agency-owned field devices |
| `07-phi-data-classification-policy.md` | A.5.12, A.5.13 | Data classification specifically calibrated to PHI/HIPAA |
| `08-incident-scenario-lost-tablet.md` | A.5.24-A.5.27 | A full worked incident response walkthrough, start to finish |
| `09-completed-internal-audit-checklist.csv` | Clause 9.2 | A sample completed (not blank) audit checklist with real findings |
| `10-management-review-minutes-sample.md` | Clause 9.3 | A realistic completed management review |

## How to read this as a learning exercise

Follow the files in numeric order — they follow the same Plan → Do → Check → Act sequence as the clause guide in `docs/clause-guide.html`. Notice how the risk register (04) directly produces the SoA justifications (05), which in turn produce the two policies (06, 07), which get tested in the incident scenario (08) and verified in the audit (09) and management review (10). That chain **is** the ISMS operating.
