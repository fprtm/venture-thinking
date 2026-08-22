# venture-thinking

A Claude skill that stress-tests a business, product, or feature idea *before* you build it.

It runs a loop — **idea → hypothesis → riskiest assumption → cheapest test → one action this week** — instead of letting an idea coast on optimism. Amateurs ask *"is my idea good?"*; this skill asks *"which assumption is riskiest, and what's the cheapest way to find out?"*

Fires automatically when you bring an idea, ask "should I build this?", want to validate a market or willingness-to-pay, frame the real problem behind a request, or decide whether to pivot.

## What's inside

```
venture-thinking/
├── .claude-plugin/
│   ├── plugin.json            # plugin manifest (name, version, license)
│   └── marketplace.json       # makes this repo installable as a marketplace
├── SKILL.md                   # the active loop the agent runs
└── references/
    ├── framing.md             # the 7-question FRAME battery
    ├── loop.md                # full OBSERVE → SCALE arc, wedge, horizons
    ├── economics.md           # quick unit-economics check (margin, CAC, LTV)
    ├── research.md            # desk research vs primary evidence
    └── skill-tree.md          # the 13 sub-skills, for self-study
```

## Install

### Claude Code or Cowork — one URL, one click (recommended)

Both read this repo as a plugin marketplace, so no manual file copying is needed.

**Claude Code (CLI):**
```bash
claude marketplace add fprtm/venture-thinking
claude plugin install venture-thinking@venture-thinking
```

**Cowork (Desktop app or claude.ai):**
1. Sidebar → **Customize** → **Plugins**
2. **Add marketplace** → paste `https://github.com/fprtm/venture-thinking`
3. Find **venture-thinking** in the list → **Install**

Updating later: `claude marketplace update venture-thinking`, or click **Update** on the marketplace in Cowork's Plugins page.

### Claude Code — manual clone (alternative)

Skills are just a folder with a `SKILL.md`; you can also drop this repo straight into a skills directory.

```bash
# personal, all projects
git clone https://github.com/fprtm/venture-thinking.git ~/.claude/skills/venture-thinking
# one project only
git clone https://github.com/fprtm/venture-thinking.git .claude/skills/venture-thinking
```
Update later: `git -C <path>/venture-thinking pull`

---

Once installed it is model-invoked: the agent reaches for it on its own when you're weighing an idea. You can also just describe an idea and let it fire.

## License

MIT — see [LICENSE](LICENSE).
