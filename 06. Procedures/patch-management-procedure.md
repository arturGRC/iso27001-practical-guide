# Patch Management Procedure

**Supports:** Control A.8.8 (Management of Technical Vulnerabilities)

## 1. Purpose
To ensure systems are kept up to date against known vulnerabilities in a controlled manner.

## 2. Procedure
1. Vulnerability/patch feeds monitored continuously (vendor advisories, CVE feeds)
2. Patches classified by severity using CVSS score
3. Patch deployment SLAs:
   | Severity | Deployment Target |
   |---|---|
   | Critical | 72 hours |
   | High | 7 days |
   | Medium | 30 days |
   | Low | Next maintenance window |
4. Patches tested in staging before production deployment where feasible
5. Emergency patching process available to bypass standard change window for actively exploited vulnerabilities (coordinate with Change Management Procedure)
6. Patch compliance tracked and reported monthly

## 3. Records
Patch deployment records retained in `08. Records`.
