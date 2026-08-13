# Backup Policy

**Supports:** Control A.8.13 (Information Backup)

| Document Control | |
|---|---|
| Document Owner | [IT Operations Manager] |
| Version | 1.0 |
| Review Cycle | Annual |

## 1. Purpose
To ensure information and systems can be recovered following data loss, corruption, or a security incident.

## 2. Requirements
- Backup frequency: [Daily incremental / Weekly full] based on data criticality (see Asset Register)
- Backups are encrypted at rest and in transit
- Backups are stored following the 3-2-1 principle (3 copies, 2 media types, 1 offsite/offline)
- Restore tests are performed at least [quarterly] and logged in `08. Records`
- Backup retention: [X days/months] per legal and business requirements
- Backup access is restricted to authorized IT personnel only

## 3. Review
Reviewed annually and after any failed restore test or backup-related incident.
