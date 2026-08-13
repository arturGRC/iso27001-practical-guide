# Backup Procedure

**Supports:** Backup Policy | Control A.8.13

## 1. Scope
Applies to all systems classified as Critical or High in the Asset Register.

## 2. Procedure
1. Automated backups scheduled per system criticality (see Backup Policy frequency table)
2. Backup job success/failure monitored daily; failures escalated to IT Ops within [4 hours]
3. Backups encrypted using [AES-256] before transmission to storage
4. Quarterly restore test performed on a sample system; result documented (success/failure, time-to-restore)
5. Annual full disaster-recovery restore test performed as part of BCP testing (`11. Business Continuity`)

## 3. Records
Backup logs and restore test results retained in `08. Records` for [X years].
