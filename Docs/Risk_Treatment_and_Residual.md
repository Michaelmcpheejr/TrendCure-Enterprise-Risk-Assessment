# Risk Treatment and Residual Risk

## Treatment Options
- Mitigate: reduce likelihood and/or impact via controls
- Accept: acknowledge risk with no additional controls
- Transfer: shift liability via contracts/insurance while maintaining oversight
- Avoid: discontinue the activity that introduces the risk

## Treatment Summary
- R-01 Identity Compromise: Mitigate
- R-02 RBAC Overprivilege: Mitigate
- R-03 Unauthorized Remote Access: Mitigate
- R-04 Endpoint Loss/Compromise: Accept
- R-05 Regulated Data Exposure: Mitigate
- R-06 Third-Party Data Breach: Transfer

## Control Selection and Ownership (High Level)
R-01 Identity Compromise (Mitigate)
- Enforce MFA for all users (Preventive) | Owner: IAM Team
- Conditional Access policies (Preventive) | Owner: Cloud Security
- Sign-in logging/monitoring (Detective) | Owner: SOC
- Phishing awareness training (Preventive) | Owner: Compliance/Awareness

R-02 RBAC Overprivilege (Mitigate)
- Periodic access reviews (Detective/Corrective) | Owner: IAM Team
- Least-privilege RBAC via groups (Preventive) | Owner: Cloud Ops
- Documented role definitions (Preventive) | Owner: Governance/Compliance

R-03 Unauthorized Remote Access (Mitigate)
- Secure configuration baselines (Preventive) | Owner: Infrastructure/Cloud Ops
- Remote access logging/alerting (Detective) | Owner: SOC
- MFA-enforced VPN authentication (Preventive) | Owner: Network Security

R-04 Endpoint Loss/Compromise (Accept)
- Full disk encryption (Preventive) | Owner: Endpoint Management
- Intune compliance enforcement (Preventive) | Owner: Endpoint Management
- Lost device reporting process (Corrective) | Owner: IT Operations

R-05 Regulated Data Exposure (Mitigate)
- DLP policies (Preventive/Detective) | Owner: Data Security
- Restricted repository access (Preventive) | Owner: Application Owners
- Audit logging (Detective) | Owner: SOC
- Data classification/handling policy (Preventive) | Owner: Governance/Compliance

R-06 Third-Party Data Breach (Transfer)
- Contractual security requirements (Preventive) | Owner: Legal/Procurement
- Vendor access monitoring (Detective) | Owner: SOC
- Periodic vendor risk assessments (Detective/Corrective) | Owner: GRC/ERM

## Residual Risk Statements
R-01 Residual Risk: Medium
Residual risk remains due to evolving phishing techniques and user behavior despite layered identity controls.

R-02 Residual Risk: Low
Access reviews and role governance reduce excessive privilege accumulation to a low residual level.

R-03 Residual Risk: Low
Secure baselines and monitoring reduce the likelihood of unauthorized remote access to a low residual level.

R-04 Residual Risk: Medium
Residual risk remains due to the operational reality of a hybrid workforce, despite encryption and endpoint management controls.

R-05 Residual Risk: Medium
DLP and logging reduce disclosure likelihood, but residual risk remains due to collaboration complexity and human error.

R-06 Residual Risk: Medium
Contracts and oversight transfer a portion of liability, but residual exposure remains due to limited control over vendor internal processes.
