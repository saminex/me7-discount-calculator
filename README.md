# ME7 Discount Calculator

A browser-based tool for determining maximum discount percentages on Microsoft 365 E7 (ME7) ramp deals based on Field Empowerment (FE) guidelines.

**🔗 Live Tool:** [saminex.github.io/me7-discount-calculator](https://saminex.github.io/me7-discount-calculator/)

---

## What It Does

- Calculates FE-allowed discounts (Max / Average / Exit) based on SKU and coverage tier
- Compares current customer spend against ME7 list price ($99/user/mo) to determine revenue-neutral discount
- Generates a ramp schedule mapped to enrollment years with editable per-year discounts
- Validates ramp structure against FE caps (weighted average, exit year limits)
- Identifies when Deal Desk (DD) approval is needed and shows the DD ask

## How to Use

### Section 1 — Current Customer Profile

1. **Total M365 Workforce Seats** — Enter the customer's total M365 seat count
2. **Base Licenses** — Enter ME3 and/or ME5 quantities with weighted average $/user/mo
3. **Displacement Licenses** — Enter any Copilot, Entra Suite, or Agent 365 add-ons (qty + price)

### Section 2 — ME7 Discount Threshold

1. **SKU** — Select the ME7 licensing path:
   - *ME7 Full Suite* — New full licenses
   - *ME5 to ME7 Step Up* — Upgrading from ME5
   - *ME3 to ME7 Step Up* — Upgrading from ME3
   - *Entra + A365 Add-On* — Requires lead status, E5, and Copilot
   - *ME3 to ME5 Step Up* — Upgrading from ME3 to ME5
2. **Seats** — Enter the number of ME7 seats (field changes based on SKU selected)
3. **Deal Term** — Enter months (12–60). Defaults to 36.
4. Click **Calculate Discounts**

### Reading the Results

- **Side-by-Side Comparison** — Current spend vs. ME7 at list price
- **Revenue-Neutral Analysis** — The discount needed to match current spend, with FE guidance:
  - 🟢 *Within FE* — Full ramp available
  - 🟡 *Ramp Structuring Needed* — Within FE max, but needs careful ramp design
  - 🔴 *Exceeds FE* — Deal Desk approval required (DD ask details shown)
- **Ramp Schedule** — Editable per-year discounts with real-time weighted average validation
- **Enrollment Extension Guidance** — Rules for mid-term extensions (if applicable)

## Key Rules (Table 2)

| SKU | Coverage | Max | Avg | Exit |
|-----|----------|-----|-----|------|
| ME7 Full Suite | 50% or 80% | 50% | 40% | 30% |
| ME5 → ME7 Step Up | 80% | 73% | 60% | 40% |
| ME3 → ME7 Step Up | 80% | 65% | 53% | 38% |
| Entra + A365 Add-On | 80% | 73% | 60% | 40% |
| ME3 → ME5 Step Up | 80% | 50% | 40% | 30% |

- Deals > 36 months: −5pts off exit discount for Year 4/5
- Coverage = ME7 seats ÷ total M365 seats

## No Installation Required

Open the link in any browser. All calculations run client-side — no data is sent anywhere.
