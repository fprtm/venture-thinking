# RED TEAM — attacking the hypothesis before the market gets to

Run this after ASSUME has named the riskiest assumption, before sinking real effort into TEST. The goal is to find the strongest reasons this fails *before* spending a test on it — not to talk yourself out of everything, and not to rubber-stamp what's already exciting you. Never become attached to a hypothesis mid-analysis: the moment something feels exciting, that is the signal to stop and run this, not skip it.

## Evidence classification — label every important claim

Do not let a claim's plausibility stand in for its evidence. Classify each material claim as one of:

- **VERIFIED FACT** — directly confirmed (a price actually listed, a quote actually posted).
- **STRONG EVIDENCE** — multiple independent, consistent signals.
- **WEAK SIGNAL** — one anecdote, or evidence that could point multiple ways.
- **INFERENCE** — a reasonable conclusion drawn from other facts, not observed directly.
- **SPECULATION** — a plausible guess with no supporting signal yet.
- **UNKNOWN** — genuinely don't know; say so rather than filling the gap with a guess dressed as a fact.

Never invent statistics, quotes, market size, prices, review data, revenue, features, or behavior. If estimating, label it **ESTIMATE** and give a range, not false precision. If evidence conflicts, show the conflict rather than picking the version that supports the thesis.

### Evidence strength ladder (for ranking how solid a pain claim is)

- **Level 0** — pure speculation.
- **Level 1** — a single anecdote.
- **Level 2** — multiple independent complaints.
- **Level 3** — repeated documented patterns across communities.
- **Level 4** — people actively build workarounds or hire labor to cope with it.
- **Level 5** — companies already spend meaningful money trying to solve it.

Prioritize Level 4–5 findings; treat Level 0–2 as "worth investigating further," not "validated."

### Fake signals vs. strong validation signals

Flag explicitly when a finding is one of these **fake/weak signals**, even though it feels like traction: people liking an idea, social-media hype or upvotes without buying behavior, "large TAM" with no identifiable reachable customer, waitlist signups, free users, survey answers of "I'd use this," generic AI enthusiasm, a competitor raising funding, a search-trend spike, vanity metrics.

Prefer these **strong signals**: a customer pays, a customer prepays, a customer signs a real commitment (LOI), a customer shares internal data, a customer introduces you to the actual decision-maker, a customer invests real employee time in onboarding, a customer follows up unprompted asking when it'll be ready, multiple customers independently describe the identical problem unprompted, customers currently spend money on an inferior solution, a customer is willing to replace an existing workflow for this.

## Follow the money

For every opportunity, name explicitly (mark UNKNOWN where genuinely unclear, don't guess):

- **Economic buyer** — who can actually approve the spend?
- **User** — who experiences the problem day to day (often not the same person as the buyer)?
- **Champion** — who inside the organization would advocate for this?
- **Blocker** — who could kill or stall adoption (IT/security/procurement/an entrenched incumbent relationship)?
- **Budget** — where would the money actually come from (an existing line item, a new one, a personal card)?
- **Buying trigger** — what event makes this urgent *now* (hiring spike, new regulation, audit, growth, a customer complaint, a security incident, a migration, new management, a lost contract, an operational failure, an acquisition)?

**If you cannot name a realistic budget owner, aggressively downgrade the opportunity** — a real, felt problem with no identifiable buyer is not yet a business.

## Ladder the pain to its real consequence

For every pain found, keep asking "why does that matter?" until it terminates in an economic, operational, regulatory, reputational, or strategic consequence — the surface complaint is rarely the sellable pain.

> "Manual invoice entry is annoying" → consumes 30 employee-hours/week → creates errors → errors delay reconciliation → delayed reconciliation delays month-end close → finance works overtime → management gets late numbers → **decisions get made on stale financial data.**

The deepest consequence found is usually the one worth quoting back to the buyer — sell the removal of *that*, not the surface annoyance.

## Pain quality vs. business quality — score separately

A problem can be real and still be a bad business; don't let a severe pain paper over a broken business model, or a great business model excuse a weak pain. Evaluate both:

- **Pain quality:** severity, frequency, urgency, economic consequence, emotional frustration, existence of a current workaround.
- **Business quality:** willingness to pay, reachable buyer, sales-cycle length, market fragmentation vs. concentration, incumbent strength, switching cost, solution complexity, support burden, regulatory burden, gross-margin potential, recurring-revenue potential, retention potential, expansion potential.

## The red-team attack

Once a hypothesis exists, argue against it as a skeptical investor actively trying to kill it — generate the *strongest* objections, not straw men:

What if the pain isn't as severe as it looks? What if people complain but won't actually pay? What if the current workaround is "good enough" to keep? What if an incumbent can ship this as a feature overnight? What if implementation is painful for the customer? What if CAC exceeds LTV? What if the buyer and the user are different people with different incentives? What if security/compliance blocks adoption? What if data access is the real blocker? What if integrations are too fragmented to be worth building against? What if the market is too small — or too large and already crowded? What if every customer needs a custom build (service trap, not software)? What if retention is weak once the novelty wears off? What if the workflow is too infrequent to justify a subscription? What if the value can't be measured, so it can't be sold on ROI? What if onboarding takes months? What if switching costs protect the incumbent regardless of how bad it is? What if an AI-based approach isn't accurate enough and a human still has to check everything? What if liability becomes unacceptable? What if the target customer already has an internal dev team that'll just build it? What if procurement blocks a small/unknown vendor? What if there's no natural distribution channel to reach these buyers at all?

## Falsification requirement

For every hypothesis that survives the attack above, state explicitly: **what evidence would convince us this is NOT worth pursuing?** Examples: the problem occurs less than monthly; the current workaround costs under $100/month; fewer than ~10% of the target segment actually experiences it; competitors already charge under $20/month profitably; buyers explicitly say it's low priority; adoption requires ripping out a core system (ERP-class); onboarding needs months of consulting; the problem disappears after a one-time setup. Then actively research *for* disconfirming evidence, not only supporting evidence — the point is to try to break the hypothesis, not decorate it.

## Anti-confirmation-bias write-up (required for every top opportunity)

Write these four, in order, before calling anything validated:

1. **Bull Case** — why this could become a genuinely valuable business.
2. **Bear Case** — why this could fail badly.
3. **Kill Shot** — the single strongest reason not to pursue it, stated as sharply as an opponent would state it.
4. **What evidence would change our mind?** — the next concrete piece of evidence, and where to get it.

This is the concrete form of the Stance's "never stop at kill it" rule — it's not satisfied by a vague "there are risks," it needs all four sections filled with specifics.

## PMF stage ladder — don't call it validated before it is

Desk research and social listening are not product-market fit. Track progress on this ladder and never claim a stage that hasn't actually been reached:

0. **Hypothesis** — an interesting problem idea.
1. **Evidence of pain** — multiple independent signals.
2. **Evidence of existing spend** — customers already spend money or time solving it.
3. **Problem validation** — direct customer interviews confirm the pain.
4. **Solution validation** — customers actively try the proposed solution.
5. **Willingness to pay** — a customer agrees to actually pay.
6. **Repeatability** — multiple customers buy for the same stated reason.
7. **Early PMF signal** — strong retention / repeat usage / organic pull.

State plainly which stage the current evidence actually supports — "we have Level 4 evidence of pain (stage 1–2), nothing yet at stage 3" is a correct and useful statement; calling that "validated" or "PMF" is not.
