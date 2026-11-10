# Brain

A founder operating system in Claude Code. One goal: **become the most successful youth entrepreneur in Indonesia**, defined in numbers and checked every week.

It has three parts:

1. **A mentor** (`CLAUDE.md`). It knows your businesses, checks your commitments at the start of every session, weighs policy and ecosystem impact on every business question, thinks about investing in fundamentals rather than speculation, and corrects your English first (IELTS 7.5 target).
2. **Rituals** that keep pushing you: `/onboard`, `/checkin` (daily), `/weekly-review` (weekly), `/policy-watch` (monthly).
3. **The Roast Room**: a council of advisors that debates your big decisions and gives a scored verdict. It is built on [roast-room](https://github.com/nateherkai/roast-room) (MIT), with two seats added for Indonesia:

| Seat | Pillar | The question it owns |
|---|---|---|
| **Regulasi** | Policy and regulation (Indonesia) | Which rule, policy, or official decides whether this works, and what happens when that policy shifts? |
| **Ekosistem** | Ecosystem and impact (Indonesia) | Does this make the wider ecosystem stronger, and will that strength come back to the business? |

Both are knowledge seats, not people. They are built from MBG and BGN rules, procurement (LKPP, e-katalog, TKDN), construction licensing, BUMN and Danantara, OJK, data protection, labour, tax, and anti-corruption law. Every fact has a confidence tag, and `/policy-watch` refreshes them from the web. They sit on the default board next to Bezos, Paul Graham, Hormozi, Gary Vaynerchuk, Dan Martell, Gino Wickman, and Buffett. Naval, Codie Sanchez, Leila Hormozi, Sara Blakely, and Elon Musk are on call.

## Start here

1. Open Claude Code in this folder (or in a cloud session on this repo).
2. Run `/onboard`. It asks about 15 to 20 quick questions and fills `me/profile.md` and `me/north-star.md`.
3. Every morning: `/checkin morning`. Every evening: `/checkin evening`.
4. Every Sunday: `/weekly-review`.
5. Any big decision: `/roast-room <the decision, your options, your numbers, your lean>`.
6. Once a month, and before signing anything that depends on a rule: `/policy-watch`.

Example council:

```
/roast-room Should I become an SPPG mitra myself (build and run an MBG kitchen),
or stay a supplier of kitchen equipment and consulting to mitra? Capex for a kitchen
is about Rp1.5 miliar (assumed). Equipment business makes TODO per month. I'm leaning
toward running a kitchen because it locks in demand for my supply chain plan.
```

## The weekly loop

```
morning checkin ──> work ──> evening checkin ──> (x7) ──> weekly review
      ^                                                       │
      └────── commitments and next week's one big thing ──────┘
big decision ──> /roast-room ──> decisions/log.md ──> reviewed on its date
```

## Files

| Path | What |
|---|---|
| `CLAUDE.md` | The mentor's operating rules |
| `me/` | Your profile, north star, commitments, scorecard |
| `journal/` | Daily check-ins |
| `decisions/log.md` | Decisions with your predictions, reviewed later |
| `sessions/` | Roast Room councils |
| `.claude/skills/` | `onboard`, `checkin`, `weekly-review`, `policy-watch`, `roast-room`, `newroaster` |
| `.claude/skills/roast-room/brains/regulasi-indonesia/`, `ekosistem-indonesia/` | The Indonesia knowledge seats |
| `app/` | The visual room (`npm start`, then http://localhost:4730) |
| `docs/roast-room.md` | Full Roast Room documentation |

## Important

- **Keep this repository private.** It holds business numbers and your journal.
- **Cloud sessions are deleted** after use; the rituals commit and push so your history survives.
- The Regulasi seat's knowledge is dated. Facts marked VERIFY must be checked before a one-way decision. Nothing here is legal, tax, or investment advice; get sign-off from a licensed Indonesian professional.
- Person seats are simulations built from public work, not the people themselves. See `docs/roast-room.md`.

Roast Room code: MIT, AI Automation Society (see `LICENSE`).
