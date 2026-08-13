# Context of the Organization — Hearthside Home Health

**Supports:** Clause 4.1

## External Issues
- **Regulatory:** HIPAA Security Rule and Privacy Rule (US); state-level home health licensing requirements; HHS Office for Civil Rights (OCR) breach reporting obligations (60-day notification for breaches affecting 500+ individuals)
- **Payer requirements:** Medicare/Medicaid and commercial insurers increasingly require SOC 2 or ISO 27001 attestation as a condition of network participation
- **Threat landscape:** Healthcare is a top-3 targeted sector for ransomware; home health specifically faces device-theft risk (laptops/tablets in clinician vehicles) and unsecured home Wi-Fi during patient visits
- **Medical device risk:** Remote Patient Monitoring (RPM) devices (BP cuffs, pulse oximeters, glucose meters) transmit PHI over consumer-grade Bluetooth/Wi-Fi and are frequently unpatched
- **Referral ecosystem:** Hospital systems and physician groups referring patients require evidence of security controls before data-sharing agreements are signed
- **Workforce mobility:** 180 clinicians work independently in the field with limited direct IT oversight, unlike a fixed office workforce

## Internal Issues
- Rapid patient growth (22% YoY) straining IT provisioning processes for new clinician devices
- Clinical staff turnover typical of home health (nursing shortage nationally) affecting security training consistency
- Legacy scheduling system integrated with the EHR via a decade-old API with limited vendor support
- Mixed device fleet: agency-issued laptops (managed) alongside some clinician-owned tablets used for scheduling only (BYOD, unmanaged)
- Budget constraints typical of a mid-size home health agency versus a well-funded enterprise IT function

## Implication for Scope
These issues directly drove the decision to include mobile/field data handling and the EHR platform in ISMS scope, and to treat RPM device data flows and clinician offboarding as priority risk areas (see Risk Register).
