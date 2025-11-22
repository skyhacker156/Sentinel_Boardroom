# Vendor Vetting Checklist — Sentinel_Boardroom
**Version:** 1.0  
**Department:** Compliance & Legal  
**Purpose:** Pre-engagement verification for all Phase 1, Phase 2, and Bridge Tier vendors  
**Status:** DOCUMENTATION ONLY — No execution authority  
**Last Updated:** November 22, 2025

---

## Overview
This checklist ensures that vendor engagement aligns with liability frameworks, bureau-reporting requirements, and identity consistency protocols before account activation.

**Mandatory:** Complete this checklist for every vendor. Do not proceed to payment or reporting integration until all sections are cleared.

---

## Section 1: Entity Identity Verification

| Item | Requirement | Status | Notes |
| :--- | :--- | :--- | :--- |
| **Entity Name Match** | Verify vendor account name matches Secretary of State filing exactly (including punctuation, commas, capitalization). | ☐ | Example: "Sentinel Labs, LLC" must appear identically in vendor portal. |
| **Address Standardization** | Confirm address matches IRS EIN Letter (CP-575) in USPS standardized format. Lock one format and use it consistently across all vendors. | ☐ | Choose: "Ste 100" OR "Suite 100" OR "#100" — not mixed. |
| **Phone Registration** | Verify dedicated business phone (VoIP or landline, NOT personal mobile) is registered to the entity. | ☐ | Recommended: RingCentral, Vonage, or equivalent commercial VoIP. |
| **Email Domain** | Confirm professional domain email (accounting@sentinellabs.io or equivalent), NOT Gmail/Yahoo/personal accounts. | ☐ | Bureau algorithms flag personal emails as higher fraud risk. |
| **Bureau Pre-Check** | Query D&B and Experian for any existing records under the entity name. Flag if "split files" exist. | ☐ | Contact D&B Advisor if duplicates detected before proceeding. |

---

## Section 2: Terms & Conditions — Personal Guarantee Detection

**CRITICAL:** This section prevents inadvertent personal liability.

| Red-Flag Language | Detection Rule | Action | Risk Level |
| :--- | :--- | :--- | :--- |
| **"Individually and severally liable"** | Search T&Cs for: "Individual agrees," "Personal guarantee," "Joint and several liability." | **STOP.** Flag for Legal Review before signing. Do NOT proceed. | **HIGH** |
| **"Personal credit check required"** | Vendor states: "We will pull your SSN for credit purposes." | **CLARIFY:** Ask vendor to confirm this is for Identity Verification ONLY, not a personal guarantee. Document response. | **MEDIUM** |
| **"Owner/Signatory Pledge"** | Language requiring: "Owner personally endorses," "Executive sign-off on liability," or "Guarantor designation." | **ESCALATE:** Confirm with Legal that entity-only liability is achievable. If not, document and approve as exception. | **HIGH** |
| **"Commingling Clause"** | Vendor requests: personal bank account, personal credit card, or commingling of funds. | **REJECT.** All payments must flow Entity Bank → Vendor. | **HIGH** |
| **"Indemnification (Unlimited)"** | Language: "Company indemnifies Vendor for all damages, losses, claims without limit." | **REVIEW:** Legal must assess scope. Unlimited indemnification is a liability red flag. | **MEDIUM** |

**Checklist Item:**
- ☐ T&Cs reviewed for all red-flag language listed above
- ☐ Clarifications documented (email, screenshot, or written response from vendor)
- ☐ Legal Review completed (if any HIGH flags detected)
- ☐ Exception approvals documented (if proceeding despite flags)

---

## Section 3: Vendor Tier Classification

**Purpose:** Differentiate reporting mechanisms and timeline expectations.

### Tier 1: Credit-Card-Default Vendors (Typically: Self-Service Checkout)
These vendors default to credit card or pre-pay. **Reporting is NOT automatic.**

| Vendor Type | Characteristics | Reporting Trigger | Action Required |
| :--- | :--- | :--- | :--- |
| **Adobe, Slack, Zoom** | Self-service SaaS; monthly subscription. | Enterprise Sales agreement with Net-30 invoice terms. | Contact Business/Enterprise Sales. Minimum: 5–10 seats or annual contract paid monthly. |
| **Smaller SaaS** | Sub-$100/month tools. | Often no commercial invoicing available. | **Skip for credit-building.** Use personal card or prepay only. |

**Checklist Item:**
- ☐ Identified all Tier 1 vendors in Phase 1
- ☐ Confirmed Enterprise Sales contact (not self-service checkout)
- ☐ Verified minimum seat/contract requirements before applying
- ☐ Documented Enterprise Sales email or phone contact

### Tier 2: Invoice-Native Vendors (Typically: B2B Industrial/Office Supply)
These vendors issue commercial invoices automatically. **Reporting is automatic if payment terms are Net-X.**

| Vendor Type | Characteristics | Reporting Trigger | Action Required |
| :--- | :--- | :--- | :--- |
| **Uline, Grainger, W.B. Mason** | B2B industrial/office supply; invoice-based purchasing. | Automatic upon invoice generation. | Standard application; no special negotiation needed. |
| **AWS, GCP (Business Accounts)** | Cloud services; business invoicing available. | "Pay by Invoice" option triggered after credit check. | Must have Layer 0 posting before AWS application (credit check dependency). |

**Checklist Item:**
- ☐ Identified all Tier 2 vendors in Phase 1
- ☐ Confirmed invoice-native reporting is automatic
- ☐ Documented any credit-check prerequisites (e.g., Layer 0 sequencing for AWS)

### Tier 3: Bridge Tier (High-Frequency / Financial)
These vendors report more frequently (weekly/bi-weekly) or carry higher weight in bureau algorithms.

| Vendor Type | Characteristics | Reporting Frequency | Action Required |
| :--- | :--- | :--- | :--- |
| **WEX Fleet / AtoB** | Commercial fuel/vehicle expense card. | Weekly or bi-weekly usage reporting. | Application may require bank account or existing trade line. Sequence after Layer 0. |
| **Nav Prime** | Subscription credit-builder (financial service). | Reports as "Financial Service" — higher bureau weight. | Straightforward application; can be activated in parallel with Phase 1. |

**Checklist Item:**
- ☐ Identified Bridge Tier vendors approved for integration
- ☐ Confirmed reporting frequency and bureau classification
- ☐ Documented sequencing dependencies (e.g., Layer 0 before WEX)

---

## Section 4: Bureau-Alignment Syntax Verification

**Purpose:** Prevent "split files" caused by data inconsistency.

Before submitting any vendor application, complete this step:

1. **Pull Master Entity Profile from D&B:**
   - Go to D&B Business Portal (or contact D&B Advisor).
   - Search for "Sentinel Labs" under your EIN.
   - **Document:** Exact name, address, phone, and email as D&B has it on file.

2. **Compare Vendor Application to D&B Profile:**
   - Entity Name: Does it match exactly?
   - Address: Does it match the standardized format?
   - Phone: Does it match the registered business phone?
   - Email: Does it match the professional domain email?

3. **Resolution Protocol:**
   - **Perfect Match:** Proceed with application.
   - **Minor Variance (e.g., "Sentinel Labs LLC" vs. "Sentinel Labs, LLC"):** Contact D&B to file a **consolidation request** before submitting the vendor application. This prevents split file creation.
   - **Major Discrepancy:** Escalate to Legal and D&B Advisor. Do not proceed until resolved.

**Checklist Item:**
- ☐ D&B profile pulled and documented
- ☐ Vendor application data compared to D&B profile
- ☐ Any variance flagged and consolidated before application submission
- ☐ Consolidation request filed (if needed)

---

## Section 5: Pre-Activation Sign-Off

**All sections must be complete before vendor account activation.**

| Sign-Off Item | Responsibility | Status |
| :--- | :--- | :--- |
| **Identity Verification** (Section 1) | Compliance Officer | ☐ |
| **T&C Red-Flag Review** (Section 2) | Legal Advisor | ☐ |
| **Tier Classification** (Section 3) | Finance Officer | ☐ |
| **Bureau-Alignment Verification** (Section 4) | Compliance Officer (+ D&B Advisor if variance detected) | ☐ |
| **Founder Authorization** | Founder | ☐ |

**Gate:** Do not proceed to account activation until all sign-offs are complete.

---

## Appendix: Template — Vendor Application Log

Use this template to track each vendor application.
