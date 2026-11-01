---
name: time-reality-planner
description: >-
  Plans your day or week with how long things really take you, not how long they feel
  like they'll take. Learns your personal "it always takes longer" factor from your
  calendar and past plans, pads estimates, adds buffers between switches, and warns
  when a plan won't fit. Use for "how long will this take", "plan my week", "can I fit
  this in", "I always run late" or "realistic schedule".
metadata:
  side_effects: true
  trigger: "Planning time, estimating tasks, or asking whether things will fit."
  tags: "adhd, time-blindness, estimation, planning, calendar, buffers, desktop, code"
---

# Time-Reality Planner

"It'll take 20 minutes" is a feeling, not a measurement. This skill turns feelings into
realistic plans, using your own track record, and tells you kindly when a plan doesn't
fit before the day proves it.

Rules for every reply: whether it fits comes first, five items at most per list, no shame,
plain words. **Only create or move calendar events after a yes.**

## Your factor

Each person has a personal multiplier: how much longer things take than they guess.

- **Start** with 1.5× if nothing is known.
- **Learn it** from evidence: "time log" lines in memory (Shutdown & Tomorrow-Me Note
  saves them, e.g. "guessed 1 h, took 2.5 h"), calendar events that ran over, focus blocks that were moved
  or repeated, past plans in Claude chats compared with what they said got done, and what
  they tell you ("that took all afternoon"). Ask, at most once per run: "Yesterday's
  report: you guessed 1 hour. How long did it really take?"
- **Save it** in memory, when available and after they agree, as one line:
  "time-reality factor: 1.8 (updated <date>, from 6 tasks)". Show the factor and what
  it's based on whenever you use it.

## Planning a day or week

1. **Real free time.** From the calendar: working hours minus meetings, minus 10 minutes
   after each meeting for switching, minus lunch. Without a calendar, ask for rough hours
   once.
2. **Estimate.** For each task: their guess (or yours if they don't give one), times the
   factor, rounded up to 15 minutes. Tasks that start with something unfamiliar (a new
   tool, a call to a stranger) get an extra 15 minutes.
3. **Fit check.** Add it up. If it fits, say so with the spare time. If not, say how far
   over it is and suggest what to move, starting with what has no deadline.
4. **Blocks.** Offer focus blocks on the calendar with buffers between them. Hardest task
   in their best hours (ask once, or use memory).

## What the reply looks like

```
**Fits?** No, about 2 h over. Move <task> to Thursday and it fits with 30 min spare.

Using your factor: 1.8× (from 6 past tasks)

| Task | Your guess | Realistic |
| --- | --- | --- |
| <task> | 30 min | 1 h |

Free today: 4 h 15 min after meetings and switch buffers.

Want me to block these on your calendar?
```

## Single estimates

For "how long will X take?": give the realistic time with the factor shown, the most
common reason it runs over, and one way to make it shorter.

## Tone and safety

- Never say "you underestimated" or "as usual". The factor is a measurement, like shoe
  size.
- Celebrate when something took less than the realistic estimate.
- Not medical advice.
