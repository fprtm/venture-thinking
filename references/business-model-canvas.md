# Business Model Canvas — properly filled, not a template dump

The Business Model Canvas (Osterwalder & Pigneur, *Business Model Generation*) is 9 blocks mapping how a venture creates, delivers, and captures value:

```
┌─────────────┬─────────────┬─────────────┬─────────────┬─────────────┐
│    KEY      │    KEY      │   VALUE     │  CUSTOMER   │  CUSTOMER   │
│ PARTNERSHIPS│ ACTIVITIES  │PROPOSITIONS │ RELATIONSHIPS│ SEGMENTS   │
│             ├─────────────┤             ├─────────────┤             │
│             │    KEY      │             │  CHANNELS   │             │
│             │  RESOURCES  │             │             │             │
├─────────────┴─────────────┴─────────────┴─────────────┴─────────────┤
│         COST STRUCTURE               │      REVENUE STREAMS         │
└───────────────────────────────────────┴───────────────────────────────┘
```

The failure mode isn't getting the 9 boxes wrong — it's filling them with generic, made-up placeholders ("Marketing" as a Key Activity, "Subscription" as a Revenue Stream) that could belong to any business. A canvas is *proper* only when every block is a direct, specific consequence of what FRAME/ASSUME/TEST already established for this idea — not a fresh brainstorm.

## When to produce it

Only once the loop has real material to draw from — at minimum FRAME is done (customer + pain + willingness-to-pay named) and ideally ASSUME/TEST have run too. A canvas built straight off a one-line pitch is fiction; say so and produce a draft canvas with the un-validated blocks explicitly marked, rather than inventing specifics to fill every box.

## Filling each block from the loop's own output — not from scratch

| Block | Pull it from | Bad (generic) | Good (specific, traceable) |
|---|---|---|---|
| **Customer Segments** | FRAME's "who exactly" | "Small businesses" | "Owner-operator klinik gigi 1–3 dokter, Jabodetabek, masih pakai buku antrian manual" |
| **Value Propositions** | FRAME's pain + painkiller/vitamin grading — one VP per segment if there's more than one | "Makes things easier" | "Menghilangkan 3 jam/hari admin manual entri antrian WhatsApp — painkiller, bukan vitamin, karena tanpa ini pasien menumpuk dan komplain" |
| **Channels** | Whatever TEST actually used or is proposing (landing page, WA broadcast, marketplace, referral from an existing supplier) | "Digital marketing" | "Landing page + iklan Instagram lokal ke grup komunitas klinik gigi, referral dari distributor alat gigi" |
| **Customer Relationships** | How the person actually interacts with this segment today (self-serve, high-touch onboarding, community) | "Customer support" | "Onboarding 1-on-1 by WhatsApp for the first 2 weeks, then self-serve" |
| **Revenue Streams** | ASSUME's willingness-to-pay figure + TEST's pass/fail signal on pricing | "Subscription" | "Rp99.000/bulan flat, ditagih via invoice WA — belum diuji, ini masih hipotesis dari FRAME" (mark explicitly if untested) |
| **Key Resources** | What must exist to deliver the value prop (a dataset, a license, a team skill, a partnership) | "Technology" | "Nomor WhatsApp Business API terverifikasi, template pesan approved Meta" |
| **Key Activities** | The core process from the domain grounding ([`domain-knowledge.md`](domain-knowledge.md)) that the venture must run well | "Marketing", "Sales" | "Triage antrian pasien real-time, sinkronisasi jadwal dokter" |
| **Key Partnerships** | Who the venture depends on and can't easily replace (a supplier, a platform, a distribution channel) | "Partners" | "Meta/WhatsApp Business Platform (dependency risk — API policy changes can kill the channel)" |
| **Cost Structure** | [`economics.md`](economics.md)'s Cost to serve + CAC, plus fixed costs implied by Key Resources/Activities | "Operational costs" | "Cost to serve Rp200rb/bln (WA API + hosting), CAC ~Rp1,5jt (iklan + referral fee)" |

## Rules for a mature canvas

- **One value proposition per distinct customer segment**, not one generic VP stretched across all of them — if there are two segments with meaningfully different pain, there are two rows.
- **Every number in Revenue Streams / Cost Structure must trace to [`economics.md`](economics.md)'s five numbers** (price, cost to serve, CAC, retention/LTV) — don't state a price or cost that hasn't been run through that check.
- **Mark what's validated vs. hypothesis.** A block backed by TEST evidence (social listening, a real test result) gets stated as fact; a block that's still a guess gets flagged inline (e.g. "— untested, riskiest assumption per ASSUME") so the canvas doesn't read as more certain than the loop actually is.
- **Key Activities and Key Resources should read like the domain's real value chain**, not generic startup verbs — pull the actual process/system names from [`domain-knowledge.md`](domain-knowledge.md) grounding instead of "build the app" / "do marketing."
- **Cross-check internal consistency** before presenting: does the Channel actually reach the named Customer Segment? Does the Revenue Stream's price match what TEST's willingness-to-pay signal actually showed? Does Cost Structure account for every Key Resource/Partnership that isn't free? A canvas with a contradiction between blocks is not done.
- **The riskiest assumption from ASSUME should be visibly attached to whichever block it lives in** — it's usually Revenue Streams (will they pay this price) or Customer Segments (is this really who has the pain) or Channels (can we reach them profitably).

## Localize global research back to the actual target market

Research now runs globally (see [`research.md`](research.md)) precisely so the canvas has richer reference points — a competitor's pricing model, a channel that worked, a pivot someone already tried elsewhere. But a foreign data point is an *input* to calibrate against, not a value to copy into the canvas verbatim. Before finalizing Revenue Streams, Channels, and Customer Relationships:

- **Re-price for the actual market**, don't transplant a foreign number. A $29/mo US SaaS benchmark tells you a *ceiling* or a *positioning signal* (premium vs. budget), not the Rp price to charge an Indonesian SMB — convert via local willingness-to-pay (ASSUME/TEST), not currency conversion.
- **Re-check the channel against local behavior.** A channel that works abroad (App Store search, cold email) may not exist as a real habit for this segment locally — if the target customer lives on WhatsApp/Instagram groups, the Channels block should say that, not "content marketing" because that's what the global example used.
- **Flag regulation, payment rails, and cultural norms that differ.** Payment methods (WA invoice + bank transfer vs. Stripe card-on-file), data/privacy rules, and trust signals (referral from a known distributor vs. a review site) vary by market — note explicitly where the global reference doesn't hold locally.
- **State it as a comparison, not a substitution:** "Global reference: US clinic-SaaS charges $49/mo self-serve. Target market reality: Indonesian klinik kecil owners don't self-serve on card payment and expect a human WA onboarding — canvas reflects the latter, global figure used only to sanity-check margin headroom."

## Format to present

A markdown table (9 rows: block name → content, 1–3 sentences each) is enough — don't build an ASCII grid by hand for the actual deliverable, that's only useful as the mental model above. Close the canvas with one line naming which block is least validated and what the TEST-stage result would need to be to firm it up.
