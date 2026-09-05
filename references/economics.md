# Quick unit economics

Not a 50-page financial model — the back-of-envelope check that turns an idea into a *business model*. Run it as soon as there is a price in mind.

## The five numbers

- **Price** — what one customer pays (per month, if recurring).
- **Cost to serve** — variable cost of serving one customer.
- **Gross margin** — Price − Cost to serve. The room you have to run the business.
- **CAC** — customer acquisition cost: what it costs to win one customer.
- **Retention / LTV** — how many months they stay × gross margin = lifetime value.

## The check

```
Price:            Rp1.000.000 / mo
Cost to serve:    Rp  200.000 / mo
Gross profit:     Rp  800.000 / mo   (80% margin)
CAC:              Rp1.500.000
Payback:          ~1.9 months of gross profit to recover CAC
LTV (12 mo):      Rp9.600.000  →  LTV:CAC ≈ 6.4:1
```

Rules of thumb: **LTV:CAC ≥ 3:1** is healthy; **CAC payback < 12 months** for most SMB SaaS. If the math only works at scale you do not have yet, that assumption belongs in the ASSUME stage as a risk.

## Customer economics — price against value created, not feature count

Before pricing, estimate the **current cost of the pain** to the customer:

```
Cost of pain ≈ (people involved × hours spent × loaded hourly cost)
             + error cost + delay/opportunity cost
             + existing software/contractor cost
             + compliance/regulatory risk cost
             + revenue leakage
```

Then estimate plausible **solution value** as the portion of that cost the solution actually removes — not the full cost of pain, since most solutions don't eliminate 100% of it. Price by **capturing a fraction of value created**, not by counting features:

> If the problem costs the company ~$100,000/yr and the solution eliminates ~$60,000 of it, pricing at $10k–$20k/yr is easier to justify to the buyer than a price built up from a feature checklist — it's visibly a good trade against their own numbers.

Use ranges, not false precision, and label the estimate as such (see [`red-team.md`](red-team.md) evidence classification) — don't fabricate a customer's internal numbers you haven't actually seen.

## The four questions engineers skip

Building is not the bar. Ask:

1. **Should we build it?** (not just *can* we)
2. **Will people pay for it?**
3. **Can we acquire them profitably?** (CAC < LTV)
4. **Can this become meaningfully large?**
