# Master SOP — Audit Layer Integration into Phase 1 Vendor Onboarding
**Version:** 1.0  
**Department:** Compliance  
**Purpose:** Step-by-step operationalization of the Audit Layer controls; integration with Phase 1 vendor onboarding  
**Status:** DOCUMENTATION ONLY — No execution authority  
**Last Updated:** November 22, 2025

---

## Executive Summary

This SOP operationalizes the three primary risks identified in the **Audit Layer: Integrated Corrections & Appendices**:

1. **SaaS Procurement Risk:** Self-service checkout does NOT trigger commercial invoicing.
2. **Payment Timing Risk:** Early payment before invoice booking causes "ghost balance" non-reporting.
3. **Identity Consistency Risk:** Bureau algorithms flag syntax variances, creating split files.

This SOP integrates these controls into a step-by-step workflow that Founder and Operations Lead must follow before activating any vendor relationship.

---

## Governance & Roles

| Role | Responsibility | Authority |
| :--- | :--- | :--- |
| **Founder** | Final authorization for all vendor activations; ultimate liability | Approval/Rejection |
| **Operations Lead** | Day-to-day vendor onboarding execution; checklist completion | Execution |
| **Compliance Officer** | Vendor vetting checklist review; identity verification; T&C red-flag flagging | Gating Authority |
| **Legal Advisor** | Personal guarantee detection; liability assessment; terms & conditions escalation | Gating Authority |
| **Finance Officer** | Timing & sequencing validation; payment window verification; D&B reconciliation | Gating Authority |
| **D&B Advisor** (External) | Bureau profile management; consolidation requests; variance resolution | Advisory |

---

## Pre-Onboarding Phase (Before Any Vendor Application)

### Step 1: Establish Master Entity Syntax (Day 0)

**Objective:** Define the single, authoritative version of entity information to be used across all vendors and D&B profile.

**Actions:**
1. Pull your **Secretary of State filing** (your state's SOS website).
   - **Document:** Entity name as it appears on the filing (including punctuation, commas, capitalization).
2. Pull your **IRS EIN Letter (CP-575)** from IRS.gov or your tax advisor.
   - **Document:** Address as listed on the EIN letter. Standardize into USPS format (choose one: "Ste 100" OR "Suite 100" OR "#100" — lock this choice).
3. Establish a **dedicated business phone** (VoIP or landline; NOT personal mobile).
   - **Recommend:** RingCentral, Vonage, or equivalent.
   - **Document:** Phone number and service provider.
4. Establish a **professional domain email** (NOT Gmail/Yahoo).
   - **Document:** Email address (e.g., accounting@sentinellabs.io).
5. Create a **Master Entity Syntax Document** (internal reference).

**Master Entity Syntax Template:**
```
ENTITY NAME: [Exact text from Secretary of State]
ADDRESS: [Standardized USPS format from EIN Letter]
PHONE: [Dedicated business VoIP/landline]
EMAIL: [Professional domain]
EIN: [Your EIN]
SECRETARY OF STATE FILING: [Link or reference]
NOTES: [Any other identifiers]
```

**Gate:** All subsequent vendor applications must use this syntax **with zero variance.**

**Founder Sign-Off:** ☐ Master Entity Syntax approved and locked

---

### Step 2: Establish D&B Profile & Baseline Query (Day 1–3)

**Objective:** Query D&B to confirm they have your entity profile and identify any pre-existing "split files" that must be consolidated.

**Actions:**
1. Contact **D&B Advisor** or access **D&B Business Portal** directly.
2. Search for your entity by name and EIN.
3. Document the result:
   - **Scenario A:** "Single, consolidated profile found." — Proceed to Step 3.
   - **Scenario B:** "Multiple profiles found (split files)." — File consolidation request NOW before proceeding further.
   - **Scenario C:** "No profile found." — This is normal for new entities. D&B will create a profile upon first vendor reporting.

4. If Scenario B: Contact D&B Advisor to consolidate records. This typically takes 5–10 business days. **Do not proceed with vendor applications until consolidation is complete.**

**D&B Query Log:**
```
Query Date: [YYYY-MM-DD]
D&B Status: [Single Profile / Split Files / No Profile]
D&B DUNS #: [if assigned]
Consolidation Requested: [Y/N]
Consolidation Date (if applicable): [YYYY-MM-DD]
Status: [Pending / Complete]
```

**Gate:** Either Scenario A or confirmed Scenario B consolidation required before proceeding.

**Compliance Officer Sign-Off:** ☐ D&B profile verified; no split files or consolidation in progress

---

## Vendor Onboarding Phase (Per-Vendor Workflow)

### Step 3: Vendor-Specific Vetting (Per Vendor)

**Objective:** Evaluate each vendor against the Compliance checklist before application.

**Actions:**
1. Identify vendor and tier classification (Tier 1 / Tier 2 / Tier 3).
2. Complete **Vendor Vetting Checklist** (from `/compliance/Vendor_Vetting_Checklist_v1.0.md`):
   - Section 1: Entity Identity Verification
   - Section 2: T&C Red-Flag Detection
   - Section 3: Tier Classification
   - Section 4: Bureau-Alignment Syntax Verification
3. Document findings in **Vendor Application Log** (template in checklist).
4. Escalate any HIGH flags to Legal Advisor for review.
5. Obtain required sign-offs:
   - **Compliance Officer:** Identity verification + D&B variance check
   - **Legal Advisor:** T&C review (if any flags)
   - **Finance Officer:** Tier classification + sequencing prerequisites

**Gate:** Do not proceed to Step 4 until all sign-offs obtained.

**Required Documentation:**
- ☐ Completed Vendor Vetting Checklist
- ☐ Vendor Application Log entry
- ☐ Legal sign-off (if T&C review required)
- ☐ Finance sequencing verification (prerequisites met)

---

### Step 4: Application Submission

**Objective:** Submit vendor application using Master Entity Syntax (zero variance).

**Actions:**
1. Open vendor application portal (vendor website, Enterprise Sales contact, etc.).
2. Fill out application form using **Master Entity Syntax** (copy-paste from Master Entity Syntax Document to ensure exact match).
   - Entity Name: [from Master Entity Syntax]
   - Address: [from Master Entity Syntax]
   - Phone: [from Master Entity Syntax]
   - Email: [from Master Entity Syntax]
3. For Tier 1 vendors (SaaS): Contact Enterprise Sales directly if self-service checkout does NOT offer Net-X invoicing.
4. For Tier 2 vendors (B2B): Proceed through standard application process.
5. For Tier 3 vendors (Bridge): Proceed through standard application process.
6. **Document:** Application submission date, contact name (if applicable), confirmation number.

**Application Submission Log:**
```
Vendor: [Name]
Tier: [1 / 2 / 3]
Application Date: [YYYY-MM-DD]
Submission Method: [Self-Service / Enterprise Sales Contact / etc.]
Contact Name (if applicable): [Name, email, phone]
Confirmation Number: [if provided]
Entity Name Submitted: [confirm matches Master Entity Syntax exactly]
```

**Gate:** Confirmation of application submission. Proceed to Step 5 upon approval/account activation.

---

### Step 5: Account Activation & First Order (Per Vendor Timeline)

**Objective:** Upon approval, activate account and place first order with legitimate business purpose.

**Actions:**
1. Upon vendor approval email, log into vendor portal and activate account.
2. Confirm that account profile shows **Master Entity Syntax exactly** (check against Master Entity Syntax Document).
3. Place **first order:**
   - **Tier 0 (Uline/Grainger):** Minimum $250–$500 of legitimate business supplies (office equipment, networking gear, etc.).
   - **Tier 1A (Adobe/Slack/Zoom):** Minimum seats/subscription as negotiated with Enterprise Sales.
   - **Tier 1B (AWS):** Minimum infrastructure spend (~$100–$500/month) or reserved capacity to generate invoice.
   - **Tier 2 (WEX/AtoB):** Activate card upon issuance; link to business bank account; use for legitimate vehicle/fuel expenses.
   - **Tier 3 (Nav Prime):** Activate subscription; set automatic monthly payment.
4. **Document:** Order date, order ID, expected invoice date (if applicable).

**Vendor Account Activation Log:**
```
Vendor: [Name]
Approval Date: [YYYY-MM-DD]
Account Portal Name (as shown): [confirm matches Master Entity Syntax]
First Order Date: [YYYY-MM-DD]
Order ID: [if provided]
Expected Invoice/Statement Date: [YYYY-MM-DD]
Amount: [if applicable]
Notes: [legitimate business purpose for order]
```

**Gate:** Account activated and first order placed. Proceed to Step 6.

---

### Step 6: Invoice Generation & Payment Timing (Ghost Balance Prevention)

**Objective:** Execute payment following the 48-hour/5-day protocol to prevent non-reporting.

**Actions:**
1. **Wait for invoice generation** (do not pay immediately upon order placement).
   - Monitor vendor portal or email for "Invoice Generated," "Statement Available," or "Payment Due" notification.
   - Expected window: 3–10 business days after order placement (varies by vendor).
2. **Verify invoice details:**
   - Confirm invoice ID exists in vendor portal.
   - Confirm line items match order (usage → invoiced).
   - Confirm due date (typically Net-30, Net-15, etc.).
3. **Payment execution window:**
   - **Earliest payment:** 48 hours after invoice generation (when invoice is "booked" in vendor system).
   - **Latest payment:** At least 5 days before due date.
   - **Execution method:** ACH transfer from business bank account (NOT personal credit card, NOT personal bank account).
4. **Document:** Invoice date, invoice ID, amount, payment execution date, payment confirmation number.

**Payment Execution Log (Ghost Balance Prevention):**
```
Vendor: [Name]
Invoice Generation Date: [YYYY-MM-DD]
Invoice ID: [if available]
Invoice Amount: [amount]
Due Date: [YYYY-MM-DD]
Payment Execution Date: [YYYY-MM-DD] (must be 48h post-invoice, 5d pre-due)
Payment Method: [ACH from business bank account]
Payment Confirmation Number: [from bank]
Status: [Executed]
D&B Posting Expected: [YYYY-MM-DD] (typically 10–15 days post-payment)
```

**Gate:** Payment executed within the 48-hour/5-day window. Proceed to Step 7.

---

### Step 7: Bureau Posting Verification (D&B Reconciliation)

**Objective:** Verify vendor has posted to D&B and confirm reporting is accurate.

**Actions:**
1. **Timeline:** 10–15 days after payment execution, query D&B to verify vendor has reported.
2. **Query D&B:**
   - Log into D&B Business Portal or contact D&B Advisor.
   - Search for your entity.
   - Review "Active Trade Lines" section.
3. **Verification:**
   - ☐ Vendor name appears in Active Trade Lines.
   - ☐ Reporting shows "Usage → Invoiced → Paid Early" (or "Paid On-Time" if on schedule).
   - ☐ No duplicate entries or split files created.
   - ☐ Account name matches Master Entity Syntax exactly.
4. **If vendor NOT reporting:**
   - Contact vendor immediately to verify invoice was sent to bureau.
   - Ask vendor to confirm bureau reporting is activated (some vendors require explicit activation).
   - If vendor confirms reporting is active, wait an additional 5 business days and re-query D&B.
5. **If split file created:**
   - Contact D&B Advisor immediately to file consolidation request.
   - Do not proceed with additional vendor onboarding until split is resolved.

**Bureau Posting Verification Log:**
```
Vendor: [Name]
Query Date: [YYYY-MM-DD]
D&B Status: [Reporting / Pending / Not Found / Split File]
Account Name (as shown on D&B): [exact text]
Active Trade Line Status: [Yes / No / Duplicate]
Variance from Master Entity Syntax: [None / List discrepancies]
Action Required: [None / Contact Vendor / D&B Consolidation / Escalate]
Date Resolved: [YYYY-MM-DD] (if applicable)
```

**Gate:** Vendor reporting verified and no split files created. Vendor onboarding COMPLETE.

---

## Post-Onboarding Phase (Ongoing Monitoring)

### Step 8: Recurring D&B Monitoring (Monthly)

**Objective:** Ensure all active vendors continue reporting correctly and no new split files emerge.

**Actions:**
1. **Monthly D&B Query (recommended timing: mid-month):**
   - Log into D&B Business Portal.
   - Review all active trade lines.
   - Verify each vendor is showing current reporting (no late/overdue status).
2. **Reconciliation:**
   - Cross-reference active vendors against your Master Vendor List.
   - Identify any new entries or duplicates.
   - Flag any vendors with "Reported Late" or overdue status.
3. **Follow-up Actions:**
   - If vendor is reporting late, contact vendor to confirm payment was processed correctly.
   - If split file emerges, contact D&B Advisor immediately.
   - If new entry appears without your application, investigate for fraud/duplicate registration.

**Monthly D&B Monitoring Log:**
```
Query Date: [YYYY-MM-DD]
Active Trade Lines: [# of vendors]
Late/Overdue Status: [Yes / No]
New Entries Since Last Query: [None / List]
Split Files Detected: [None / List]
Action Items: [None / List actions + responsible party + due date]
```

**Frequency:** Monthly (or quarterly, depending on vendor velocity).

---

## Escalation & Exception Handling

### Scenario A: Vendor Denies Application

**Likely Cause:** Insufficient credit history or failed credit check.

**Actions:**
1. Request denial reason from vendor.
2. If credit-check-related: Ensure Layer 0 vendors (Uline/Grainger) have posted to D&B before re-applying. This typically improves approval odds for Tier 1 vendors.
3. Document denial in Vendor Application Log and escalate to Finance Officer.
4. Consider alternative vendor in same tier.

---

### Scenario B: Vendor Defaults to Self-Service Credit Card Checkout (No Invoice Option)

**Likely Cause:** Vendor size or product offering does not support commercial invoicing.

**Actions:**
1. Contact vendor's Business/Enterprise Sales team (if available) to inquire about Net-X invoicing options.
2. If unavailable: **This vendor is not suitable for credit-building.** Remove from Phase 1.
3. Select alternative vendor that supports commercial invoicing.

---

### Scenario C: Payment Executes But Vendor Does NOT Report to D&B (After 15+ Days)

**Likely Cause:** Vendor did not activate bureau reporting, or reporting was sent to wrong bureau.

**Actions:**
1. Contact vendor and ask: "Can you confirm you are actively reporting this account to D&B?"
2. If vendor confirms reporting is NOT active: Ask vendor to activate bureau reporting explicitly.
3. If vendor confirms reporting IS active but D&B shows nothing: Ask vendor which bureau(s) they report to. Request they report to D&B specifically.
4. If vendor is unable or unwilling to report: **Remove vendor from active relationship** and identify replacement.

---

### Scenario D: T&C Red Flag Detected (E.g., "Personal Guarantee")

**Actions:**
1. **STOP vendor application immediately.**
2. Escalate to Legal Advisor with full T&C excerpts.
3. Legal Advisor provides one of three recommendations:
   - **Proceed:** Personal guarantee language is acceptable or can be negotiated out.
   - **Escalate to Founder:** Higher-risk approval required; Founder must authorize exception.
   - **Reject:** Do not proceed with this vendor.
4. Document Legal decision in Vendor Vetting Checklist and Vendor Application Log.

---

### Scenario E: Split File Detected in D&B (Before or After Vendor Onboarding)

**Critical Escalation.**

**Actions:**
1. Contact D&B Advisor immediately.
2. File consolidation request to merge duplicate profiles.
3. **Pause all new vendor onboarding** until consolidation is complete (typically 5–10 business days).
4. Once consolidated, re-query D&B to verify single profile exists.
5. Document consolidation timeline in D&B Query Log.

---

## Drift Prevention Checklist

**Before each vendor activation, verify this checklist to prevent operational drift:**

| Item | Verification | Status |
| :--- | :--- | :--- |
| **Master Entity Syntax Locked** | Confirm Master Entity Syntax Document exists and is current. | ☐ |
| **D&B Profile Current** | Most recent D&B query shows single, consolidated profile. | ☐ |
| **Vendor Vetting Checklist Complete** | All sections signed off (Identity, T&C, Tier, Bureau Alignment). | ☐ |
| **Sequencing Prerequisites Met** | For Tier 1+, confirm Layer 0 vendors are posting. For Tier 2+, confirm 2–3 Layer 1 vendors active. | ☐ |
| **Application Syntax Verified** | Confirm application submitted using Master Entity Syntax with zero variance. | ☐ |
| **Payment Timing Protocol Understood** | Confirm Operations Lead understands 48-hour/5-day window (no early payment). | ☐ |
| **D&B Monitoring Planned** | Confirm monthly D&B query is scheduled and assigned to responsible party. | ☐ |
| **Founder Authorization Obtained** | Confirm Founder has approved vendor activation. | ☐ |

---

## Approval Workflow Summary
```
┌─────────────────────────────────┐
│   Founder: Identify Vendor      │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Compliance: Vetting Checklist  │
│   + D&B Variance Check          │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Legal: T&C Review             │
│   (if red flags detected)       │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Finance: Sequencing Validation│
│   (prerequisites met?)          │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Founder: Final Approval       │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Operations: Application        │
│   Submission + Order Placement   │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Finance: Payment Execution    │
│   (48-hour/5-day protocol)      │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Compliance: D&B Verification  │
│   + Posting Confirmation        │
└─────────────────────────────────┘
                ↓
┌─────────────────────────────────┐
│   Vendor Onboarding: COMPLETE   │
└─────────────────────────────────┘
```

---

## Documentation Repository

**All documents required by this SOP must be stored in the following structure:**
```
/sentinel_boardroom
  /finance
    - Credit_Sequencing_Diagram_v1.0.md
    - Vendor_Sequencing_Prerequisites.md
    - Payment_Timing_Protocol.md
  /compliance
    - Vendor_Vetting_Checklist_v1.0.md
    - Audit_Integration_SOP_v1.0.md
    - Master_Entity_Syntax_Document.md
    - D&B_Query_Log.md
    - Vendor_Application_Log_Template.md
    - Monthly_D&B_Monitoring_Log.md
  /legal
    - T&C_Red_Flag_Language_Examples.md
    - Personal_Guarantee_Detection_Guide.md
```

---

## Document Maintenance & Review

**Next Review:** Upon onboarding 3rd vendor (Phase 1 completion expected Day 45–60)  
**Maintained By:** Compliance Department  
**Version Control:** Update version number upon any material change to protocol  
**Distribution:** All team members with vendor onboarding responsibilities

---

**SOP Status:** APPROVED FOR IMMEDIATE IMPLEMENTATION  
**Effective Date:** November 22, 2025  
**Founder Authorization:** [Signature / Approval date to follow]
