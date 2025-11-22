# Credit Sequencing Diagram — Sentinel_Boardroom
**Version:** 1.0  
**Department:** Finance  
**Purpose:** Timeline and dependency map for Phase 1, Phase 2, and Bridge Tier vendor activation  
**Status:** DOCUMENTATION ONLY — No execution authority  
**Last Updated:** November 22, 2025

---

## Overview
This diagram maps the sequential activation of vendor relationships to optimize reporting cycles and prevent execution failures (e.g., "ghost balancing," credit check denials, or invoice timing misses).

**Key Principle:** Certain vendors have prerequisites. Attempting to activate them out of sequence results in denials or non-reporting.

---

## Layer 0: Foundation Layer (Days 1–14)

**Purpose:** Establish initial trade-line presence and satisfy credit-check prerequisites for higher-tier vendors.

| Vendor | Account Type | Minimum Purchase | Expected Posting Window | Reporting Mechanism | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Uline** | B2B Industrial Supply (Net-30) | $250–$500 (legitimate business supplies) | 3–5 business days after order | Automatic invoice reporting | First vendor; establishes baseline credit profile. |
| **Grainger** | B2B Industrial Supply (Net-30) | $250–$500 (legitimate business supplies) | 3–5 business days after order | Automatic invoice reporting | Second vendor; increases trade-line count. |

**Execution Protocol:**
1. Complete vendor vetting checklist (Compliance sign-off required).
2. Place order with legitimate business supplies (e.g., office equipment, networking gear, cleaning supplies).
3. **Do NOT pay early.** Wait for invoice generation and statement notification.
4. Payment execution: **48 hours after invoice generation, but at least 5 days before due date.**
5. Expected bureau reporting: **10–15 days after payment posted.**

**Layer 0 Gate:** Do not proceed to Layer 1 until both Uline and Grainger have posted to D&B (typically 14–21 days from first order).

**Verification Checklist:**
- ☐ Uline account active and first invoice posted
- ☐ Grainger account active and first invoice posted
- ☐ D&B query shows both vendors listed in "Active Trade Lines"
- ☐ No "ghost balance" issues (verify usage and payment posting separately)

---

## Layer 1A: SaaS Tier — Enterprise Gate (Days 15–35)

**Purpose:** Activate high-frequency, recognizable SaaS vendors through enterprise channels to trigger Net-X invoicing.

### Pre-Requisite Gate
**Layer 0 must post to D&B before Layer 1A applications.** This improves approval odds for enterprise SaaS applications and may eliminate deposit requirements.

| Vendor | Enterprise Channel | Minimum Commitment | Invoice Frequency | Expected Posting Window | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Adobe** | Adobe Business Sales | 5–10 seats OR annual contract paid monthly | Monthly | 10–15 days after payment posted | Contact Business Sales, not self-service. Inquire about Net-30 terms. |
| **Slack** | Slack Business Sales | 3+ users (varies) OR annual contract | Monthly | 10–15 days after payment posted | Similar to Adobe; requires enterprise contact. |
| **Zoom** | Zoom Business Sales | 5+ users OR annual contract | Monthly | 10–15 days after payment posted | Often easiest to negotiate; start here if budget-constrained. |

**Execution Protocol:**
1. Contact Business/Enterprise Sales for each vendor (DO NOT use self-service checkout).
2. Inquire explicitly: **"Do you offer Net-30 or Net-15 invoicing terms with monthly reporting?"**
3. If yes, proceed with application. If no, skip vendor and move to alternatives.
4. Upon account approval, place initial order (minimum commitment as negotiated).
5. **Ghost Balance Prevention:** Wait for first invoice generation. Do not pay immediately upon order placement.
6. Payment execution: **48 hours after invoice generation, but at least 5 days before due date.**
7. Expected bureau reporting: **10–15 days after payment posted.**

**Layer 1A Gate:** Do not proceed to Layer 1B until at least two Layer 1A vendors have posted to D&B.

**Vendor Application Log Template:**
```
**Vendor:** [Adobe/Slack/Zoom]
**Enterprise Sales Contact:** [Name, email, phone]
**Application Date:** [YYYY-MM-DD]
**Net-X Terms Confirmed:** [Yes / No / Negotiated to ___]
**Account Activation Date:** [YYYY-MM-DD]
**First Invoice Date:** [YYYY-MM-DD]
**Payment Execution Date:** [YYYY-MM-DD]
**D&B Posting Date:** [YYYY-MM-DD] (verify via D&B query)
**Status:** [Pending / Active / Reporting]
```

**Verification Checklist:**
- ☐ At least 2 Layer 1A vendors showing in active trade lines on D&B
- ☐ No duplicate entries or "split files" detected
- ☐ Monthly invoices being generated and posted on-time

---

## Layer 1B: AWS / Cloud Services (Days 25–45)

**Purpose:** Establish cloud infrastructure vendor relationship with high bureau weight.

### Pre-Requisite Gates
1. **Layer 0 posting required.** AWS credit check pulls D&B profile; prior trade-line presence improves approval odds.
2. **Consider sequencing:** Apply for AWS after Layer 0 posts but in parallel with Layer 1A applications to optimize timeline.

| Vendor | Account Type | Minimum Spend | Invoice Frequency | Reporting Mechanism | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **AWS** | Business Account (Pay by Invoice) | $100–$500/month typical | Monthly | Automatic invoice reporting (upon "Pay by Invoice" activation) | Requires credit check. Layer 0 posting improves odds. |

**Execution Protocol:**
1. Open AWS account using corporate entity details (match Master Entity Syntax exactly).
2. Use corporate email for primary contact.
3. Upon account creation, AWS will likely default to "Pay by Credit Card." **Request to switch to "Pay by Invoice" immediately.**
4. AWS will trigger a credit check at this point. **Expected outcome:** Approved (if Layer 0 is posting) or request for a deposit (if insufficient credit history).
5. Once "Pay by Invoice" is activated, place initial infrastructure order (or reserve capacity to generate a minimal invoice).
6. **Ghost Balance Prevention:** Wait for first invoice generation and statement notification.
7. Payment execution: **48 hours after invoice generation, but at least 5 days before due date.**
8. Expected bureau reporting: **10–15 days after payment posted.**

**Layer 1B Gate:** AWS should post within 30–45 days of account opening.

**Verification Checklist:**
- ☐ AWS account active with "Pay by Invoice" enabled
- ☐ First invoice generated and payment executed
- ☐ D&B query shows AWS listed in active trade lines

---

## Layer 2: Bridge Tier — High-Frequency & Financial (Days 35–60)

**Purpose:** Accelerate payment-frequency data points and increase bureau algorithm weight through specialized vendors.

### Pre-Requisite Gates
1. **Layer 0 must post to D&B.**
2. **At least 2–3 Layer 1 vendors must be active.** This demonstrates established payment behavior before applying for higher-risk products.

### Bridge Tier A: Fuel & Vehicle Expense (WEX Fleet / AtoB)

| Vendor | Account Type | Minimum Activation | Reporting Frequency | Reporting Mechanism | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **WEX Fleet** | Commercial fuel card | Linked to business bank account | Weekly or bi-weekly | Automatic usage & payment reporting | High-frequency reporting accelerates "active trade line" count. |
| **AtoB** | Commercial fuel card (alternative) | Linked to business bank account | Weekly or bi-weekly | Automatic usage & payment reporting | Similar to WEX; offers alternative if WEX denies. |

**Execution Protocol:**
1. Ensure business bank account is established and visible on D&B profile.
2. Apply for fuel card using entity details. Expect credit check (Layer 0 posting improves odds).
3. Upon approval, activate card and link to business bank account.
4. Use card for legitimate business vehicle/fuel expenses.
5. **Automatic Reporting:** Weekly/bi-weekly usage and payments are reported automatically to bureaus.
6. No manual payment timing required; reporting is tied to card usage.

**Verification Checklist:**
- ☐ Fuel card account active and linked to business bank account
- ☐ First transaction posted
- ☐ D&B query shows weekly/bi-weekly reporting activity

### Bridge Tier B: Financial Trade Line (Nav Prime)

| Vendor | Account Type | Subscription Cost | Reporting Frequency | Reporting Classification | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Nav Prime** | Credit-builder subscription | ~$15–$30/month | Monthly | Reports as "Financial Service" — higher bureau weight | Can be activated in parallel with other vendors. |

**Execution Protocol:**
1. Navigate to Nav Prime (navprime.com or equivalent).
2. Open account using entity details. Straightforward application (minimal underwriting).
3. Activate subscription and set automatic monthly payment from business bank account.
4. Expected reporting: **Monthly to Experian, TransUnion, and Equifax as a "Financial Service."**
5. This trade line carries higher weight in D&B algorithm than vendor accounts.

**Execution Notes:**
- Nav Prime is independent of other Layer 1/Layer 2 sequencing; can be activated immediately.
- Monthly subscription cost is tax-deductible (IRC § 162 — ordinary and necessary business expense).

**Verification Checklist:**
- ☐ Nav Prime account active
- ☐ First subscription payment posted
- ☐ D&B query shows "Financial Service" classification

---

## Timeline Summary — Full Sequence
```
Days 1–14:   Layer 0 posting (Uline, Grainger)
Days 15–35:  Layer 1A (Adobe/Slack/Zoom) + Layer 1B (AWS) applications and first invoices
Days 25–45:  Layer 1B (AWS) credit check, activation, and first invoice
Days 35–60:  Layer 2 (WEX/AtoB, Nav Prime) applications and first transactions
Days 60–90:  Full credit profile established with 5–7 active trade lines
```

**Expected Outcome (Day 90):**
- 2 Layer 0 vendors (Uline, Grainger)
- 2–3 Layer 1A vendors (Adobe, Slack, Zoom)
- 1 Layer 1B vendor (AWS)
- 2 Layer 2 vendors (WEX or AtoB, Nav Prime)
- Total: 6–7 active trade lines with diverse reporting frequencies

---

## Dependency Matrix

| Vendor | Prerequisites | Blocks | Optimal Activation Window |
| :--- | :--- | :--- | :--- |
| **Uline** | None | None (gates Layer 0) | Day 1 |
| **Grainger** | Uline posting | None (gates Layer 0) | Day 3–5 |
| **Adobe/Slack/Zoom** | Layer 0 posting (not strictly required, but improves odds) | None (gates Layer 1) | Days 15–25 |
| **AWS** | Layer 0 posting (credit check dependency) | None | Days 25–35 |
| **WEX/AtoB** | Layer 0 posting + 2–3 Layer 1 vendors active | None | Days 35–50 |
| **Nav Prime** | None (independent) | None | Days 1–90 (flexible) |

---

## Ghost Balance Mitigation Checklist

**For every vendor, apply this protocol to prevent non-reporting:**

| Step | Timing | Action | Verification |
| :--- | :--- | :--- | :--- |
| **1. Order Placement** | Day 0 | Place order with vendor. | Order confirmation received. |
| **2. Invoice Generation** | Day 5–10 (typical) | Wait for "Invoice Generated" or "Statement Available" email. | Invoice ID visible in vendor portal. |
| **3. Payment Window Opens** | 48 hours post-invoice | Begin payment execution window. | Manual confirmation: invoice is "booked" in vendor system. |
| **4. Payment Execution** | 48 hours–5 days pre-due date | Execute ACH transfer from business bank account. | Payment confirmation from business bank. |
| **5. Bureau Posting** | 10–15 days post-payment | Verify vendor has reported to D&B. | D&B query shows: Usage → Invoiced → Paid Early. |

**Critical:** Do not deviate from the 48-hour/5-day window without explicit finance approval.

---

## Document Status
**APPROVED FOR USE IN SENTINEL_BOARDROOM**  
**Next Review:** Upon Layer 2 vendor activation (expected Day 60)  
**Maintained By:** Finance Department
