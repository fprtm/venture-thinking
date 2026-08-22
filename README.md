# venture-thinking

A Claude skill that stress-tests a business, product, or feature idea *before* you build it.

It runs a loop — **idea → hypothesis → riskiest assumption → cheapest test → one action this week** — instead of letting an idea coast on optimism. Amateurs ask *"is my idea good?"*; this skill asks *"which assumption is riskiest, and what's the cheapest way to find out?"*

Fires automatically when you bring an idea, ask "should I build this?", want to validate a market or willingness-to-pay, frame the real problem behind a request, or decide whether to pivot.

## What's inside

```
venture-thinking/
├── SKILL.md                  # the active loop the agent runs
└── references/
    ├── framing.md            # the 7-question FRAME battery
    ├── loop.md               # full OBSERVE → SCALE arc, wedge, horizons
    ├── economics.md          # quick unit-economics check (margin, CAC, LTV)
    └── skill-tree.md         # the 13 sub-skills, for self-study
```

## Install

Skills are just a folder with a `SKILL.md`. Drop this repo into any agent's skills directory.

**Claude Code — personal (all projects):**
```bash
git clone git@github.com:fprtm/venture-thinking.git ~/.claude/skills/venture-thinking
```

**Claude Code — one project only:**
```bash
git clone git@github.com:fprtm/venture-thinking.git .claude/skills/venture-thinking
```

**Update everywhere later:**
```bash
git -C <path>/venture-thinking pull
```

Once installed it is model-invoked: the agent reaches for it on its own when you're weighing an idea. You can also just describe an idea and let it fire.

## License

MIT — see [LICENSE](LICENSE).
