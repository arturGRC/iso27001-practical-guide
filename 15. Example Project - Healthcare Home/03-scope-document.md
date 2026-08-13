# ISMS Scope Document — Hearthside Home Health

**Supports:** Clause 4.3

## Scope Statement
The ISMS covers the people, processes, and technology involved in the collection, storage, transmission, and disposal of Protected Health Information (PHI) across Hearthside Home Health's care delivery operations, specifically: the cloud-hosted EHR platform, the telehealth video platform, agency-issued clinician devices used in patient homes, the corporate office network (Springfield, IL), and the Remote Patient Monitoring (RPM) device integration pipeline.

## In Scope
- EHR platform (hosted on [Cloud Provider], HIPAA-eligible service tier)
- Telehealth video platform and its integration with the EHR
- Agency-issued clinician laptops and tablets (approx. 210 devices)
- Corporate office network and on-site staff (40 employees, Springfield, IL headquarters)
- RPM device data pipeline (device → gateway → EHR ingestion)
- Scheduling and dispatch system
- Clinician onboarding/offboarding processes affecting system access

## Out of Scope (with justification)
- **Payroll/HR platform** — hosted and fully managed by a separate SOC 2-audited third party; no PHI processed; excluded from ISMS scope but covered under Vendor Security Policy oversight
- **Marketing website** — public, no PHI, static content only
- **Patient-owned devices** used only to *view* their own care plan via a patient portal — patients are data subjects, not part of the organization's ISMS, though the portal *platform* itself is in scope
- **Physical therapy equipment** with no data connectivity (non-networked equipment)

## Interfaces & Dependencies
- Dependency on cloud provider's underlying infrastructure security (shared responsibility model — documented in Vendor Security assessment of the cloud provider)
- Dependency on RPM device manufacturers' firmware security (limited direct control — treated as a residual risk, see Risk Register R-004)

## Approval
Approved by Hearthside's CEO and Compliance Officer; reviewed annually and upon entry into any new service line (e.g., adding a new RPM device type).
