# DISCOVER (Stage 0) — finding the opportunity before there's an idea to test

Only run this stage when the person has **no idea yet** and wants markets/pains worth pursuing found from scratch ("what should I build", "find me a painful problem", "I'm a developer looking for a venture"). If they already brought an idea, skip straight to FRAME — DISCOVER is a wide-funnel search, FRAME is narrow interrogation of one thing.

**Everything in this stage runs at SNIFF tier** (see SKILL.md's "Rigor tiers" section) — quick reasoning, light search (~10–15 sources total per candidate being screened, not per step), checked against the named traps in [`red-team.md`](red-team.md). None of the 13 steps below need a full 50-source treatment or a complete red-team writeup — that only happens once, for the single opportunity that survives all the way to Step 13 and gets handed to FRAME. Treating every industry/segment/niche/pain candidate here as if it needed FULL rigor is exactly what made a real run of this process expensive for zero surviving ideas — most candidates should die in minutes at SNIFF, not hours.

**Do not start from technology.** Never open with "what SaaS/AI product should I build" — that's the solution jump the Stance already forbids, just one level earlier. Start from: *who has a painful, recurring, expensive, urgent problem, and what evidence proves it deserves solving.* The target endpoint is a customer who would say "I don't care what technology you use, just make this problem go away" — implementation vehicle (software, automation, agent, service) comes after the pain is proven, not before.

## The funnel: top-down, one narrowing decision at a time

When there's no idea at all yet, don't jump straight to hunting for pain across a scattered pile of markets — narrow in this explicit order, each step feeding the next:

```
Industry (pick the single best one)
        ↓
Market segmentation (within that industry)
        ↓
Niche (pick the single best segment)
        ↓
Pain-hunt (within that niche only)
        ↓ (market map + evidence across candidate pains)
   ~5 shortlisted opportunities
        ↓ (deep dive)
   top 3, fully mapped
        ↓ (red team — see red-team.md)
   1 hypothesis, fed into FRAME
```

Don't lock onto the first interesting market. Traditional industries with bad software (construction, field services, property management, insurance ops, procurement, agencies) are often better hunting ground than "software startups" as customers — boring beats trendy.

### Step 1 — pick the best industry first

List 10–20 industries/functions as candidates (finance ops, accounting, logistics, ecommerce ops, healthcare admin, legal ops, construction, property management, manufacturing, field services, insurance ops, recruiting ops, procurement, sales ops, customer success, compliance, cybersecurity ops, IT/DevOps, developer infra, data ops, marketing ops, agencies, professional services, education admin, government contractors, niche SMB industries, import/export, supply chain, hospitality, automotive ops, B2B marketplaces — not exhaustive). Cross-reference against [`domain-knowledge.md`](domain-knowledge.md)'s Atlas industry map (§8, 45 industries) for real subindustries/roles/processes instead of guessing generically.

Compare candidates at the industry level — not a full pain investigation yet, just a sniff test — on **boring-but-expensive** signals: "we still do this manually," "we export it to Excel," "someone checks this every day," "we hired someone just for this," "we copy this from system A to system B," "we hate our current provider," "it takes days," "we pay consultants to do this," "it's required for compliance," "we can't afford mistakes here." Then commit to **one industry** to go deeper on, stating explicitly why it beat the others (don't carry all 10–20 forward in parallel — pick, then go deep; if the chosen one dead-ends later, that's what the DISCOVER restart in Iterate is for).

### Step 2 — segment that industry's market

Within the chosen industry, segment the market on the dimensions that actually change buying behavior: company size (solo/SMB/mid-market/enterprise), geography, business model (B2B vs B2C, subscription vs project-based), buyer type/role, and sub-vertical (e.g. within Healthcare: dental clinics vs hospitals vs home-care agencies are different markets, not one). List the real segments — don't invent generic ones — using Atlas's subindustry/role breakdown ([`domain-knowledge.md`](domain-knowledge.md)) as the vocabulary source.

### Step 3 — narrow to the single best niche

Pick the one segment most worth investigating, favoring **narrow market + severe problem + accessible customers + high willingness to pay** over **huge market + vague problem + hypothetical users**. State explicitly why this niche beat the other segments from Step 2 (accessibility, believed pain severity, believed budget, founder fit) — this is a reasoned bet based on what's known so far, refined with real evidence in the next step, not a guess to defend at all costs.

### Step 4 — now, and only now, hunt for the pain within that niche

With industry → segment → niche fixed, map the actual workflow: **actors** (who participates) → **workflow** (start to finish) → **frequency** → **inputs/outputs** → **software currently used** → **handoffs** → **manual steps remaining** → **bottlenecks** → **errors and consequences** → **workarounds** → **cost** → **buyer** → **trigger** → **alternatives** (software, employees, agencies, consultants, spreadsheets, doing nothing). If a dedicated workflow-discovery tool/skill is available in this environment, it can do this mapping — otherwise do it directly with search + reasoning.

### Step 5 — workarounds are gold

Search aggressively for "ugly solutions" within the chosen niche: spreadsheets (Excel/Sheets), Notion/Airtable databases, email chains, Slack/WhatsApp reminders, manual copy-paste, VAs/offshore staff, consultants/agencies/interns, Zapier/Make chains, Python scripts, macros, browser automation, homemade dashboards, CSV exports, screenshots, manual reconciliation, repeated meetings. An ugly homemade workaround means the problem matters enough that someone built something instead of doing nothing — document what it is, who runs it, how often, how long it takes, what it costs, why they tolerate it, what breaks, what they hate, and why existing software hasn't replaced it.

### Step 6 — competition is validation, not automatic rejection

No competitors can mean an undiscovered niche — or it can mean nobody cares. Existing competitors prove demand, budget, buying behavior, and category awareness — don't reject the niche just because it's occupied. Instead investigate *why customers still complain*: underserved sub-segments, expensive incumbents, terrible UX, poor integrations, enterprise-only pricing, SMB-unfriendly pricing, weak automation, poor localization, missing workflows, slow support, compliance gaps, fragmented tooling, customers stitching multiple tools together. Search patterns: `[competitor] alternative`, `[competitor] sucks`, `[competitor] too expensive`, `[competitor] pricing`, `[competitor] manual`, `[competitor] workaround`, `[competitor] reddit`, `[competitor] review`.

### Step 7 — buying signals (stronger than stated opinions)

Prefer behavioral evidence over stated opinion: hiring people specifically to perform the task, consulting firms offering this exact service, freelancer/Upwork/Fiverr jobs requesting this workflow, RFPs, expensive software already purchased for it, customers publicly asking for alternatives, implementation-consultant ecosystems around an incumbent, training courses teaching the manual process, template ecosystems, operational roles that exist solely to manage the problem. "People say this would be useful" is weak; "companies already pay $20k/yr for a hated incumbent because the task can't be ignored" is strong.

### Step 8 — market map table (candidate pains within the chosen niche)

By this point the industry, segment, and niche are fixed — this table compares the **distinct pains/workflows found within that one niche**, not different industries:

| Pain/Workflow | Actor | Core Pain | Pain Evidence | Existing Spend | Frequency | Buyer | Current Solution | Dissatisfaction | Builder Leverage | Evidence Level |
|---|---|---|---|---|---|---|---|---|---|---|

Research at least 10 serious candidate pains within the niche before narrowing further. Don't pad the table with filler ideas to hit a count — a shorter honest list beats a padded one (same "no silent caps" principle as everywhere else in this skill: if fewer than 10 genuinely distinct pains exist in this niche, say so, and it's fair evidence the niche itself may be too narrow).

### Step 9 — pain scoring (for ranking the shortlist)

Score each candidate pain 1–10 on: Severity, Frequency, Urgency, Economic Impact, Current Spend, Dissatisfaction (with current alternatives), Buyer Clarity, Reachability, Buildability (can a small team solve it), Time to Value, Switching Feasibility, Recurring Need, Retention Potential, Expansion Potential, Competitive-Advantage Potential.

**Weight Severity, Economic Impact, Current Spend, Buyer Clarity, Reachability, and Recurring Need higher than the rest.** Never let a high total built from lots of mediocre scores disguise weak pain — a candidate with Severity 4/10 should almost never make the shortlist regardless of how the other numbers look. Scores support reasoning, not replace it; don't fake precision with decimals.

### Step 10 — shortlist ~5, then deep-dive the top 3

For the shortlist of ~5, state per candidate: Pain/workflow, precise ICP, existing workflow, pain consequence, evidence, current spend/workaround, existing competitors, why incumbents fail, buyer, trigger, distribution, possible wedge, builder-leverage fit, major risks, falsification conditions (see [`red-team.md`](red-team.md)), confidence.

For the **top 3**, go deeper — market definition (precise segment), customer profile, job to be done (functional + economic), workflow map, pain map, root cause, economic cost range, current alternatives (incl. doing nothing), competitive landscape (direct + indirect + non-software), buying process (user/champion/buyer/blocker), buying trigger, solution wedge, pricing logic, distribution (how the first 10 customers get acquired realistically), retention rationale, expansion path, risks, red team (strongest reasons *not* to pursue — [`red-team.md`](red-team.md)), validation tests, and who specifically to interview next.

### Step 11 — wedge, not platform

Never propose a broad platform first. Bad: "AI platform for logistics companies." Better: "Automatically reconcile carrier invoices against contracted freight rates for mid-sized importers using 3PL providers." Use the template:

> We help **[specific customer]** solve **[specific painful workflow]** when **[trigger/context]**, reducing **[measurable consequence]**.

### Step 12 — distribution and reachability, checked before falling in love with the idea

For every finalist: where do these customers congregate (professional communities, industry associations, LinkedIn, niche conferences/newsletters, Reddit/Slack/Facebook groups, supplier ecosystems, marketplaces, integration marketplaces, consultants/agencies/accountants/brokers as resellers, cold outbound, SEO, YouTube, industry directories)? Estimate ease of identifying prospects, contact availability, buyer concentration, likely response rate, sales cycle, trust barrier.

If the person building this has no major brand or team, explicitly answer: **could they realistically contact and interview 20–50 potential customers themselves?** If no, downgrade the opportunity unless another strong distribution mechanism exists (an accessible reseller/consultant channel, an existing community they're already in).

### Step 13 — "why now"

Investigate the catalyst that makes this solvable *now* and not five years ago or five years from now: AI capability jump, new API availability, regulatory change, labor cost increase, remote work shift, fragmented SaaS stacks, new compliance requirement, incumbent price increase, category shift, platform change, new data availability. Don't force a timing narrative — if there's no strong "why now," say so plainly rather than inventing one.

## Builder-leverage filter (only when the person building this is a developer/technical)

Favor problems where software leverage clearly matters: API-accessible data, repetitive digital workflows, browser-based operations, structured/semi-structured documents, frequent reconciliation, high-volume communication, workflow orchestration, cross-system sync, reporting, monitoring, rules-based decisions, human-in-the-loop automation, legacy-system integration, fragmented systems, data extraction/classification/document processing, scheduling, alerting, audit trails. Don't assume AI is required — recommend the simplest technical approach that removes 80% of the pain. Possible solution forms: automation, integration, workflow software, vertical SaaS, internal-tool-as-product, managed software, API, data pipeline, browser automation, agent, human-in-the-loop system, software-enabled service.

**Service-first is a legitimate path, not a fallback failure.** `manual service → understand the workflow deeply → standardize → automate → productize` is often the correct sequence, especially for a solo/small builder with no distribution yet — it forces real workflow understanding before writing a line of reusable code. Distinguish a genuine **service wedge** (temporary, deliberately chosen to learn and prove willingness-to-pay before automating) from a **permanent low-margin custom-consulting trap** (every customer needs a bespoke build, nothing standardizes) — flag explicitly which one a given opportunity risks becoming.

## Output of DISCOVER

End DISCOVER with a **final recommendation, not a menu of equal options**: the one opportunity to investigate first (exact market, exact ICP, exact painful workflow, strongest evidence, current workaround, why people would pay, why now, wedge, initial offer, pricing hypothesis, acquisition approach, biggest risk, fastest falsification test), plus a second and third choice with the specific reason each lost to #1. Then feed opportunity #1 into **FRAME** as the hypothesis to interrogate and run through the rest of the loop — DISCOVER's output is an input to FRAME, not a replacement for it.
