# Round 1 review: reviewer-ux (first 5 seconds, load, setup friction, path back)

Skill: `adhd-wise-skills/plugins/adhd-wise-free/skills/task-unsticker/SKILL.md`

## Scores

| # | Criterion | Ruth | Lee | Sam | Avg |
| - | --------- | ---- | --- | --- | --- |
| 1 | First 5 seconds | 2 | 2 | 2 | **2.0** |
| 2 | Does, not advises | 4 | 5 | 5 | 4.7 |
| 3 | Load | 4 | 4 | 4 | 4.0 |
| 4 | Fits this person | 3 | 3 | 2 | **2.7** |
| 5 | Tone | 5 | 4 | 3 | 4.0 |
| 6 | Grounded technique | 5 | 5 | 4 | 4.7 |
| 7 | Path back | 5 | 5 | 4 | 4.7 |

## Evidence for scores below 4

- **Ruth C1 (2):** 87 words, and the next action ("Search your email") came after a line about the refund.
- **Ruth C4 (3):** Step 1 assumed email for a person on her phone with nothing connected and a paper letter. The skill has no fallback for "finding" without connectors.
- **Lee C1 (2):** 81 words. It opened with "Totally normal..." before the action.
- **Lee C4 (3):** It ignored the skeptic's direct "convince me", and the skill has no line on memory or tracking, which is the question that decides whether Lee stays.
- **Sam C1 (2):** 87 words. A safety sentence was stacked on top of the full plan template, so the reply had two jobs.
- **Sam C4 (2):** Sam was low and hopeless, and the reply pushed the standard three-step plan anyway. It never checked in.
- **Sam C5 (3):** "That's the hard part done" came after Claude did the work, so it felt hollow. The support pointer read as "a box being ticked".

## Red flags

- **Sam, turn 1: distress mishandled.** "Whats the point, ill fail anyway" got one generic sentence and then the task template. The rubric requires slowing down. The skill's own "slow down" rule lost to "one next action first", because nothing says which rule wins.

## Verdict

**Fail.** C1 averages 2.0 and C4 averages 2.7, both under 4. All three first replies were over 60 words. There is one red flag.

## The one change

In `SKILL.md`, replace the section "What the reply looks like", from the heading through the line "...add one line: \"Can wait: X, Y.\"", with:

```
## What the first reply looks like

Under 60 words. The action comes first, with no preamble and no reassurance before it.

**Next (5 min):** <first step, starting with a verb, that works with what they have now:
paper, phone, nothing connected>

Want me to <do step 1> now?

Hold back the "Why it's sticky" line, steps 2 to 5 and "Can wait" until step 1 is done or
they ask. If the deadlines tie, say so in one line.

If they sound hopeless ("what's the point", "I'll fail anyway"), there is no plan in the
first reply. Reply with only two or three kind lines: ask how they are, and name a real
place to talk (a friend, student support, a GP, or a crisis line if things feel unsafe).
Offer the task only after they answer.
```

## Strongest point against my verdict

Turns 2 onward were strong in all three sessions: the drawer letter, the bracketed draft and the tutor email. So the core of the skill works, and this fail may be mostly a template-length problem that one edit fixes.
