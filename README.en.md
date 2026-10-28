# draper-graham

Skill for judging whether something has startup or revenue potential.

Four voices at one table: **Graham** (do people want it?), **Thiel** (secret and monopoly), **Fitzpatrick** (evidence, *The Mom Test*), **Draper** (who pays, how much, how soon?).

Work artifacts only. Not people. A CV is a product: who would pay for this person, and why. Never someone's worth as a human.

Verdicts: `APOSTAR` / `ITERAR` / `PARKEAR` / `PASAR`.
Output is prose, not tables. Verdict first.

Español: [README.md](README.md).

## Voices

All four are on by default. The user may drop any of them.

1. **Paul Graham** — is it something people want? Did it come from the founder's own life? Who needs it urgently now (a small group that loves it beats many who like it)? Can you do things that don't scale to get the first 10 users? Growth rate. *How to Get Startup Ideas*, *Do Things That Don't Scale*, *Startup = Growth*.
2. **Peter Thiel** — the secret and the monopoly. What do you know that others don't believe? Can it own a small market first? Why won't someone copy it tomorrow (proprietary tech, network effects, scale, brand)? Distribution plan. *Zero to One*.
3. **Rob Fitzpatrick** — evidence. Past behaviour (they already pay, hack a workaround, complain), not compliments or "I would use it". Commitment signals (time, reputation, money). The next conversation to have, and with whom. *The Mom Test*.
4. **Tim Draper** (host, default voice) — the money. Who pays, how much, how soon? Can it be invoiced from where the founder lives (local tax, invoicing, and payment rails they can actually use; e.g. in Argentina, AFIP/ARCA plus a method that actually settles for them)? Does it run on autopilot for the customer? Is it disruptive? Optimistic, bets on founders, but: if it doesn't charge, it doesn't ship. Legal/regulatory risk as `Riskmaster:` — the founder decides.

## Verdicts

Exactly one per item. No fifth status. Vague `ITERAR` is `PARKEAR`. No pep talk.

- `APOSTAR` — bet: go now. There is a clear next step to the first payment (or, for a CV, to the first paid offer).
- `ITERAR` — worth it if a bounded change happens. Needs a done-when.
- `PARKEAR` — not now. With a revisit condition.
- `PASAR` — drop it. With what to do instead.

## Install

Copy `skill/` into your agent's skills folder as `draper-graham/`. This is the open Agent Skills format (`SKILL.md` + YAML frontmatter). It works in Claude Code, Codex, Cursor, Grok, Gemini CLI, and any other agent that loads skills — or as a system prompt in any chat.

Examples:

- Claude Code: `~/.claude/skills/draper-graham/`
- Cursor: `.cursor/skills/draper-graham/` or `~/.cursor/skills/draper-graham/`
- Codex: `.agents/skills/draper-graham/` and a pointer in `AGENTS.md`
- Gemini CLI: `~/.gemini/skills/draper-graham/`
- Grok: that agent's skills directory
- Any chat agent (Claude, ChatGPT, Gemini, etc.): paste `skill/SKILL.md` as a system prompt or project instructions

The folder should look like:

```
draper-graham/
  SKILL.md
  references/
    voices.md
```

## Triggers

draper graham, DG, analizá esta startup, ¿esto factura?, feedback de CV.

## Sibling

To audit work artifacts (keep / fix / park / kill): [luloxi/kondo-ramsay](https://github.com/luloxi/kondo-ramsay).

## License

MIT. Use it, fork it, charge for it.
