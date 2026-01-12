# TrendCure Health | Enterprise Risk Assessment (Audit Readiness)

## Overview
This repository contains an enterprise risk assessment for **TrendCure Health**, a **Healthcare Technology & Services** organization (~5,000 employees) with a **cloud-first Azure and Microsoft 365 environment**. The assessment was performed to support **audit readiness** and identify prioritized risks across identity, access, endpoints, regulated data, and third parties.

## Scope
**In Scope**
- Identity & Access Management (Azure Entra ID)
- Group-based RBAC access model
- VPN and remote access services
- Intune-managed endpoints
- Patient/customer data repositories (PHI/PII)
- SaaS vendors with PHI/PII access

**Out of Scope**
- Physical security
- On-prem legacy servers
- Medical/industrial equipment

## Key Results
- **High Risk (2):**
  - Identity compromise via phishing + inconsistent MFA enforcement
  - Regulated data exposure due to lack of DLP controls
- **Medium Risk (3):**
  - RBAC excessive permissions from lack of periodic access reviews
  - Endpoint loss/compromise risk (encryption-driven)
  - Third-party vendor insider threat (monitoring-driven)
- **Low Risk (1):**
  - Unauthorized remote access (high impact, low likelihood)

## Files
- `docs/Executive_Summary.md`  
- `docs/Risk_Methodology.md`  
- `docs/Scope_and_Assets.md`  
- `docs/Risk_Treatment_and_Residual.md`  
- `registers/risk_register.csv`

## How to Use
1. Start with `docs/Executive_Summary.md`
2. Review the scoring approach in `docs/Risk_Methodology.md`
3. See scope and assets in `docs/Scope_and_Assets.md`
4. Review risk treatments and residual risk in `docs/Risk_Treatment_and_Residual.md`
5. Open `registers/risk_register.csv` for the full register

## Notes
This is a simulated enterprise assessment, structured to mirror real GRC deliverables and audit-ready documentation.
