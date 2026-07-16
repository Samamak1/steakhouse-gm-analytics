# Beverage-Led Profitability: A GM Business Case

**An upscale steakhouse inside a major casino property - July 2024**

Written while pursuing the General Manager position, from the floor, on the property's
June-2024 statements. All confidential figures are replaced with `$-` placeholders or
**clearly-labeled illustrative numbers**; the models and program designs are reproduced
as built.

---

## Part 1 - The financial models

### Model 1: Average alcohol profit margin

For each beverage category (wine, beer, liquor), profit margin from the P&L:

```
margin_category = (revenue_category − COS_category) / revenue_category
```

then the program-level view:

```
avg_margin = (margin_wine + margin_beer + margin_liquor) / 3
```

Finding (direction, not figures): all three categories ran high-margin - liquor highest,
wine lowest but still far above food margin. The blended average made the strategic point
on one line: **beverage dollars are worth several food dollars in profit terms.**

### Model 2: Beverage share of revenue

Each category's contribution to total revenue:

```
share_category = revenue_category / revenue_total
share_beverage = (rev_liquor + rev_wine + rev_beer) / revenue_total
```

Finding: total beverage share sat in the mid-teens as a percentage of revenue -
materially below the 25-30% typical of high-performing full-service steakhouses. Wine
and liquor were near-equal contributors; beer was minor. That gap *is* the opportunity.

### Model 3: Average guest spend, two ways

**From actuals:**

```
avg_guest_spend = net_revenue / MTD_covers
```

**From the menu (basket build-up):** assume a typical order - one appetizer, one entree,
one side, one beverage - and price the basket from the menu:

```
avg_spend_menu = p_appetizer + p_entree + p_side + p_beverage
```

Running both exposes the gap between what the menu *invites* a guest to spend and what
guests *actually* spend - and located the shortfall in the beverage line item, not food.

### Model 4: One more glass of wine per guest

The core of the case. Because fixed costs (payroll, occupancy, operating expenses) do not
move with one incremental pour, the marginal profit of an extra glass is the glass price
minus pour cost - nothing else.

Variables:

- `n` = monthly covers
- `p` = average by-the-glass wine price
- `c` = beverage pour-cost ratio (COS_beverage / revenue_beverage)

```
incremental_revenue = n × p
incremental_cost    = n × p × c
marginal_profit     = n × p × (1 − c)
```

**Illustrative example (not actual figures):** at n = 3,000 covers, p = $15, and c = 20%:

```
3,000 × $15 = $45,000 incremental revenue
$45,000 × 0.20 = $9,000 incremental cost
$45,000 × 0.80 = $36,000 added monthly profit
```

One glass per guest, at steakhouse pour costs, is a six-figure annual profit swing - with
zero new fixed cost. Even fractional attach rates (one extra glass per *three* guests)
clear most monthly P&L gaps.

The companion scenario modeled a **beverage-share target** instead of a per-glass attach:

```
rev_beverage_target = s × revenue_total          (e.g., s = 30%)
revenue_new   = rev_food + rev_beverage_target
COS_bev_new   = rev_beverage_target × c
profit_new    = revenue_new − (COS_food + COS_bev_new) − OpEx_total
```

Holding food flat and lifting beverage to the target share flipped the month from a loss
to a profit in the modeled P&L - the same conclusion as the per-glass model, stated in
the language of a revenue mix target.

### Model 5: Comp-adjusted profitability

Casino steakhouses comp heavily, and comps distort the P&L. To see the true cash
economics, strip comped food revenue and the costs that ride on it. With `k` = comp share
of food revenue:

```
rev_cash        = rev_food_cash + rev_beverage
COS_food_cash   = COS_food × (1 − k)             (COS assumed proportional to volume)
OpEx_variable'  = OpEx_variable × (1 − k)        (variable expenses scale with volume served)
profit_cash     = rev_cash − (COS_food_cash + COS_bev + payroll + OpEx_variable')
```

Finding (direction): on a cash-only lens the operation ran meaningfully negative - the
house was effectively financing food comps at food margins. Beverage sales, which were
almost entirely cash revenue at high margin, were the natural counterweight. This
reframed the beverage push from "nice upside" to "the P&L repair mechanism."

---

## Part 2 - The wine program

A redesigned wine menu proposal, built to make the extra glass easy to sell. Every wine
carries a fixed four-field format that doubles as server training material:

- **Taste profile** - plain-language flavor description
- **Pairing** - named dishes from the actual menu
- **Price** - by the glass and by the bottle
- **Why** - one sentence a server can say verbatim at the table

Example entry (proposal, format as written):

> **Veuve Clicquot Brut Yellow Label** - Crisp and full-bodied with flavors of ripe
> apple, honey, and brioche. *Pairing:* Raw Bar Sampler, Jumbo Lump Crab Cake, Seared
> Scallops. *Price:* $- glass / $- bottle. *Why:* the crisp acidity and effervescence cut
> through the richness of seafood.

Categories: Sparkling, White, Rosé, Red, Reserve - with by-the-glass tiers from an
accessible entry point to prestige pours, so the upsell has a ladder rather than a leap.

---

## Part 3 - The training programs

Analysis identifies the profit; the floor staff captures it. Two programs, both my
authorship, were designed to execute.

### Server Training Certification Program (wine-focused)

Structure: six segments, each with educational content, a written test, and a role-play
or verbal test to a manager - followed by a final comprehensive test.

1. **Understanding the wine menu** - categories, the four-field icon format, and how to
   use it at the table
2. **Sparkling wines** - taste profiles, pairings, and the "why" for each pour
3. **White wines**
4. **Rosé wines**
5. **Red wines**
6. **Reserve wines**

Then a **final comprehensive test** across all segments.

Incentive design (per the program document): a gift-card bonus for passing each segment,
a larger bonus for the final test, a formal certificate of completion, and the server's
name on a "Certified Wine Experts" board in the restaurant - paying servers to become
the sales force the wine model requires.

### 4-Week Training Program for Hosts

The host stand controls seating flow, which controls server capacity to sell.

- **Week 1 - Introduction and basics:** restaurant operations; Host 1/2/3 role
  definitions for both 2-host and 3-host shifts; greeting scripts and
  reservation/walk-in handling with role-play.
- **Week 2 - Advanced service:** managing difficult situations (waits, double-books)
  with scripted recovery language; personalized guest interaction for regulars.
- **Week 3 - Fair rotation and strategic seating:** balancing head counts and table
  counts per server; handling call-in parties and specific-server requests without
  breaking rotation.
- **Week 4 - Efficiency and communication:** wait-time quoting, kitchen/server/guest
  communication, proactive service, then observation and mentorship with an experienced
  host, feedback, and sign-off.

Every module pairs **training verbiage** (exact scripts) with **role-playing exercises** -
the same pattern as the server program: define the standard, script it, rehearse it,
test it, reward it.

---

## What this demonstrates

- P&L literacy: category margins, cost-of-sales ratios, comp accounting, marginal
  analysis
- Translation of financial analysis into operational programs with incentive design
- The operator's habit of building the *whole* chain: number → menu → script → training →
  certification → payoff
