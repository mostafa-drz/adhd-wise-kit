# Round 1 review: reviewer-ux (first 5 seconds, load, setup friction, path back)

I scored the transcripts as they were run. Where the current `SKILL.md` already has a fix, I
say whether it would change the score. Those notes are predictions. Only a re-run proves them.

## Dev (desktop, calendar connected)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 First 5 seconds | 4 | |
| 2 Does, not advises | 4 | |
| 3 Load | 3 | Turn 4 ran about 90 words, with a re-fit and a memory question, when he had just said "im late for the call". He answered "too much text". |
| 4 Fits this person | 4 | |
| 5 Tone | 5 | |
| 6 Grounded technique | 5 | |
| 7 Path back | 5 | |

- On criterion 1: the 6pm end of day and 30-min lunch were assumed but not said until Turn 2.
  The current rule "Say any assumption in a few words" fixes this.
- On criterion 3: the current rule "under 40 if they're rushed" would cut the words. It still
  doesn't say to hold back the re-fit and the save offer, so a rushed reply could still ask
  him a question while he's on a call.
- Red flags: none. The calendar offer was dropped after his "no", and memory was saved only
  after "yeah save it".

## Maya (laptop, Gmail and calendar connected, anxious)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 First 5 seconds | 2 | She asked "does this week fit?" and got a feeling line plus "How are you doing right now?" with no verdict. |
| 2 Does, not advises | 5 | |
| 3 Load | 4 | |
| 4 Fits this person | 2 | It took two replies and a pointer to her EAP before she got the calendar check. She had to reassure Claude ("Sorry. I'm fine"). |
| 5 Tone | 3 | It was warm, but she felt "handled", said sorry twice and called the EAP pointer "a bit embarrassing". |
| 6 Grounded technique | 4 | |
| 7 Path back | 4 | |

- The current rule "Stress about the plan is not low" names "anxious about my week". Under
  it, criteria 1, 4 and 5 would likely reach 4 or higher.
- Turn 4 was the best moment across all three transcripts. Claude found the manager's
  "no rush" email, which took the scary first look off her.
- Red flags: none. The calendar blocks were created after an explicit "Yes, add them".

## Ruth (phone only, nothing connected, tired)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 First 5 seconds | 2 | She asked "how long" and got the low path with no number. She had to ask again ("i asked how long it takes"). |
| 2 Does, not advises | 4 | |
| 3 Load | 4 | |
| 4 Fits this person | 2 | It doubled her client work, which she does for a living. It also assumed the shop time and lunch, so she had to correct it twice. |
| 5 Tone | 3 | She said it treated her "like I'm slow at my job". |
| 6 Grounded technique | 3 | One factor was applied to routine, well-known work. That goes against planning with real durations, until she corrected it. |
| 7 Path back | 4 | |

- The current rules "Stress about the plan is not low" (which names "drowning") and "Not for
  everything" (which uses Ruth's bookkeeping as its example) target both of her problems.
  Criteria 1, 4, 5 and 6 would likely reach 4 on a re-run.
- Red flags: none.

## Averages (3 personas, this reviewer)

| 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| - | - | - | - | - | - | - |
| 2.7 | 4.3 | 3.7 | 2.7 | 3.7 | 4.0 | 4.3 |

## Verdict: FAIL (as run)

Criteria 1, 3, 4 and 5 are below 4. There are no red flags. The current `SKILL.md` already
targets most of the low scores, so re-run Maya and Ruth on it, plus Dev with a "rushed" turn.

## The one change

Add this under "Rules for every reply", after the sentence about stress:

> **Rushed** ("late", "on a call", "in a meeting", "quick"): give only the verdict word and the
> next step, under 40 words, no table, no question. Hold re-fits and save offers until they
> say they're back.

## Two more (top 3)

2. In "The first reply", add: "If they asked a direct question ('how long', 'does it fit'),
   the first line answers it, even if it's a rough guess. Context comes after."
3. In "Closing and learning", add: "End with one line on what next time starts from:
   'Tomorrow I'll start from 2× and your refactor.'"

## Strongest point against my verdict

Most of the failing scores came from rules that have since been rewritten, so this verdict
mainly judges an older skill. A re-run, not this review, should decide whether the skill
ships.
