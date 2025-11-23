# EIN_Bank_Account_Separation_Blueprint.md
Multi-Entity Banking & EIN Strategy • Sentinel Labs Finance Department  
**Version:** 1.0 | **Last Updated:** 2025-11-23 | **Audience:** Founder / Finance Team | **Status:** Internal Strategy

---

## Executive Summary

This blueprint outlines how to establish separate EINs and banking infrastructure across multiple business entities, enabling:
- **Financial segregation** (clear accounting boundaries)
- **Credit building** (independent credit profiles per entity)
- **Risk isolation** (liability separation)
- **Operational clarity** (distinct revenue streams, P&Ls, tax filings)

**Use case:** Sentinel Labs operating as a holding company with subsidiary entities for different business lines (e.g., web studio, coherence computing, research divisions).

**This document covers:**
- EIN basics and multi-entity structure
- Bank account segregation strategy
- Fund flow architecture
- Tax implications
- Compliance and documentation
- Implementation timeline

---

## Part 1: EIN Fundamentals

### What is an EIN?

**EIN = Employer Identification Number**
- Issued by the IRS
- Unique identifier for business entities (like SSN for individuals)
- Required for: banking, payroll, tax filing, contracts
- Format: XX-XXXXXXX (9 digits)

**Key fact:** Every legal entity needs its own EIN (holding company, subsidiary, LLC, corp—all separate).

### Why Separate EINs Matter

**Single EIN (all entities under one number):**
- ✗ All revenue mixed together
- ✗ Difficult to track subsidiary performance
- ✗ Tax filings complex (commingled income)
- ✗ Can't establish independent credit for subsidiaries
- ✗ Hard to sell or spin-off entities later

**Multiple EINs (one per entity):**
- ✓ Clean financial separation
- ✓ Independent credit profiles
- ✓ Clear P&L per business line
- ✓ Easier tax planning (some entities taxed differently)
- ✓ Scalable (add entities as business grows)
- ✓ Facilitates future transactions (sale, spin-off, merger)

---

## Part 2: Multi-Entity Structure for Sentinel Labs

### Recommended Entity Architecture

**Option A: Holding Company + Operating Subsidiaries**

```
SENTINEL LABS, INC. (Delaware C-Corp)
├─ EIN: 98-765432 (Holding Company)
├─ Purpose: Parent entity, holds equity in subsidiaries
├─ Bank Account: Treasury (minimal operating activity)
│
├─ SENTINEL STUDIO, LLC (Delaware LLC)
│  ├─ EIN: 98-765433
│  ├─ Purpose: Web design, branding, marketing services
│  ├─ Revenue: $X annually
│  ├─ Bank Accounts: Operating (checks, payroll)
│  └─ Tax: Pass-through (taxed at holding company level)
│
├─ SENTINEL CAPITAL, LLC (Delaware LLC)
│  ├─ EIN: 98-765434
│  ├─ Purpose: Finance operations, credit building, lending
│  ├─ Revenue: $Y annually
│  ├─ Bank Accounts: Operating (credit lines, vendor payments)
│  └─ Tax: Pass-through (taxed at holding company level)
│
└─ SENTINEL RESEARCH, LLC (Delaware LLC)
   ├─ EIN: 98-765435
   ├─ Purpose: Coherence computing research, IP development
   ├─ Revenue: Grants, licensing (research focused)
   ├─ Bank Accounts: Operating (research expenses, vendor payments)
   └─ Tax: Pass-through (taxed at holding company level)
```

**Why this structure:**
- Holding company owns all subsidiaries (100% ownership)
- Each subsidiary has independent EIN and banking
- Each subsidiary can have separate credit profile
- Holding company can allocate funds to subsidiaries as needed
- Subsidiaries pass through income to holding company (consolidated tax)

**Alternative: Separate Operating Companies (No Holding Company)**

```
SENTINEL STUDIO, LLC (EIN: 98-765433)
├─ Bank accounts: Operating
├─ Credit profile: Independent
└─ Taxes: File separately

SENTINEL CAPITAL, LLC (EIN: 98-765434)
├─ Bank accounts: Operating
├─ Credit profile: Independent
└─ Taxes: File separately

SENTINEL RESEARCH, LLC (EIN: 98-765435)
├─ Bank accounts: Operating
├─ Credit profile: Independent
└─ Taxes: File separately
```

**Pros:** Simple, independent
**Cons:** No parent entity to coordinate, harder to allocate profits, more complex equity ownership

**Recommendation:** Use holding company structure (Option A) for scalability and founder equity clarity.

---

## Part 3: EIN Registration Process

### Step 1: Register Business Entity First

**For each entity (subsidiary), register in Delaware (or chosen state):**

1. **Prepare articles of organization** (LLC) or incorporation (Corp)
   - Entity name
   - Registered agent
   - Manager/member or director/officer info
   - Operating agreement terms

2. **File with state** (Delaware Division of Corporations)
   - Online filing: $90–$150
   - Timeline: 1–3 business days
   - Receive: Certificate of formation/incorporation

3. **Record in company files**
   - Save certificate
   - Keep operating agreement
   - Document formation date

---

### Step 2: Apply for EIN (IRS)

**After entity is registered, apply for EIN:**

**Method 1: Online (Fastest)**
- Go to IRS.gov → EIN search
- Select "Apply for an EIN online"
- Answer questions about entity and owners
- Receive EIN immediately (same screen)
- Print confirmation
- Timeline: 15 minutes

**Method 2: Phone**
- Call IRS Business Line: 1-800-829-4933
- Provide same information
- Receive EIN verbally
- Confirmation mailed within 2 weeks
- Timeline: 30 minutes on hold

**Method 3: Mail (Slowest)**
- Complete Form SS-4
- Mail to IRS address (varies by state)
- Receive EIN by mail
- Timeline: 2–4 weeks

**Recommendation:** Use online method (fastest, instant confirmation).

---

### Step 3: Document EIN Assignment

**For each entity, record:**

| Entity Name | EIN | Registration Date | State | Entity Type | Primary Contact | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Sentinel Labs, Inc. | 98-765432 | 2025-01-15 | Delaware | C-Corp | Founder | Holding company |
| Sentinel Studio, LLC | 98-765433 | 2025-01-20 | Delaware | LLC | Operations Lead | Web/marketing |
| Sentinel Capital, LLC | 98-765434 | 2025-01-22 | Delaware | LLC | Finance Lead | Finance operations |
| Sentinel Research, LLC | 98-765435 | 2025-01-25 | Delaware | LLC | Research Lead | Coherence research |

**Store in:**
- Company file (physical and digital)
- Finance software (QuickBooks, Stripe Atlas records)
- Bank documents (provided with account opening)

---

## Part 4: Bank Account Segregation Strategy

### Account Hierarchy

**Recommended structure:**

```
HOLDING COMPANY (Sentinel Labs, Inc.)
├─ Primary Treasury Account
│  ├─ Purpose: Consolidated fund management
│  ├─ Activity: Fund transfers between subsidiaries
│  └─ Balance: Minimal (daily operations handled at subsidiary level)

SUBSIDIARY 1 (Sentinel Studio, LLC)
├─ Operating Checking Account
│  ├─ Purpose: Daily operations, payroll, vendor payments
│  ├─ Activity: High (customer invoices, payroll, supplies)
│  └─ Balance: 1–3 months operating expense reserve
│
├─ Savings Account (Optional)
│  ├─ Purpose: Emergency cash, short-term projects
│  ├─ Activity: Low (strategic withdrawals)
│  └─ Balance: $25K–$100K

SUBSIDIARY 2 (Sentinel Capital, LLC)
├─ Operating Checking Account
│  ├─ Purpose: Credit operations, vendor management
│  ├─ Activity: High (vendor payments, credit line draws)
│  └─ Balance: 1–3 months operating expense reserve
│
├─ Vendor Credit Account (Optional)
│  ├─ Purpose: Vendor deposits, term line management
│  ├─ Activity: Medium (credit line draws, vendor payments)
│  └─ Balance: Available credit limit

SUBSIDIARY 3 (Sentinel Research, LLC)
├─ Research Checking Account
│  ├─ Purpose: Grant funding, research expenses
│  ├─ Activity: Grant-dependent (seasonal)
│  └─ Balance: 2–6 months operating expense reserve
```

---

### Bank Selection by Entity & Purpose

**Holding Company: Primary Treasury Account**

**Best banks:**
- Wells Fargo / Bank of America (strong D&B reporting, relationship banking)
- Chase (credit products, treasury services)
- Mercury (modern, API-friendly for transfers)

**Why:** 
- Low activity (minimal fees)
- Strong banking relationship (matters for holding company)
- Facilitates inter-company transfers

**Subsidiaries: Operating Accounts**

**Best banks (multiple recommendations):**

**Primary (Tier 1):**
- Wells Fargo Business
- Bank of America Business
- Chase Business

Why: Reports to D&B, strong credit building, business services

**Secondary (Operational):**
- Mercury (fast transfers, clean interface)
- Brex (if you have good credit history)
- Wise (international transfers, if needed)

Why: Operational convenience, lower fees for transactions

**Recommendation:** Open at least 2 accounts per subsidiary (Tier 1 + operational).

---

### Account Opening Requirements (Per Entity)

**Documents needed for each account:**

1. **Business registration documents**
   - Certificate of formation/incorporation
   - Operating agreement (LLC) or bylaws (Corp)
   - EIN confirmation letter (from IRS)

2. **Ownership documentation**
   - Ownership structure (who owns the entity)
   - Authorized signers (who can access account)
   - Beneficial ownership declaration (FinCEN requirement)

3. **ID and personal information**
   - Founder photo ID
   - Founder SSN
   - Manager/member names and SSNs
   - Business address and phone

4. **Tax information**
   - EIN (from IRS)
   - Expected annual revenue
   - Business purpose / industry classification

**Timeline:** 1–2 weeks from application to account opening

**Cost:** $0 for most business accounts (no minimum balance)

---

## Part 5: Fund Flow Architecture

### Inter-Company Transfers (How Money Moves)

**Scenario: Holding company receives equity investment; distributes to subsidiaries for operations**

```
INVESTOR DEPOSITS $5M → SENTINEL LABS (HOLDING COMPANY)
│
└─ Holding company receives funds
   ├─ Holds $500K as treasury reserve
   │
   ├─ Transfers $2M → SENTINEL STUDIO LLC
   │  └─ Studio uses for: payroll, ops, marketing
   │
   ├─ Transfers $1M → SENTINEL CAPITAL LLC
   │  └─ Capital uses for: vendor relationships, credit building
   │
   └─ Transfers $1.5M → SENTINEL RESEARCH LLC
      └─ Research uses for: equipment, grants, development
```

**How to execute transfers:**

**Method 1: Wire Transfer (Most Professional)**
- Initiate from holding company account
- Route to subsidiary account ABA/routing number
- Fee: $0–$15 per wire
- Speed: Same day or next day
- Record: Required for accounting

**Method 2: ACH Transfer (Slower, Cheaper)**
- Initiate from holding company account
- Route via ACH (3–5 business days)
- Fee: $0–$5 per transfer
- Speed: 3–5 business days
- Record: Required for accounting

**Method 3: Check (Old-School but Clear)**
- Holding company writes check to subsidiary
- Subsidiary deposits check
- Fee: Minimal
- Speed: 5–7 business days (clearing time)
- Record: Clear paper trail

**Recommendation:** Use ACH for routine transfers (cheaper, fast enough). Use wire for urgent/large transfers.

---

### Fund Flow Tracking

**Create tracking spreadsheet:**

| Date | From Entity | To Entity | Amount | Purpose | Transfer ID | Recorded Y/N |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 2025-01-15 | Sentinel Labs | Sentinel Studio | $2,000,000 | Initial operating capital | Wire 12345 | Yes |
| 2025-01-15 | Sentinel Labs | Sentinel Capital | $1,000,000 | Credit building fund | Wire 12346 | Yes |
| 2025-01-15 | Sentinel Labs | Sentinel Research | $1,500,000 | Research operations | Wire 12347 | Yes |
| 2025-02-01 | Sentinel Studio | Sentinel Labs | $50,000 | Profit distribution | ACH 9876 | Yes |

**Purpose:** Clear audit trail showing fund movements and justification.

---

### Accounting Records (Critical for IRS)

**Each entity must maintain:**

1. **Separate general ledger**
   - All transactions recorded by entity
   - Transfers clearly marked as inter-company
   - No commingling of accounts

2. **Bank reconciliation (monthly)**
   - Match bank statement to ledger
   - Identify all transfers
   - Flag any discrepancies

3. **Inter-company agreements (optional but recommended)**
   - Document the terms of any inter-company loans or transfers
   - Shows legitimate business purpose
   - Protects in IRS audit

**Example inter-company agreement:**

```
INTER-COMPANY FUND TRANSFER AGREEMENT

Between: Sentinel Labs, Inc. (Lender)
And: Sentinel Studio, LLC (Borrower)

Terms:
- Amount: $2,000,000
- Date: January 15, 2025
- Purpose: Operating capital for web design and marketing operations
- Term: No repayment required (equity contribution)
- Interest: None

Both parties acknowledge this transfer as a capital contribution
to Sentinel Studio, LLC, authorized by board resolution.
```

---

## Part 6: Tax Implications of Separation

### Entity Taxation

**Holding Company (C-Corp, Sentinel Labs, Inc.):**
- Taxed at corporate level (21% federal rate)
- If subsidiaries pass through income: Holding company pays tax on combined subsidiary income
- Alternative: Holding company elects S-Corp status (pass-through to founder personal tax)

**Subsidiaries (LLC, pass-through):**
- No entity-level tax
- Income passes through to holding company (or to members if standalone)
- Holding company (or founder) pays tax on income

**Example (assuming Sentinel Labs is C-Corp holding company):**

```
Year 1 Scenario:

Sentinel Studio LLC
├─ Revenue: $5,000,000
├─ Expenses: $3,500,000
└─ Net income: $1,500,000 (passes to Sentinel Labs)

Sentinel Capital LLC
├─ Revenue: $500,000
├─ Expenses: $200,000
└─ Net income: $300,000 (passes to Sentinel Labs)

Sentinel Research LLC
├─ Revenue: $0 (research, not revenue-generating)
├─ Expenses: $800,000
└─ Net loss: ($800,000) (losses reduce Sentinel Labs taxable income)

SENTINEL LABS CONSOLIDATED TAXABLE INCOME:
$1,500,000 + $300,000 - $800,000 = $1,000,000
Tax owed (C-Corp 21% rate): $210,000
```

### Separate Tax Filings

**Each entity files its own return (if required):**

| Entity | Return Type | Filing Deadline | Cost | Purpose |
| :--- | :--- | :--- | :--- | :--- |
| Sentinel Labs (C-Corp) | Form 1120 | March 15 (or extended) | $500–$2K CPA | Consolidated income |
| Sentinel Studio (LLC) | Form 1065 (partnership return) | March 15 | Included in Sentinel Labs | Pass-through income |
| Sentinel Capital (LLC) | Form 1065 (partnership return) | March 15 | Included in Sentinel Labs | Pass-through income |
| Sentinel Research (LLC) | Form 1065 (partnership return) | March 15 | Included in Sentinel Labs | Pass-through income, R&D deductions |

**Key advantage of separation:** Research LLC losses can offset other subsidiaries' income, reducing total tax burden.

---

### Payroll Taxes (Multi-Entity Considerations)

**If subsidiaries have employees:**

**Each entity files separate payroll:**

```
Sentinel Studio LLC
├─ Employees: 5
├─ Payroll: $500K annually
├─ Payroll taxes: 7.65% (FICA) + State unemployment
└─ Files: Form 941 (quarterly) + Form 940 (annual)

Sentinel Capital LLC
├─ Employees: 2
├─ Payroll: $200K annually
├─ Payroll taxes: 7.65% (FICA) + State unemployment
└─ Files: Form 941 (quarterly) + Form 940 (annual)

Sentinel Research LLC
├─ Employees: 3
├─ Payroll: $300K annually
├─ Payroll taxes: 7.65% (FICA) + State unemployment
└─ Files: Form 941 (quarterly) + Form 940 (annual)
```

**Why separate:** Each entity has its own EIN, so payroll is filed separately. Clear accounting per division.

---

## Part 7: Compliance & Regulatory Requirements

### State Filing Obligations

**For each entity registered in Delaware:**

**Annual requirements:**

1. **Delaware Division of Corporations:**
   - Annual report due: June 30
   - Fee: $25 per entity
   - Form: DSCB: Annual Report
   - Purpose: Register continued existence

2. **Federal (IRS):**
   - Form 1120 (C-Corp) or Form 1065 (LLC partnership return)
   - Due: March 15 (or extended to Sept 15)
   - Purpose: Report taxable income

3. **State income tax return (if applicable):**
   - Varies by state (Delaware has no income tax for LLCs, but if operating in other states, file there)
   - Varies by timeline

**All entities must file:**
- ✓ Annual Delaware report (if registered there)
- ✓ Federal income tax return
- ✓ Payroll tax returns (if employees)
- ✓ Sales tax returns (if applicable to business)

---

### FinCEN Beneficial Ownership Registration

**All entities must comply with Corporate Transparency Act (CTA):**

**Requirement:** Report beneficial owners (anyone owning 25%+) to FinCEN

**Who needs to file:**
- All new entities (registered after Jan 1, 2024)
- Most existing entities (deadline: Jan 1, 2025)

**What to report:**
- Entity name and EIN
- Beneficial owner names, DOBs, addresses
- Who filed (if applicant)

**How:** FinCEN Beneficial Ownership Information (BOI) reporting system

**Timeline:** Due at incorporation (or Jan 1, 2025 for existing entities)

**Cost:** $0 (free, though CPA may charge for filing)

**Failure to file:** Civil penalty up to $500/day; criminal penalties up to $5K fine + 2 years imprisonment

---

### IRS Notices & Audits

**With separate entities, increased complexity:**

**IRS may audit:**
- Individual entity returns (1065, 1120)
- Holding company consolidated return
- Inter-company transactions (making sure they're legitimate)
- Transfer pricing (if subsidiaries are invoicing each other)

**How to prepare:**
- Keep detailed records of all inter-company transactions
- Document business purpose for transfers
- Maintain clean accounting (separate GL per entity)
- Have CPA review before filing

---

## Part 8: Implementation Timeline

### Phase 1: Entity Registration (Weeks 1–2)

**Week 1:**
- [ ] Prepare articles of organization for each subsidiary
- [ ] File with Delaware Division of Corporations (online)
- [ ] Receive certificates of formation

**Week 2:**
- [ ] Apply for EIN for each entity (online)
- [ ] Receive EINs immediately
- [ ] Record EINs in master spreadsheet

---

### Phase 2: Bank Account Opening (Weeks 2–4)

**Week 2–3:**
- [ ] Gather documents for holding company account
- [ ] Apply for treasury account (Tier 1 bank)
- [ ] Receive account approval and debit card

**Week 3–4:**
- [ ] Gather documents for each subsidiary
- [ ] Apply for operating accounts (Tier 1 banks)
- [ ] Apply for secondary accounts (operational banks)
- [ ] Receive all account approvals

---

### Phase 3: Accounting Setup (Week 4–5)

**Week 4:**
- [ ] Set up accounting software (QuickBooks or similar)
- [ ] Create separate chart of accounts for each entity
- [ ] Document account mapping (GL codes per entity)

**Week 5:**
- [ ] Set up inter-company accounts (clearing accounts for transfers)
- [ ] Test ACH/wire transfer process
- [ ] Train finance team on account usage

---

### Phase 4: Documentation & Compliance (Week 5–6)

**Week 5:**
- [ ] Prepare inter-company agreements
- [ ] Create fund transfer documentation
- [ ] File FinCEN BOI reports

**Week 6:**
- [ ] Register all entities for state taxes (if applicable)
- [ ] Set up payroll system (if hiring)
- [ ] Schedule annual compliance calendar reminders

---

## Part 9: Account Usage Best Practices

### Holding Company Treasury Account

**Purpose:** Coordinate funding and consolidate cash

**Usage guidelines:**
- Primary inflow: Investor capital, revenue from subsidiaries
- Primary outflow: Fund transfers to subsidiaries
- Transactions per month: 1–10 (low activity)
- Minimum balance: $50K–$500K (depends on subsidiary needs)

**Do:**
- ✓ Use for strategic fund allocation
- ✓ Keep clean (minimal day-to-day activity)
- ✓ Document all transfers with business purpose

**Don't:**
- ✗ Use for operating expenses (subsidiaries handle that)
- ✗ Mix personal and business funds
- ✗ Make undocumented transfers

---

### Subsidiary Operating Accounts

**Purpose:** Handle day-to-day operations, payroll, vendor payments

**Usage guidelines:**
- Primary inflow: Fund transfers from holding company, customer revenue
- Primary outflow: Payroll, vendor payments, operational expenses
- Transactions per month: 50–500 (high activity)
- Minimum balance: 1–3 months operating expenses

**Do:**
- ✓ Use for all operational expenses
- ✓ Reconcile monthly
- ✓ Keep separate from other subsidiaries

**Don't:**
- ✗ Commingle with holding company day-to-day activity
- ✗ Mix business and personal expenses
- ✗ Transfer between subsidiaries (route through holding company)

---

### Subsidiary Secondary Accounts (Optional)

**Purpose:** Operational convenience, faster transfers, backup account

**Usage guidelines:**
- Used for: High-frequency transactions, payroll, transfers
- Balance: Minimal ($10K–$50K)
- Purpose: Speed (ACH, checks clear faster at online banks)

**Best uses:**
- Payroll account (if using payroll service that requires bank connection)
- Vendor payment account (if high frequency vendor payments)
- Backup account (if primary account is down)

---

## Part 10: Segregation Best Practices

### Financial Isolation Checklist

**Ensure clear separation:**

- [ ] Each entity has separate EIN (registered with IRS)
- [ ] Each entity has separate bank account(s) at different banks
- [ ] Each entity has separate business name and branding
- [ ] Each entity has separate business address (or clear designation)
- [ ] Each entity maintains separate accounting records (GL, journal, ledger)
- [ ] Transfers between entities are documented with business purpose
- [ ] No commingling of funds or accounts
- [ ] No co-signing of documents (each entity signs separately)
- [ ] Board/management decisions made separately for each entity
- [ ] Contracts specify which entity is party to agreement

---

### Audit Trail Documentation

**Create master documentation for each entity:**

**Holding Company File:**
- [ ] Certificate of incorporation
- [ ] Bylaws
- [ ] EIN confirmation letter
- [ ] Board resolutions (fund transfers, subsidiary equity grants)
- [ ] Ownership documentation
- [ ] Bank account agreements

**Subsidiary File (per subsidiary):**
- [ ] Certificate of formation
- [ ] Operating agreement
- [ ] EIN confirmation letter
- [ ] Board/member resolutions
- [ ] Ownership structure (held by holding company)
- [ ] Bank account agreements (operating + secondary)
- [ ] Fund transfer documentation (from holding company)

**Finance File (Master):**
- [ ] Consolidated EIN registry (all entities)
- [ ] Consolidated bank account registry (all accounts, all entities)
- [ ] Fund transfer tracking (holding company → subsidiaries)
- [ ] Inter-company agreement templates
- [ ] Accounting policy (how transfers recorded)

---

## Part 11: Troubleshooting & Edge Cases

### Scenario A: Bank Rejects Inter-Company Transfer

**Problem:** Bank flags transfer between entities as suspicious

**Why it happens:**
- Same owner, but different entities
- Bank's compliance system thinks it's unusual

**Solution:**
1. Call bank, explain: "These are subsidiaries under same holding company"
2. Provide: Documentation of ownership structure
3. Bank may request: Inter-company agreement (showing business purpose)
4. Whitelist transfer: Bank may ask to pre-approve pattern going forward

**Prevention:**
- Proactively inform bank of multi-entity structure when opening account
- Provide board resolutions showing fund transfers are authorized
- Use same bank for holding company + subsidiaries (if possible)

---

### Scenario B: IRS Questions Inter-Company Transaction

**Problem:** IRS audit asks about transfer, questions business purpose

**Why it happens:**
- Undocumented transfer
- Transfer amount seems large/unusual
- Missing supporting documentation

**Solution:**
1. Respond with: Board resolution authorizing transfer
2. Provide: Inter-company agreement showing business purpose
3. Show: How funds were used (subsidiary accounting records)
4. Demonstrate: Legitimate business reason

**Prevention:**
- Document ALL inter-company transfers with business purpose
- Keep board resolution before fund transfer
- Maintain separate accounting per entity (shows funds used legitimately)

---

### Scenario C: Subsidiary Becomes Insolvent

**Problem:** Subsidiary can't pay debts, needs restructuring

**Benefit of separation:**
- ✓ Holding company is protected (subsidiary is separate entity)
- ✓ Other subsidiaries unaffected
- ✓ Founder's personal assets protected (LLC liability shield)

**If subsidiary fails:**
- Creditors of Subsidiary A can't pursue Holding Company or Subsidiary B
- Shareholders may lose equity in Subsidiary A, but other assets protected

**Key reason for multi-entity structure.**

---

## Part 12: Scaling: Adding More Entities

### Process for Adding New Subsidiary (Future)

**Timeline: 2 weeks**

**Week 1:**
1. Prepare articles of formation (new entity)
2. Register with Delaware
3. Apply for EIN
4. Board resolution (holding company approves subsidiary creation)

**Week 2:**
1. Open bank account (new subsidiary)
2. Document ownership (holding company owns 100%)
3. Update cap table
4. Update accounting software (add new GL)

**That's it.** Same process, can be repeated as needed.

---

## Part 13: Checklist: Complete EIN/Bank Separation

**Pre-launch:**
- [ ] Defined entity structure (holding company + subsidiaries)
- [ ] Identified business lines (what each subsidiary does)
- [ ] Chose jurisdiction (Delaware recommended)
- [ ] Founder approval of structure

**Registration:**
- [ ] Articles of organization filed for each entity
- [ ] EIN applied for and received for each entity
- [ ] EINs recorded in master registry
- [ ] Certificates of formation stored

**Banking:**
- [ ] Bank selected for holding company (Tier 1)
- [ ] Bank selected for each subsidiary (Tier 1 + Tier 2)
- [ ] Accounts opened for all entities
- [ ] Account details recorded (ABA, routing, account #)

**Accounting:**
- [ ] Accounting software set up (QuickBooks or similar)
- [ ] Chart of accounts created per entity
- [ ] Inter-company accounts established
- [ ] Bank reconciliation process documented

**Compliance:**
- [ ] FinCEN BOI filed (if required)
- [ ] Inter-company agreements prepared
- [ ] Board resolutions documented (fund transfers authorized)
- [ ] Annual compliance calendar set up

**Operational:**
- [ ] Finance team trained on fund transfer process
- [ ] Fund transfer documentation templates created
- [ ] Fund flow tracking spreadsheet active
- [ ] Monthly reconciliation process in place

---

## Part 14: FAQ: EIN & Bank Separation

**Q: Do I really need separate banks for each entity?**
A: No, but it's recommended. Single bank with multiple accounts (one per entity) works, but separate banks create cleaner separation. At minimum, keep accounts separate within same bank.

**Q: What if I'm a single-entity business?**
A: You only need one EIN and one bank account. But if you plan to grow or spin off divisions, set up structure now (easier than retrofitting later).

**Q: Can I have one EIN for multiple entities?**
A: No. IRS requires one EIN per entity. Attempting to use one EIN for multiple entities triggers IRS problems.

**Q: How much does EIN registration cost?**
A: $0. EIN is free from IRS (online, instant).

**Q: How much does setting up bank accounts cost?**
A: $0. Most business banks waive fees for business accounts (no minimum balance). Cost is only if you need special services (wire transfers, lockbox, etc.).

**Q: Can I use my personal SSN for business account?**
A: No. Business account requires EIN (employer ID). Your SSN is used for personal guarantee (founder identification), but primary account identifier is EIN.

**Q: What's a W-9 and does each entity need one?**
A: W-9 is tax form showing who you are. Yes, each entity needs its own W-9 if they invoice customers. Banks may request W-9 during account opening.

**Q: Can I combine accounting for multiple entities in one QuickBooks file?**
A: Yes, but creates confusion. Better to have separate QB company file per entity, then consolidate for holding company reporting.

**Q: What if a subsidiary operates in multiple states?**
A: Register holding company in Delaware (preferred for business). Subsidiaries can operate in any state without re-registering (they're owned by Delaware entity). But may need to file for "foreign LLC" status in operating state (low cost, paperwork).

**Q: Can founder personally guarantee subsidiary accounts?**
A: Yes, common for startups. Bank asks for founder's personal guarantee on subsidiary account (ensures someone is accountable). This is normal; doesn't undermine liability protection.

---

## Status: Ready for Founder Approval

This EIN and bank account separation blueprint is complete and ready for implementation.

**Next steps (upon approval):**
1. Founder reviews and approves entity structure
2. Finance team begins entity registration (Week 1)
3. Finance team opens bank accounts (Week 2–4)
4. Finance team sets up accounting (Week 4–5)
5. Finance team completes compliance documentation (Week 5–6)
6. Finance team trains operations team on fund flows
7. System live for operations

---

**Document Owner:** Finance Department / Founder  
**Last Updated:** 2025-11-23  
**Classification:** Internal Finance — Multi-Entity Strategy  
**Status:** Active — Ready for Implementation
