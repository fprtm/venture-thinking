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

## The four questions engineers skip

Building is not the bar. Ask:

1. **Should we build it?** (not just *can* we)
2. **Will people pay for it?**
3. **Can we acquire them profitably?** (CAC < LTV)
4. **Can this become meaningfully large?**
