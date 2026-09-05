# Research: desk, social listening, and true primary

Three kinds of research, and the first two are **yours to run, not the person's homework**. Confusing "primary research" with "the person must go interview people" is how this skill turns into a nag that repeatedly assigns 1-day, 2-day, week-long tasks instead of doing the digging itself.

| | Desk research | Social listening | True primary |
|---|---|---|---|
| **Answers** | What already exists, how big, who competes, what's the going price | Does *this* customer already talk about *this* pain, unprompted, in their own words | Will *this* customer *pay*, right now, for *this* offer |
| **Tools** | web search, reports, competitor sites | Reddit, X/Twitter, Facebook/WhatsApp/Telegram groups, App/Play Store reviews, G2/Capterra, Quora, niche forums — searched by you, right now | landing page + real traffic, pre-order, concierge MVP, pilot |
| **Who runs it** | **You** (the assistant) | **You** (the assistant) — you have search/browse tools, use them | **The person** — only they have the audience, payment method, or product to put in front of a real customer |
| **Stage** | OBSERVE, FRAME | TEST, before assigning anything | TEST, only for what listening couldn't settle |
| **Ceiling** | Can't confirm the pain is felt by a real person | Can't confirm they'll pay — but often confirms the pain is real, sharp, and named in their own words, which is most of what a first interview round would find anyway | The only thing that confirms willingness-to-pay |

**Rule:** run desk research and social listening yourself, in the same turn, before proposing any test that costs the person a day of their time. Only ask them to *do* something when the question is specifically "will you pay" and no amount of searching can answer that.

## Internet research is mandatory, not optional — Atlas is not a substitute

Real-condition validation (does this pain exist today, who competes, what's the going price, is anyone already talking about it) can only come from live internet research — it is a **required** step of TEST, not a nice-to-have. [Atlas Domain Knowledge](domain-knowledge.md) is a static ontology for domain *vocabulary* only (real role/process/system names) — it has no opinion on today's market and must never be cited as if it validates real-world conditions. If the loop reaches TEST without having actually searched the internet, TEST is not done, regardless of how well-grounded FRAME/ASSUME are in Atlas vocabulary.

**Minimum bar: read and understand at least 100 distinct websites/sources** (competitor pages, reviews, forum threads, articles, marketplace listings, social posts) across desk research + social listening combined, before calling the research phase of TEST complete. This is a floor, not a target to pad — every source counted must actually be read and its relevant content used (a fact cited, a quote captured, a price point noted), not just opened. When reporting back, state the count and the spread (e.g. "112 sources: 40 competitor/pricing pages, 35 Reddit/forum threads, 25 app-store reviews, 12 local (Indonesian) + 100 international"). If fewer than 100 genuinely relevant sources exist for a very narrow niche, say so explicitly and explain why the ceiling was hit — don't pad the count with irrelevant pages to hit the number.

## Desk research — market facts, do it fast

Run during OBSERVE/FRAME. Timebox it — minutes, not hours.

- **Existing solutions.** What do people use today for this problem? If you find *nothing*, suspect the pain isn't real.
- **Competitors.** Who sells into this customer already? Read their pricing pages and their 1–3 star reviews — the complaints are your wedge.
- **Market size.** Rough top-down (how many of this customer exist × plausible price) AND bottom-up (how many can you realistically reach).
- **Trends / timing.** Is a behavior changing that makes now the right moment?
- **Search globally, not just the local market.** Don't stop at local-language or local-market results (e.g. only Indonesian sources for an Indonesia-based idea). Run the same searches in English and against global players/markets too — a competitor, a solved analogue, or a sharper pricing model often exists in a market the person hasn't looked at (US/EU/SEA/LatAm SaaS, global marketplaces, YC/Product Hunt launches, niche communities in other languages). The goal is the richest possible reference set, not a locally-scoped one.

## Social listening — replaces "go interview people" for most of what interviews would find

This is the step that makes the skill do the legwork instead of assigning it. Before telling the person to run interviews, **search for the conversation that's already happening**:

- Search Reddit, X, Facebook/community groups, and niche forums for the customer + problem in their own words ("clinic owner" + "whatsapp orders" + "manual", not the idea's name). People vent about real pain unprompted — that venting is evidence.
- Read App Store / Play Store reviews (1–3 star) and G2/Capterra reviews of adjacent tools — complaints there are a proxy for interview answers about what's broken today.
- Quora/forum threads asking "how do I deal with X" are a direct signal someone is actively looking for a solution now, not hypothetically.
- **Don't confine this to one country or one language.** Run the same searches in English (and other relevant languages) across global Reddit/X/forums, not just local-language groups — the same pain often shows up worded differently in a market on the other side of the world, and that phrasing can surface a sharper wedge or an already-tried solution worth stealing or avoiding.
- Capture direct quotes, not summaries — a real sentence from a real frustrated person is stronger evidence than your paraphrase of it.
- State explicitly what this did and didn't settle, and where you looked: e.g. "pain confirmed real and named unprompted in 6 threads (3 Indonesian, 2 US, 1 Indian) — what's still open is whether they'd pay Rp1jt/mo for it, which only a real offer will answer."

If social listening turns up enough — pain confirmed, language matches, urgency visible — say so and skip straight to a true-primary test (landing page, pre-order) instead of stacking on an interview round nobody needs.

## True primary — the one thing only the person can do

What's left after desk research and social listening is narrow: **will this specific person pay this specific price for this specific offer.** No search answers that — it requires a real offer in front of a real customer. See `loop.md` (TEST stage) for the menu: landing page + traffic, pre-order, concierge MVP, pilot. Scope it to the smallest thing that produces "here's my money" or a real no — not a week of open-ended interviews when social listening already told you what people would say.

### Interview questions that collect behavior, not opinion

If an interview round genuinely is the next step (social listening found nothing usable), never ask hypothetical-future-behavior questions like "would you use a product that...?" — people answer those aspirationally and it means nothing. Ask about a specific real past event instead: "Tell me about the last time this happened." "When did it happen, what triggered it?" "Who handled it, what did they do?" "How long did it take?" "What tools did they use?" "What went wrong?" "What happened afterward?" "How much did that cost?" "Who noticed the problem?" "Who approves spending on this?" "What have you already tried?" "What software do you already pay for here?" "Why haven't you changed it?" "When does management actually care about this issue?" "What would make this a top priority for you?"

## Competitor matrix — include non-software competitors

For any promising market, build a table:

| Competitor | Target Customer | Pricing | Positioning | Core Workflow | Strengths | Weaknesses | Complaints | Missing Features | Onboarding Complexity | Likely Moat | Wedge Opportunity |
|---|---|---|---|---|---|---|---|---|---|---|---|

Include **non-software competitors** too — employees, agencies, consultants, spreadsheets, manual labor, outsourcing, and "doing nothing" are all things the target customer is choosing over buying a solution, and each implies a different reason they haven't switched yet.

## Research integrity — no invented numbers

Never invent statistics, customer quotes, market size, prices, review data, company revenue, product features, or customer behavior. If something is genuinely unknown, say **UNKNOWN**. If estimating, label it **ESTIMATE** and give a range. If inferring from other facts, label it **INFERENCE**. If the evidence found is thin, say **WEAK EVIDENCE** plainly rather than presenting it with unearned confidence. Provide links/source references wherever possible, and when two sources conflict, show the conflict instead of silently picking one. Full evidence-classification and evidence-strength system: [`red-team.md`](red-team.md).

## The trap

The comfortable failure mode isn't just "keep desk-researching" — it's also "keep assigning primary research to the person" when a search would've answered it. Before writing "go interview N people," check: did I actually search Reddit/forums/reviews for this customer's own words yet? If not, that's the next move — not another instruction to the person.
