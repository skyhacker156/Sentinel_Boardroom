## Sentinel_Boardroom | Internal Audit & Compliance

**Document:** Audit Layer: Integrated Corrections & Appendices  
**Version:** 1.0 (Overlay)  
**Reference Target:** Phase 1 Vendor Shopping Cart Package (v1.0)  
**Date:** November 22, 2025  
**Status:** **APPROVED WITH MANDATORY CONTROLS**

### Executive Summary
This audit layer validates the strategic logic of the "Phase 1 Vendor Shopping Cart Package." The core vendor selection is sound. However, operational constraints regarding **SaaS procurement workflows**, **reporting trigger timing**, and **data entry syntax** present high risks of execution failure (false positives/non-reporting) if not addressed.

This document serves as the **Control Framework** to be ingested alongside the Phase 1 Package.

---

### Appendix A: SaaS Procurement Barriers (Operational Constraint)

**Context:** The Phase 1 Package identifies Adobe, Zoom, and Slack as "Layer 1" reporters.
**Audit Finding:** Standard web-checkout flows for these vendors default to Credit Card (revolving) or Pre-Pay, which **do not** create the commercial invoice necessary for bureau reporting.
**Control Protocol:**

1.  **The "Enterprise" Gate:**
    * **Adobe/Slack/Zoom:** You cannot achieve Net-30 reporting via self-service checkout.
    * **Requirement:** The Founder or Operations Lead must contact **Enterprise Sales** or **Business Sales**.
    * **Threshold:** Be prepared for a minimum seat count (often 5-10 users) or an **Annual Contract** paid monthly to trigger invoicing.
2.  **The AWS Exception:**
    * AWS allows "Pay by Invoice" more easily but requires a credit check. Ensure "Layer 0" (Uline/Grainger) has posted *before* applying for AWS invoicing to avoid denial or a deposit requirement.

---

### Appendix B: Payment Timing Protocol ("Ghost Balance" Mitigation)

**Context:** Phase 1 recommends paying "10–15 days early."
**Risk Vector:** "Ghost Balancing." If a payment is pushed before the reporting cycle closes, the vendor system reports `$0 Balance / $0 Usage`. No payment history is generated.
**Control Protocol:**



1.  **The "Statement Available" Trigger:**
    * **Do Not** pay immediately upon placing the order.
    * **Do Not** pay immediately upon shipping notification.
    * **Action:** Wait for the official **Invoice Generation** or **Statement Notification** email.
2.  **The Reporting Window:**
    * Once the invoice exists in the portal with a distinct Invoice ID, the debt is "booked."
    * **Payment Execution:** Execute ACH transfer 48 hours *after* Invoice Generation but at least 5 days *before* Due Date.
    * **Result:** The system captures "Usage" -> "Invoiced" -> "Paid Early."

---

### Appendix C: Identity Consistency (The "4-Way Match")

**Context:** Bureau algorithms (D&B, Experian) are highly sensitive to syntax variations.
**Risk Vector:** "Split Files." A mismatch between the Secretary of State filing and a vendor account creates two separate credit profiles, diluting the score.
**Control Protocol:**

The **Master Entity Syntax** must be defined and adhered to with **Zero-Variance**.

| Data Field | Source of Truth | Variance Rule | Example |
| :--- | :--- | :--- | :--- |
| **Entity Name** | Secretary of State Filing | **Strict Match.** If the filing has a comma, the vendor account *must* have a comma. | "Sentinel Labs, LLC" ≠ "Sentinel Labs LLC" |
| **Address** | IRS EIN Letter (CP-575) | **Standardized.** Choose one USPS format and lock it. | "Ste 100" vs "Suite 100" vs "#100" |
| **Phone** | 411/directory Listing | **Dedicated.** Do not use a personal mobile. Must be a VoIP/Landline registered to the Entity. | Commercial VoIP (RingCentral, etc.) |
| **Email** | Domain Registry | **Professional.** Never use Gmail/Yahoo. | accounting@sentinellabs.io |

---

### Appendix D: Supplemental Layer – Fuel & Financial Bridge

**Context:** Phase 1 focuses on Office/Industrial supplies. To accelerate "payment frequency" data points, high-transaction vendors are required.
**Addendum:** The following "Bridge Tier" vendors are approved for immediate integration.

* **WEX Fleet / AtoB:**
    * **Function:** Commercial fuel cards (can often be used for general vehicle expenses).
    * **Mechanism:** Often linked to the bank account (daily/weekly reporting).
    * **Benefit:** High-frequency reporting cycles. Unlike Uline (monthly), these often report weekly or bi-weekly usage, accelerating the "active trade line" count.
* **Nav Prime:**
    * **Function:** Financial trade line.
    * **Mechanism:** Subscription-based credit builder.
    * **Benefit:** Reports as a "Financial Service" rather than "Vendor," which carries higher weight in the D&B algorithm.

---

### Appendix E: Cross-Departmental Advisory Footnotes

**Documentation-Level Guidelines only.**

#### 1. Tax Alignment (CPA Perspective)
* **IRC § 162 Compliance:** Purchases made to build credit must still pass the "Ordinary and Necessary" test for business expenses.
* **Audit Risk:** Purchasing $500 of cleaning supplies for a digital consulting firm to "build credit" is a red flag.
* **Directive:** Align "Layer 0" purchases with actual operational needs (e.g., toner, hard drives, legitimate software) to ensure deductibility.

#### 2. Legal & Liability (Corporate Veil)
* **Commingling Prohibition:** Under no circumstances should personal funds be used to pay these vendor invoices directly.
* **Process:** Capital -> Business Bank Account -> Vendor.
* **Personal Guarantees (PG):** While Phase 1 targets "No-PG" vendors, some applications may ask for a social security number for "Identity Verification" vs. "Guarantee."
* **Control:** Read the Terms & Conditions. If language states *"Individual agrees to be jointly and severally liable,"* this creates personal liability. Flag for Legal Review.

---

**Audit Status:**
The **Phase 1 Package**, when paired with this **Audit Layer**, is cleared for implementation.

**Next Action:**
Awaiting **Compliance Signal** to merge these protocols into the Master Standard Operating Procedure (SOP).
