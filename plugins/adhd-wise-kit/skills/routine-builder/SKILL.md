---
name: routine-builder
description: >-
  Builds a routine you'll actually keep: anchored to something you already do, small
  enough to start tomorrow, with a "minimum version" for bad days, and optional reminders
  set up as calendar events or Claude scheduled tasks. Use for "build a routine", "morning
  routine", "I can't stick to habits", "evening routine" or "help me start exercising /
  journaling / tidying".
metadata:
  side_effects: true
  trigger: "Wanting to build or rebuild a routine or habit."
  tags: "adhd, routines, habits, anchors, reminders, scheduled-tasks, desktop, code"
---

# Routine Builder

Most routines fail because they're designed for your best day. This skill designs for
your average day, with a minimum version for your worst one, so the routine survives a
bad week.

Rules for every reply: the routine first, five steps at most, no streaks, no shame,
plain words. **Only create calendar events or scheduled tasks after a yes.**

## The flow

1. **One routine.** Which part of the day, and what it's for ("mornings so I leave on
   time"). If they want five new habits, help pick one to start.
2. **Anchor.** Attach it to something that already happens every day: after coffee, when
   the laptop opens, after brushing teeth. Ask what reliably happens at that time.
3. **Design it small.** Three to five steps, each with a time, total under 20 minutes to
   start. Put the easiest step first so starting is effortless.
4. **Minimum version.** The two-minute version for bad days ("just put on shoes"). Doing
   the minimum counts as doing the routine.
5. **Make it visible.** Offer one of: a calendar event at the anchor time, a Claude
   scheduled task that sends the checklist each morning (where scheduled tasks are
   available), or a short checklist to copy to a sticky note or phone. Set it up only
   after a yes.
6. **Restart rule.** Tell them up front: "Missing days is part of it. When you come back,
   start with the minimum version." Never count or mention streaks.

## What it looks like

```
**Your morning routine** (after coffee, about 12 min):
1. <easiest step> (1 min)
2. <step> (5 min)
3. <step> (6 min)

**Bad-day version (2 min):** <minimum>

**Restart rule:** skipped days are normal; restart with the 2-minute version.

Want me to add a calendar reminder at <time>, or set up a daily scheduled task?
```

## Check-ins

If they come back saying it isn't working, don't add willpower: shrink it, move the
anchor, or swap a step. Ask one question: "Which step is the one that gets skipped?"

## Safety

For exercise or sleep routines, keep advice general and suggest checking with a
professional for medical concerns. Not medical advice.
