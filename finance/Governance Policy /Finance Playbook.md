# Founder_Vesting_Schedule_4_Year_1_Year_Cliff.md
Equity Vesting Framework • Sentinel Labs Finance Department  
**Version:** 1.0 | **Last Updated:** 2025-11-23 | **Audience:** Founder / Finance Team | **Status:** Internal Strategy

---

## Executive Summary

This document outlines the standard founder equity vesting schedule: **4-year vesting with 1-year cliff**.

**What this means:**
- Founder receives 0% equity until 1 year of service (cliff)
- After cliff, equity vests monthly: 1/48 of total per month
- Full vesting: 4 years from grant date
- Industry standard for founder-controlled companies

**Why vesting matters:**
- Protects company if founder leaves early
- Aligns founder incentives with long-term building
- Supports investor confidence (equity locked in)
- Manages tax obligations (Section 83(b) election)

**This document covers:**
- Vesting mechanics and calculations
- Multiple founder scenarios
- Tax implications
- Cliff protection rationale
- Acceleration triggers (fundraising, sale, departure)
- Implementation and documentation

---

## Part 1: Vesting Mechanics

### The 4-Year / 1-Year Cliff Schedule

**Standard structure:**

```
Year 1: CLIFF
├─ Month 0–11: 0% vesting (equity locked)
├─ Month 12: CLIFF TRIGGER
└─ Month 12 completion: 25% vests (1 year of service earned)

Year 2: LINEAR VESTING
├─ Months 13–24: 1/48 vests per month (12 months × 1/48)
└─ Cumulative at Month 24: 50% vested

Year 3: LINEAR VESTING
├─ Months 25–36: 1/48 vests per month (12 months × 1/48)
└─ Cumulative at Month 36: 75% vested

Year 4: LINEAR VESTING
├─ Months 37–48: 1/48 vests per month (12 months × 1/48)
└─ Cumulative at Month 48: 100% vested (fully vested)
```

### Monthly Vesting Calculation

**Formula:**

```
Monthly vesting amount = Total founder shares ÷ 48 months

Example:
Founder granted 1,000,000 shares
Monthly vesting = 1,000,000 ÷ 48 = 20,833 shares/month

After 1 year (cliff): 20,833 × 12 = 250,000 shares vested (25%)
After 2 years: 250,000 + (20,833 × 12) = 500,000 shares vested (50%)
After 3 years: 500,000 + (20,833 × 12) = 750,000 shares vested (75%)
After 4 years: 750,000 + (20,833 × 12) = 1,000,000 shares vested (100%)
```

### Vesting Trigger: Service Requirement

**Vesting happens automatically based on continued service:**

- **Employed/Active**: Vesting continues on schedule
- **Leave Company**: Vesting stops immediately
- **Terminated for Cause**: Vesting stops; unvested shares forfeit
- **Terminated without Cause**: Cliff still applies; post-cliff shares typically allowed to vest through departure date

**Example timeline:**

| Scenario | Departure Month | Vested at Departure | Forfeited |
| :--- | :--- | :--- | :--- |
| **Quits Year 1** | Month 11 | 0 shares (pre-cliff) | 100% |
| **Quits at Year 1** | Month 12 | 250,000 (post-cliff) | 750,000 |
| **Quits Year 2** | Month 20 | 333,333 (cliff + 8 months) | 666,667 |
| **Quits Year 3** | Month 36 | 750,000 (cliff + 24 months) | 250,000 |
| **Completes all 4 years** | Month 48 | 1,000,000 (100%) | 0 |

---

## Part 2: Founder Scenarios

### Scenario A: Single Founder, Full Control

**Grant details:**
- Total shares issued: 10,000,000 common shares
- Founder grant: 10,000,000 shares (100% ownership)
- Vesting schedule: 4-year cliff at 1 year

**Vesting breakdown:**

| Milestone | Months | Cumulative Vested | Percentage | Notes |
| :--- | :--- | :--- | :--- | :--- |
| Grant date | 0 | 0 | 0% | Shares granted but locked |
| Cliff vests | 12 | 2,500,000 | 25% | First year service earned |
| Year 2 end | 24 | 5,000,000 | 50% | Half company vested |
| Year 3 end | 36 | 7,500,000 | 75% | Three-quarters vested |
| Year 4 end | 48 | 10,000,000 | 100% | Fully vested; full control |

**Tax implication (Section 83(b)):**
- Founder must elect 83(b) to start tax clock at grant (recommended)
- Without 83(b): Tax liability deferred until vesting
- With 83(b): Single lump-sum tax at grant, no ongoing tax burden

---

### Scenario B: Co-Founders (Equal Split)

**Grant details:**
- Total shares: 10,000,000
- Founder A: 5,000,000 shares (50%)
- Founder B: 5,000,000 shares (50%)
- Both on 4-year/1-year cliff

**Vesting schedule (parallel):**

| Time | Founder A Vested | Founder B Vested | Total Vested | Control Notes |
| :--- | :--- | :--- | :--- | :--- |
| Month 0 | 0 (0%) | 0 (0%) | 0 (0%) | Neither has voting control (pre-cliff) |
| Month 12 | 1,250,000 (25%) | 1,250,000 (25%) | 2,500,000 (25%) | Both equal; post-cliff |
| Month 24 | 2,500,000 (50%) | 2,500,000 (50%) | 5,000,000 (50%) | Both 50% of company |
| Month 36 | 3,750,000 (75%) | 3,750,000 (75%) | 7,500,000 (75%) | Both still equal |
| Month 48 | 5,000,000 (100%) | 5,000,000 (100%) | 10,000,000 (100%) | Both fully vested |

**Key advantage of equal co-founder vesting:**
- Mutual protection: If A leaves Year 1 (pre-cliff), B retains 100% voting control
- Cliff ensures commitment: Must stay 1 year for equity benefit
- Symmetrical incentives: Both aligned to build long-term

**Disadvantage:**
- Deadlock risk: 50/50 split can cause decision gridlock
- Consider governance: Should one founder have board seat / tiebreaker?

---

### Scenario C: Founder + Early Employee (Unequal Split)

**Grant details:**
- Total shares: 10,000,000
- Founder: 8,000,000 shares (80%)
- Early employee: 2,000,000 shares (20%)
- Both on 4-year/1-year cliff

**Vesting schedule:**

| Time | Founder Vested | Employee Vested | Founder % | Employee % |
| :--- | :--- | :--- | :--- | :--- |
| Month 0 | 0 | 0 | 0% | 0% |
| Month 12 | 2,000,000 | 500,000 | 25% | 25% |
| Month 24 | 4,000,000 | 1,000,000 | 50% | 50% |
| Month 36 | 6,000,000 | 1,500,000 | 75% | 75% |
| Month 48 | 8,000,000 | 2,000,000 | 100% | 100% |

**Control dynamics:**
- **Pre-cliff (Month 0–11):** Founder has 100% voting control (employee's equity locked)
- **Post-cliff (Month 12+):** Founder has 80% control; employee has 20% voting rights
- **Year 4 (Month 48+):** Control ratios remain 80/20 (both fully vested)

---

### Scenario D: Multiple Founders + Investor (Post-SAFE)

**Context:** Company raised $5M on SAFE; now implementing founder equity.

**Grant details:**
- Total shares pre-SAFE: 10,000,000
- Post-SAFE conversion: Assume 20% dilution (investor converts to 20%)
- Adjusted founder pool: 8,000,000 shares (80%)
  - Founder A: 4,000,000 (40%)
  - Founder B: 4,000,000 (40%)
- Vesting: 4-year/1-year cliff for both

**Cap table (post-investor conversion):**

| Holder | Shares | Pre-Cliff % | Post-Cliff % | Notes |
| :--- | :--- | :--- | :--- | :--- |
| Founder A | 4,000,000 | 0% | 10% | Month 12 cliff |
| Founder B | 4,000,000 | 0% | 10% | Month 12 cliff |
| Investor | 2,000,000 | 20% | 20% | Fully vested immediately |
| **Total** | **10,000,000** | **20% vested** | **40% vested** | **Post-cliff** |

**Key insight:**
- Pre-cliff (months 0–11): Investor has 100% voting control (both founders' equity locked)
- Post-cliff (month 12+): Control shifts to 40% founders + 20% investor
- This protects investor until founders prove commitment

---

## Part 3: Tax Implications

### Section 83(b) Election (Critical)

**What is 83(b)?**
- IRS tax code section allowing restricted stock holders to elect early taxation
- Allows founder to start capital gains tax clock at grant (vs. vesting)
- If not filed: Tax liability deferred until each vesting event

**Why file 83(b) (recommended for founders):**

**Scenario A: Without 83(b) Election**
- Grant date: Month 0 (shares worth $0.01/share)
- Cliff vests: Month 12 (shares worth $2.00/share)
- Tax event: Founder has ordinary income on 250,000 shares × $2.00 = $500,000 ordinary income
- Tax owed: ~$125,000 (25% federal + FICA + state)
- Ongoing: Each month vests = new tax event

**Scenario B: With 83(b) Election**
- Grant date: Month 0 (shares worth $0.01/share)
- 83(b) election filed: Within 30 days of grant
- Tax event: Founder has ordinary income on 10,000,000 shares × $0.01 = $100,000 ordinary income
- Tax owed: ~$25,000 (25% federal + FICA + state)
- Month 12+: All future vesting is capital gains (lower rate)
- At exit: Long-term gains rate applies to full appreciation

**Savings: $100,000+** (in this scenario)

**How to file 83(b):**
1. Prepare Form 83(b) (available from IRS or tax advisor)
2. File with IRS (by mail or e-file) within 30 days of grant
3. Include copy with personal tax return
4. Keep copy in company records

**Critical deadline: 30 days from grant date** (miss this = no benefit)

---

### Ordinary Income vs. Capital Gains

**Ordinary income (without 83(b)):**
- Taxed at your marginal rate (24–37% federal)
- Subject to self-employment tax (2.9% Medicare, 12.4% Social Security)
- Total effective rate: 35–50%

**Capital gains (with 83(b)):**
- Long-term capital gains rate: 15–20% federal (lower than ordinary income)
- No self-employment tax
- Total effective rate: 15–20%

**Savings from 83(b) election:**
```
Example: $500,000 ordinary income vs. capital gains

Ordinary income tax: $500,000 × 40% (est.) = $200,000
Capital gains tax: $500,000 × 18% (est.) = $90,000
Savings: $110,000
```

---

### Tax Planning: Vesting + Cash Flow

**Key consideration:** Vesting creates tax liability even if you haven't received cash.

**Example problem:**
- Founder vests 250,000 shares at Month 12 cliff
- Stock price: $2.00 (paper value: $500,000)
- Tax owed: ~$125,000 (depending on 83(b) election)
- Cash received: $0 (vested equity, no sale)
- **Result: Tax bill with no cash**

**Solutions:**

**Option 1: File 83(b) early (solves above)**
- Tax liability occurs at grant date (shares worth $0.01)
- Much smaller tax bill ($25,000 in this example)
- All future appreciation = capital gains (deferred until sale)

**Option 2: Plan for tax liquidity**
- Keep cash reserve for vesting tax events
- Budget: ~$3K–$5K per quarter for tax liability
- Important if 83(b) not filed

**Option 3: Cashless exercise / secondary sales**
- Some companies allow founder to sell vested shares to pay taxes
- Not recommended during early stage (dilutes founder stake)
- But available if needed

---

## Part 4: Why 1-Year Cliff Matters

### The Cliff Protection Rationale

**Without a cliff (linear vesting from day 1):**

```
Founder granted 1,000,000 shares
Monthly vesting: 1,000,000 ÷ 48 = 20,833 shares/month

Month 6 (founder quits): 
├─ Vested: 20,833 × 6 = 125,000 shares (12.5%)
├─ Unvested: 875,000 shares (87.5% forfeited)
└─ Issue: Founder still has 12.5% equity after 6 months

Month 11 (founder quits):
├─ Vested: 20,833 × 11 = 229,163 shares (22.9%)
└─ Issue: Founder has ~23% equity after 11 months
```

**With 1-year cliff (standard):**

```
Month 6 (founder quits):
├─ Cliff not yet triggered
├─ Vested: 0 shares (0%)
└─ Unvested: 1,000,000 shares forfeited (100%)
✓ Company retains 100% equity

Month 11 (founder quits):
├─ Cliff not yet triggered
├─ Vested: 0 shares (0%)
└─ Unvested: 1,000,000 shares forfeited (100%)
✓ Company retains 100% equity

Month 12 (founder stays, then quits):
├─ Cliff triggers: 250,000 vested
├─ Founder earned: 25% equity
└─ Company's position: Founder committed 1 year; 75% still protected
```

### Why Investors Demand Cliffs

**Investor perspective:**
- Early departures risk company (lose founder, lose direction)
- Cliff ensures founder has "skin in the game" for minimum 1 year
- If founder leaves pre-cliff: Investor knows founder wasn't committed
- If founder stays past cliff: Investor gains confidence in leadership

**Standard in venture:**
- 99%+ of VC-backed companies use 1-year cliff minimum
- Some use 6-month cliff (less common)
- Some use no cliff (rare, only for highly trusted scenarios)

### Cliff Consequences: Real Scenario

**Scenario: Co-founders with disagreement**

- Founder A and B both granted 5M shares, 4-year/1-year cliff
- Month 6: Serious conflict between founders
- Founder B wants to leave; Founder A wants to continue
- **Without cliff:** 
  - B gets ~500K shares (~5% equity) just for 6 months
  - Creates financial incentive to leave
  - A has to keep paying B despite departure
  
- **With cliff:**
  - B gets 0 shares for departure at month 6
  - No incentive to leave early
  - Forces negotiation: Either resolve (stay past cliff) or leave with nothing

**Cliff creates accountability.**

---

## Part 5: Acceleration Triggers

### Double-Trigger Acceleration (Standard)

**Double-trigger:** Two events must occur for acceleration.

**Most common: Change of Control + Termination**

```
Trigger 1: Change of Control (acquisition, merger, recapitalization)
Trigger 2: Termination without cause OR founder resignation

Result: Unvested shares accelerate to 100% (or partial acceleration)
```

**Example:**

```
Founder has 1M shares, 4-year/1-year cliff
At Month 24 (2 years): 500K vested, 500K unvested

Scenario A: Acquisition (no termination)
├─ Trigger 1: YES (change of control)
├─ Trigger 2: NO (founder stays / employment continues)
└─ Result: NO acceleration (double-trigger not met)

Scenario B: Acquisition + Founder termination
├─ Trigger 1: YES (change of control)
├─ Trigger 2: YES (founder terminated post-close)
└─ Result: 100% acceleration (all 1M shares fully vest)
```

**Why double-trigger?**
- Protects company: Doesn't reward departing founders who don't contribute to exit
- Protects founder: Ensures vesting continues if acquired and kept (no punishment)
- Balances incentives: Founder benefits from successful exit + staying through it

### Single-Trigger Acceleration (Less Common, But Founder-Friendly)

**Single-trigger:** One event causes acceleration.

```
Single trigger: Change of Control (acquisition, merger)

Result: Unvested shares accelerate to 100% automatically
```

**Founder perspective:**
- ✓ Protected if acquired and then laid off
- ✓ Share in full exit value regardless of post-acquisition employment
- ✗ Company loses leverage if acquisition terms change

**Investor perspective:**
- ✗ Founder gets full payout even if not retained
- ✗ Acquirer may not want founder; must pay full equity anyway
- ✓ Simpler structure

**Typical outcome:**
- Founders negotiate for single-trigger in exit (leverage increases)
- Investors push for double-trigger in funding rounds (risk mitigation)

---

### Partial Acceleration Scenarios

**Alternative: Tiered acceleration based on timing**

```
Acquisition in Year 1 (months 0–12):
├─ If founder fired pre-cliff: 0% acceleration
├─ If founder kept post-close: 25% acceleration (cliff vests)

Acquisition in Year 2 (months 13–24):
├─ If founder fired: 50% acceleration (cliff + 12 months)
├─ If founder kept: 50% + future vest at new company

Acquisition in Year 3+ (months 25+):
├─ If founder fired: 75%+ acceleration
├─ If founder kept: Full acceleration
```

---

## Part 6: Implementation & Documentation

### Step 1: Document Vesting Agreement

**Create a written vesting agreement (required):**

**What to include:**
- Grant date and number of shares
- Vesting schedule (4-year, 1-year cliff)
- Termination provisions (good/bad leaver)
- Acceleration triggers
- Tax treatment (83(b) election instructions)
- Board seat and governance rights

**Template structure:**

```
EQUITY VESTING AGREEMENT

This agreement is between:
SENTINEL LABS, INC. (Company)
[FOUNDER NAME] (Holder)

1. Grant Details
   - Grant Date: [Date]
   - Shares Granted: [Number]
   - Share Class: Common Stock
   - Vesting Schedule: 4-year vesting with 1-year cliff

2. Vesting Schedule
   - Cliff Date (Month 12): 25% vests
   - Monthly vesting (Month 13–48): 1/48 per month
   - Service requirement: Continuous employment

3. Termination Provisions
   - Termination without cause: Vesting through departure date
   - Termination for cause: Vesting stops; unvested forfeits
   - Voluntary resignation: Vesting stops; unvested forfeits

4. Change of Control
   - [Double-trigger / Single-trigger] acceleration applies
   - Definition of change of control: [...]

5. Tax Treatment
   - Holder should file IRS Form 83(b) within 30 days
   - Company will provide 83(b) instructions

[Signatures and board approval]
```

---

### Step 2: Board Approval & Capitalization Table Update

**Board action required:**

1. **Board resolution approving equity grant**
   - Founder name and share count
   - Vesting schedule terms
   - Any special provisions

2. **Update capitalization table immediately**
   - Add founder as shareholder
   - Show grant date and vesting schedule
   - Show vesting progress monthly

3. **File stock certificate**
   - Issue founder stock certificate or book entry
   - Record in company records
   - Provide founder with evidence of ownership

---

### Step 3: 83(b) Election Filing

**Within 30 days of grant date:**

1. **Prepare Form 83(b)** (IRS form + instructions)
   - Founder name and SSN
   - Company name and EIN
   - Stock description (common shares)
   - Grant date and FMV at grant
   - Vesting schedule

2. **File with IRS** (by certified mail or e-file)
   - Mail to IRS address per 83(b) instructions
   - Keep copy for tax records

3. **Provide to tax advisor**
   - Tax advisor should file with founder's tax return
   - Confirm filing with IRS

4. **Record in company**
   - Keep copy in founder's personnel file
   - Reference on cap table

**Timeline critical: Miss 30-day deadline = lose tax benefit**

---

### Step 4: Monthly Vesting Tracking

**Create vesting spreadsheet (company responsibility):**

| Founder Name | Grant Date | Total Shares | Monthly Rate | Month | Cumulative Vested | Cumulative Unvested | Vesting % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| [Name] | [Date] | 1,000,000 | 20,833 | 0 | 0 | 1,000,000 | 0% |
| [Name] | [Date] | 1,000,000 | 20,833 | 12 | 250,000 | 750,000 | 25% |
| [Name] | [Date] | 1,000,000 | 20,833 | 24 | 500,000 | 500,000 | 50% |
| [Name] | [Date] | 1,000,000 | 20,833 | 36 | 750,000 | 250,000 | 75% |
| [Name] | [Date] | 1,000,000 | 20,833 | 48 | 1,000,000 | 0 | 100% |

**Update monthly (or quarterly) to track:**
- Cumulative vested shares
- Remaining unvested
- Vesting percentage
- Flag for upcoming vesting milestones

---

### Step 5: Annual Cap Table Update

**Include in annual financial statements:**
- Current cap table showing all shareholders
- Vesting status of all restricted stock
- Any acceleration events
- Updated FMV of shares (for 409A valuation)

---

## Part 7: Departure Scenarios & Consequences

### Good Leaver vs. Bad Leaver

**Good Leaver** (termination without cause, medical leave, retirement):
- Vesting continues through departure date
- Or: Cliff vests; post-cliff shares continue vesting for 3–12 month tail
- Founder retains vested equity

**Bad Leaver** (termination for cause, breach of agreement, misconduct):
- Vesting stops immediately
- Unvested shares forfeit to company
- Pre-cliff departure: All shares forfeited

**Example scenarios:**

| Scenario | Status | Vesting Impact | Rationale |
| :--- | :--- | :--- | :--- |
| Founder works 4 years, retires | Good leaver | 100% vested | Earned full equity |
| Founder works 2 years, takes other job | Good leaver | 50% vested + tail | Earned half; company given notice |
| Founder embezzles, fired immediately | Bad leaver | 0% vested (forfeits all) | Misconduct; no reward |
| Founder violates NDA, fired | Bad leaver | Cliff only (25%) | Some punishment; cliff already earned |
| Founder quit Month 11 | N/A | 0% vested (no cliff) | Pre-cliff departure; no equity earned |

---

### Buyback Rights (Optional)

**Company may have right to repurchase unvested shares:**

```
Founder departures and forfeits 500K unvested shares.

Company buyback options:
1. Repurchase at original grant price ($0.01/share)
   - Company cost: $5,000
   - Shares return to treasury for re-grant

2. Repurchase at FMV ($5.00/share)
   - More founder-friendly
   - Company cost: $2.5M
   - Harder for company to afford

3. No buyback (shares forfeit)
   - Company regains shares by default
   - No cash required
```

**Best practice:**
- Reserve buyback right for company at original grant price
- Only exercise if shares have appreciated significantly
- Protects company's cap table

---

## Part 8: Vesting vs. Performance

### Key Distinction: Vesting ≠ Bonus

**Vesting is based on time (service), not performance.**

**Why?**
- Retention tool (stay longer = earn equity)
- Protects company from early departures
- Long-term incentive alignment

**Performance compensation is separate:**
- Annual bonuses (cash, tied to goals)
- Refresh grants (new equity, if founder exceeds targets)
- Options for team (separate pool)

**Scenario:**

```
Founder granted 1M shares at $0.01 (4-year/1-year cliff)
Company performs amazingly: Revenue $10M YoY, valuation $50M

Month 12: Cliff vests (25% = 250K shares)
├─ Reason: Time (service), not performance
├─ Value: 250K × $5.00 = $1.25M
└─ Earned: Yes, founder stayed 1 year

Company may also grant bonus:
├─ Annual bonus: $100K cash (performance-based)
├─ New equity grant: 200K shares (refresh) if extended
└─ These are separate from vesting schedule
```

**Key insight: Vesting is automatic; bonuses are discretionary.**

---

## Part 9: Founder Vesting Post-Fundraising

### How Vesting Changes After Investor Rounds

**Pre-fundraising (founder only):**
- Founder: 10M shares (100%)
- Vesting: 4-year/1-year cliff

**Post-Seed ($1M):**
- Dilution ~10%
- Founder: 9M shares (~90%)
- Investor: 1M shares (~10%)
- **Founder vesting:** Still 4-year/1-year cliff on original 9M shares
- **Investor:** Typically fully vested immediately (no cliff)

**Post-Series A ($5M):**
- Additional dilution ~20%
- Founder: ~7.2M shares (~72%)
- Seed investor: 1M shares (still ~10%)
- Series A investor: 1.8M shares (~18%)
- **Founder vesting:** Continues on original schedule (no change due to Series A)
- **New investors:** Fully vested on their shares

**Key rule: Founder vesting does NOT reset with new fundraising**
- Same 4-year clock
- Same monthly accrual
- Company can't restart vesting due to dilution

---

### Refreshment Grants (Optional, Post-Fundraising)

**Company may grant new equity (separate from original vesting):**

```
Original grant (Month 0): 10M shares, 4-year cliff
├─ Month 12: 2.5M vests
├─ Month 24: 2.5M vests (5M total)
├─ Month 36: 2.5M vests (7.5M total)

Refreshment grant (Month 24, after Series A): 1M new shares, 3-year cliff
├─ Reason: New company valuation, retention, performance
├─ Vests: 1M ÷ 36 = 27.8K/month over 3 years
├─ Timeline: Separate 3-year clock
├─ Result: Founder now has both schedules vesting in parallel
```

**Why refreshment grants?**
- Retains founder (new long-term lock-in)
- Recognizes company growth (new equity at higher valuation)
- Incentivizes hitting next milestone (Series B, etc.)

---

## Part 10: Special Cases & Exceptions

### Accelerated Cliff (Early Cliff Trigger)

**Non-standard: Company accelerates cliff for exceptional circumstances**

```
Example: Founder diagnosed with medical emergency, forced medical leave

Standard: Cliff still at Month 12
├─ If founder unable to return by Month 12, equity forfeits
└─ Problem: Unfair to founder with medical hardship

Accelerated cliff: Company moves cliff forward to Month 6
├─ Founder gets 25% equity vested early
├─ Recognition: Company acknowledges founder's contribution
└─ Founder gets partial protection if can't return
```

**Legal consideration:**
- Requires board approval
- Should be documented formally
- May have tax implications

---

### Partial Cliff (Less Common)

**Non-standard: Cliff doesn't vest all at once**

```
Standard: 4-year/1-year cliff = 25% at Month 12

Partial cliff: 4-year vesting with 6-month milestone
├─ Month 6: 10% vests (not cliff)
├─ Month 12: Additional 15% vests (50% cumulative)
├─ Months 13–48: Remaining 50% vests monthly
└─ Effect: Less sharp cliff, smoother vesting
```

**Pros:**
- More founder-friendly (equity sooner)
- Recognizes 6-month contribution

**Cons:**
- Weaker retention (less loss if founder quits at Month 11)
- Investor disfavors (less company protection)

**Typical:** Used only for very early hires or co-founders with existing relationships

---

### Vesting Pool for Team (Separate)

**Important distinction: Founder vesting vs. employee pool**

```
After founder equity vesting is set:
├─ Founder: 8M shares (80% fully diluted)
├─ Employee option pool: 2M shares (20%)
│  ├─ Used to hire employees
│  ├─ Standard 4-year/1-year cliff
│  ├─ Company controls issuance
│  └─ Investor approved in funding rounds
└─ Note: Employee pool is separate from founder's vesting
```

**Why separate?**
- Founder vesting is locked in at grant
- Employee option pool is controlled by company/board
- Company can adjust employee grants without affecting founder

---

## Part 11: Exit Scenarios & Vesting Consequences

### Acquisition (Most Common Exit)

**Scenario: Acquisition at Month 30 (2.5 years in)**

**Founder vesting at time of acquisition:**
- Total granted: 1M shares
- Vested at Month 30: 625K shares (62.5%)
- Unvested: 375K shares (37.5%)

**Acquisition terms (assuming double-trigger acceleration):**

| Scenario | Vesting | Buyer Behavior | Founder Outcome |
| :--- | :--- | :--- | :--- |
| **Founder retained** | 100% accelerates | Buyer keeps founder 1+ year | Founder gets full 1M value + employment |
| **Founder not retained** | 100% accelerates | Buyer doesn't need founder | Founder gets full 1M value + severance |
| **Founder offered reduced role** | 100% accelerates | Buyer wants founder in limited capacity | Founder negotiates between full/partial acceleration |

**Tax consequence:**
- Acquisition triggers liquidity event
- Founder pays capital gains on appreciation
- Vested shares: Long-term capital gains (if 83(b) filed)
- Previously unvested shares: Ordinary income (if accelerated without 83(b))

---

### IPO (Rare but Possible)

**Scenario: IPO at Month 48 (4 years, full vesting)**

**Founder vesting at IPO:**
- Total granted: 1M shares
- Vested: 1M shares (100%)
- Unvested: 0 shares

**IPO process:**
- Lockup period: 180 days (founder cannot sell immediately)
- Founder remains employed (no acceleration needed)
- Post-lockup: Founder can sell vested shares
- All shares fully vested = no ongoing vesting schedule

**Tax consequence:**
- Public company shares: No section 83(b) benefit (already fully vested)
- Founder pays capital gains on sale (long-term rate)
- Potential AMT (Alternative Minimum Tax) if vested early without 83(b)

---

### Down Round or Restart

**Scenario: Company resets valuation (down round)**

```
Founder granted 1M shares at $0.01 (Month 0)
Months 1–12: Company valued at $10M (valuation increasing)
Month 12: Cliff vests (250K shares worth $500K at $2.00/share)
Month 13–24: Company valued at $2M (major setback)
```

**Vesting continues unchanged:**
- ✓ Same 4-year/1-year schedule applies
- ✓ Vesting doesn't restart or adjust
- ✗ Founder's equity value has dropped

**No adjustment for down round** (fair but harsh)

**Founder protections (if negotiated):**
- Refresh grant at lower valuation (new equity issued)
- Acceleration of some unvested shares (morale boost)
- Extended runway (founder knows harder path)

---

## Part 12: Cap Table Integration

### Cap Table Format (Including Vesting)

**Example cap table for Sentinel Labs:**

| Holder | Share Class | Shares | % Fully Diluted | Grant Date | Vesting Schedule | Vested % | Vested Shares |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Founder A | Common | 4,000,000 | 40% | 2025-01-01 | 4yr/1yr cliff | 50% | 2,000,000 |
| Founder B | Common | 4,000,000 | 40% | 2025-01-01 | 4yr/1yr cliff | 50% | 2,000,000 |
| SAFE Investor | SAFE | — | — | 2025-06-01 | Upon conversion | — | — |
| Employee Option Pool | Options | 2,000,000 | 20% | 2025-ongoing | 4yr/1yr cliff | Varies | Varies |
| **TOTAL** | — | **10,000,000** | **100%** | — | — | **50%** | **4,000,000** |

**Key metrics:**
- **Fully diluted:** All shares including options and SAFEs
- **Vested percentage:** Current vesting progress (50% = 2 years in)
- **Vested shares:** Shares actually owned (not subject to forfeiture)
- **Unvested:** Subject to termination provisions

---

## Part 13: Vesting Agreement Checklist

**Before signing vesting agreement, verify:**

- [ ] Grant date is specified clearly
- [ ] Total share count is accurate
- [ ] Vesting schedule: 4-year/1-year cliff confirmed
- [ ] Termination provisions for good/bad leaver
- [ ] Acceleration triggers (change of control)
- [ ] 83(b) election instructions provided
- [ ] Board has approved the grant
- [ ] Stock certificate or book entry provided
- [ ] Founder has copy of agreement
- [ ] All signatures are present (founder, founder's spouse if required, company officer, board)

---

## Part 14: Founder Responsibilities During Vesting

### Service Requirement (Critical)

**Vesting depends on "continued service":**

**What counts as continued service:**
- ✓ Working at company (full-time, part-time)
- ✓ On approved leave (medical, sabbatical)
- ✓ Board service (if founder is director)
- ✗ Termination for any reason (vesting stops)

**Founder should:**
- [ ] Maintain active employment status
- [ ] Fulfill role responsibilities
- [ ] Avoid actions that trigger "for cause" termination
- [ ] Communicate with company if taking leave

---

### Tax Obligations During Vesting

**Founder should:**
- [ ] File 83(b) election within 30 days (with tax advisor)
- [ ] Pay any upfront tax owed
- [ ] Set aside estimated taxes for ongoing vesting (if 83(b) not filed)
- [ ] Consult CPA about tax planning
- [ ] Report vesting events on annual tax return

**Key dates:**
- Month 0: File 83(b) within 30 days
- Month 12: First tax liability possible (cliff vesting)
- Quarterly: Estimate taxes
- April 15: File tax return showing any 83(b) or vesting events

---

### Cap Table Monitoring

**Founder should request:**
- [ ] Updated cap table quarterly
- [ ] Confirmation of vesting status
- [ ] Any option pool changes
- [ ] Dilution from new fundraising (keep cap table current)

---

## FAQ: Founder Vesting

**Q: What if I leave before the 1-year cliff?**
A: You forfeit 100% of equity. The cliff ensures you must stay 1 year to earn any equity. This is standard and non-negotiable with investors.

**Q: Can I negotiate to remove the cliff?**
A: Unlikely. Cliffs are investor-standard. But you can negotiate the cliff duration (6 months vs. 12 months) or acceleration triggers.

**Q: What does "continued service" mean?**
A: You must remain employed by the company. Approved leave (medical, maternity, sabbatical) may count; quitting or being fired stops vesting.

**Q: Do I have to file 83(b)?**
A: No, but you should. Without it, vesting creates ordinary income tax events. With it, you pay once at grant and then capital gains on appreciation. Highly recommended.

**Q: What if I'm terminated without cause?**
A: Standard terms: Vesting stops, but you keep vested equity. Some companies give you a 30-day tail to exercise vested options. Confirm your agreement.

**Q: What if the company is acquired?**
A: Depends on your vesting agreement. With double-trigger acceleration: If you're terminated post-acquisition, all remaining equity vests. Without double-trigger: You keep what you had vested; unvested forfeits.

**Q: Can the company take back my vested shares?**
A: No. Once vested, shares are yours. Unvested shares can be forfeited if you leave or are fired for cause.

**Q: What if the company does a down round?**
A: Your vesting schedule doesn't change, but your equity value may drop. No protection unless you negotiated a refresh grant.

**Q: Do I pay taxes on the cliff vesting day?**
A: If you filed 83(b): No additional tax (you already paid at grant). If you didn't file 83(b): Yes, you owe ordinary income tax on vested shares' appreciation.

**Q: Can I sell my vested shares?**
A: Depends on company stage and agreements. Pre-IPO: Unlikely (no market, may have transfer restrictions). Post-IPO: Yes, subject to lockup period.

**Q: What happens if I get promoted?**
A: Your original vesting schedule doesn't change, but company may grant additional equity (refresh grant) recognizing your new role.

---

## Status: Ready for Founder Approval

This vesting framework is complete and ready for implementation.

**Next steps (upon approval):**
1. Founder reviews and approves 4-year/1-year cliff structure
2. Finance team prepares vesting agreement
3. Board approves equity grant
4. Founder files 83(b) election within 30 days
5. Finance team tracks vesting monthly
6. Annual cap table updates

---

**Document Owner:** Finance Department / Founder  
**Last Updated:** 2025-11-23  
**Classification:** Internal Finance  
**Status:** Active — Ready for Implementation
