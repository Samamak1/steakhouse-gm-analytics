# Casino Steakhouse Beverage Profitability Program

> A sanitized GM business case translating beverage P&L analysis into menu strategy, server certification, host training, and operating controls for an upscale steakhouse inside a casino property.

This repository preserves the method and program design without publishing the employer's confidential financial statements or presenting illustrative scenarios as achieved results.

## Program brief

| Field | Detail |
|---|---|
| Business challenge | A high-cost steakhouse operation needed a credible path from operating loss toward profitability without relying on additional fixed-cost capacity. |
| My role | Operating leader and General Manager candidate; author of the business case and associated menu and training program designs. |
| Mandate | Independently diagnose the profitability gap and translate the analysis into actions the floor team could execute. |
| Source period | June 2024 operating statements; analysis and program materials written in July 2024. |
| Stakeholders considered | Property leadership, finance, culinary, beverage, servers, hosts, and restaurant managers. |
| Status | Completed business case and program design. This repository does not claim executive approval, implementation, or realized financial impact from the proposal. |

## Business argument

The case followed one chain of reasoning:

1. Compare food and beverage economics at the category level.
2. Determine whether the operation's revenue mix was leaving high-margin beverage opportunity uncaptured.
3. Model the incremental economics of improving wine attachment and beverage share.
4. Test a comp-adjusted scenario under explicit assumptions.
5. Translate the financial opportunity into a menu, sales language, training, certification, incentives, and manager reinforcement.

The point was not a spreadsheet alone. It was to connect financial diagnosis to repeatable frontline behavior.

## Financial models

All figures from the original P&L remain private. Formulas below preserve the analytical method. Any displayed numeric scenario is illustrative.

### 1. Category and weighted beverage margin

For each beverage category:

```text
margin_category = (revenue_category - COS_category) / revenue_category
```

For a true revenue-weighted program margin:

```text
margin_beverage =
  (revenue_wine + revenue_beer + revenue_liquor
   - COS_wine - COS_beer - COS_liquor)
  / (revenue_wine + revenue_beer + revenue_liquor)
```

The category comparison identified beverage as materially higher margin than food, with liquor strongest and wine lower than liquor but still strategically valuable.

### 2. Beverage share of revenue

```text
share_category = revenue_category / revenue_total
share_beverage = (revenue_liquor + revenue_wine + revenue_beer) / revenue_total
```

The original case compared the operation's mix with a working full-service steakhouse benchmark. That benchmark should be treated as a planning assumption unless a supporting industry source is added.

### 3. Average guest spend, two views

From operating actuals:

```text
average_guest_spend = net_revenue / MTD_covers
```

From a menu basket:

```text
menu_basket = appetizer + entree + side + beverage
```

Comparing the two views located the largest opportunity in beverage attachment rather than food pricing alone.

### 4. One additional glass of wine per guest

Variables:

- `n` = monthly covers
- `p` = average by-the-glass price
- `c` = beverage pour-cost ratio

```text
incremental_revenue = n * p
incremental_cost    = n * p * c
marginal_profit     = n * p * (1 - c)
```

Illustrative example only:

```text
n = 3,000 covers
p = $15 per glass
c = 20% pour cost

incremental revenue = $45,000
incremental cost    = $9,000
marginal profit     = $36,000 per month
```

This is a scenario, not a reported operating result. Fractional attachment can be modeled by multiplying `n` by the assumed attach rate.

The companion revenue-mix scenario was:

```text
revenue_beverage_target = target_share * revenue_total
revenue_new             = revenue_food + revenue_beverage_target
COS_beverage_new        = revenue_beverage_target * beverage_COS_ratio
profit_new              = revenue_new - COS_food - COS_beverage_new - operating_expense
```

### 5. Comp-adjusted scenario

Casino comps can obscure the relationship between cash revenue and the cost of service. The case therefore tested a scenario in which comped food revenue and selected proportional costs were separated from cash activity.

With `k` as the assumed comp share of food revenue:

```text
revenue_cash         = revenue_food_cash + revenue_beverage
COS_food_cash        = COS_food * (1 - k)
variable_expense_adj = variable_expense * (1 - k)
profit_cash_scenario = revenue_cash - COS_food_cash - COS_beverage
                       - payroll - variable_expense_adj
```

This is an analytical lens under stated proportional-cost assumptions, not a statement of audited cash profitability.

## Operational program design

### Pairing-led wine menu

Each wine followed a four-field sales and training format:

- Plain-language taste profile
- Named pairing from the operating menu
- By-the-glass and bottle price
- A concise reason a server could use at the table

The proposed categories were Sparkling, White, Rose, Red, and Reserve, with price tiers designed as an upsell ladder rather than a single jump.

One original proposal entry used this structure:

> **Veuve Clicquot Brut Yellow Label** - Crisp and full-bodied, with ripe apple, honey, and brioche. **Pairing:** Raw Bar Sampler, Jumbo Lump Crab Cake, and Seared Scallops. **Price:** `$-` by the glass / `$-` by the bottle. **Why:** the acidity and effervescence cut through the richness of seafood.

Prices remain withheld. The example is preserved to show how product knowledge, menu engineering, and server language were connected.

### Server training and certification

The six-segment program covered:

1. Wine-menu navigation and sales language
2. Sparkling wines
3. White wines
4. Rose wines
5. Red wines
6. Reserve wines

Each segment paired educational content with a written test and role-play or verbal assessment. A final comprehensive assessment, recognition, certificate, and proposed incentives completed the certification loop.

### Four-week host program

- **Week 1:** role definitions, greetings, reservations, walk-ins, and role-play
- **Week 2:** wait management, service recovery, and personalized interaction
- **Week 3:** fair rotation, table and head-count balancing, call-in parties, and server requests
- **Week 4:** wait-time quoting, cross-team communication, observation, mentorship, feedback, and sign-off

The common mechanism was: define the standard -> script it -> rehearse it -> assess it -> reinforce it.

## Evidence and outcome status

| Item | Evidence status |
|---|---|
| Five analytical models | Sanitized reconstruction of the original method; confidential source values withheld. |
| Wine-menu proposal | Original program design summarized without confidential prices. |
| Server certification | Original program structure summarized; employee records are not included. |
| Host training | Original four-week program structure summarized. |
| Financial upside | Illustrative scenario only; not an achieved result. |
| Approval or implementation | Not claimed by this repository. |

## Repository contents

| File | Contents |
|---|---|
| `README.md` | Recruiter-facing program overview, analytical method, evidence status, and limitations. |
| `CASE-STUDY.md` | Detailed sanitized business case and program design. |

## Role, contributors, and authorship

Sama Mushtaq authored the analytical approach, business case, wine-menu proposal, server certification structure, and host training program. Property leadership, finance, culinary, beverage, servers, and hosts were stakeholders considered in the operating design; this repository does not attribute their employer-owned work to Sama.

The underlying financial statements belong to the employer and are not reproduced.

## AI assistance

The public record does not establish the scope of AI assistance, if any, in the original 2024 work. This replacement therefore makes no unsupported claim. Any AI used later for formatting, editing, or sanitizing the public presentation should be disclosed before publication; it did not originate confidential source data or operating outcomes.

## Confidentiality and provenance

- No source P&L, employee evidence, incident record, guest record, or employer-confidential document is included.
- Actual revenue, cost, margin, and cover figures are replaced with placeholders or omitted.
- Illustrative figures are labeled as such.
- Employer identity is not treated as anonymized if it is identified elsewhere in the public portfolio.

## Limitations

- This is a retrospective, sanitized case study, not an audited financial model.
- The working benchmark requires a source before it should be presented as an industry standard.
- The comp-adjusted view depends on proportional-cost assumptions.
- The repository demonstrates diagnosis and program design; it does not prove approval, adoption, or realized financial impact.

## Related

- [Hard Rock operational transformation case](https://samamak1.github.io/work/hard-rock/)
- [Sama Mushtaq program leadership portfolio](https://samamak1.github.io/)
