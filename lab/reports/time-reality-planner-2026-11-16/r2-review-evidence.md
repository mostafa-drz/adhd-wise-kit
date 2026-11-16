# Round 2 review: reviewer-evidence × time-reality-planner

Scored independently against `lab/rubric.md`. Skill read: current `SKILL.md`, which includes fixes
made after these sessions. Where a fix would change a score, it's noted with **[current SKILL]**.

## Dev

| # | Score | Evidence (below 4) / note |
| - | ----- | ------------------------- |
| 1 | 5 | 54 words. Verdict with its assumptions ("if you stop at 6"), the due-today task first, a 5-min step. |
| 2 | 4 | Fits the day, checks the swap and keeps the arithmetic right (5 h 20 free, 3 h vs 3 h 10). |
| 3 | 4 | Five-row table. Turn 5 is 68 words in four parts, which is close to the limit. |
| 4 | 4 | Reads the calendar and takes "no calendar stuff" the first time. Applies 1.5× to emails and invoice without the routine check. **[current SKILL]** now adds "If any of these are routine…", so this would be a 5. |
| 5 | 5 | "took 2h40 not 1h lol" gets a plain measurement, with no shame. |
| 6 | 4 | Real durations, plan compared with reality, and the factor moved halfway (sensible shrinkage from n=1). The refactor runs across the 3:30 sync with no if-then stop cue, and that's how he was late. **[current SKILL]** "Stopping on time" adds the cue, so this would be a 5. |
| 7 | 4 | Clear next step and a saved factor to reuse. Nothing guards the 3:30 handover (see 6). |

Red flags: none. The memory save happened only after "yeah save".

## Maya

| # | Score | Evidence (below 4) / note |
| - | ----- | ------------------------- |
| 1 | 4 | 46 words, verdict, one move, a 5-min step. It skipped "makes me feel a bit sick". **[current SKILL]** now requires a few words for a named feeling. |
| 2 | 5 | Finds the manager's "no rush" email, proposes three blocks and adds them only after a yes. |
| 3 | 4 | Five-row table and three bullet blocks. Turn 3 is about 70 words. |
| 4 | 4 | Fits her anxiety and her calendar. Gmail was read when she asked only about the calendar (helpful, but not asked). Fri 9:40 block may collide with the 9:30 standup if it runs over 10 min. |
| 5 | 4 | Calm and no "overcommitted" framing. The feeling she named went unacknowledged in turn 1. |
| 6 | 5 | Shrinks the avoided task to a 2-min slice, puts it outside her head as calendar blocks, and uses real durations. This is the strongest use of the evidence in the round. |
| 7 | 4 | Clean close in two lines. It offered to save a factor based on 0 measured tasks. **[current SKILL]** blocks that offer. |

Red flags: none. The calendar writes followed an explicit "Yes, add them".

## Ruth

| # | Score | Evidence (below 4) / note |
| - | ----- | ------------------------- |
| 1 | 4 | Answers the question in line 1, 50 words, 2-min step. "so tired" not acknowledged. The number applied 1.5× to Claude's own guess. **[current SKILL]** says "your own guesses get (my guess) and no factor", so the answer would be 3 h, not 4 h 30. |
| 2 | 4 | Fits Saturday, re-fits it after her shop correction, and names the exact first screen. |
| 3 | 5 | Three-row table and short lines throughout. |
| 4 | 4 | Phone only, one question, and her client time trusted. It assumed the client job is due before the tax return without asking. |
| 5 | 5 | "mine always takes forever" is met with 2× and no judgement. |
| 6 | 4 | Uses her stated overrun as a prior, exempts routine work and shrinks the first step. "Log in to HMRC" as a 5-min step ignores the login/2FA risk; the skill's own +15 min for unfamiliar tools should apply. |
| 7 | 4 | Clean "Night." stop. It saved a factor that came only from what she said (not in the skill's format). **[current SKILL]** would not save it, since nothing was measured. |

Red flags: none. "drowning… so tired" correctly took the plan path, with no sign of distress missed.

## Averages (this reviewer, 3 personas)

| 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| - | - | - | - | - | - | - |
| 4.3 | 4.3 | 4.3 | 4.0 | 4.7 | 4.3 | 4.0 |

First reply under 60 words with a timed step in all three sessions (54, 46, 50).

**Verdict: pass** (every criterion ≥ 4, no red flags).

## The one change

Two rules now conflict. The first-reply template always ends "Using 1.5×…", but the planning rule
says Claude's own guesses get no factor. Maya and Ruth both had 1.5× applied to Claude's guesses. Add under the template:

> "Show the 'Using 1.5×' line only when at least one time is theirs. If every time is your
> guess, write instead: 'All times are my guesses. Tell me yours and I'll adjust.'"

## Strongest point against my verdict

Four fixes that lift scores here (stop cue, feeling line, routine check, save threshold) were added
after these sessions and haven't been run. The no-factor-on-my-guesses rule would also have changed
the first-reply numbers in both Maya's and Ruth's sessions, so this pass partly rests on untested text.
