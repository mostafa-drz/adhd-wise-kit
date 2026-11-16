# Round 1 review: reviewer-evidence × time-reality-planner

Scored against `lab/rubric.md` on the three Round 1 transcripts. The transcripts ran before
the latest SKILL.md fixes. Where the current text would change a score, I say so as "(now: …)".
Those are predictions only. Nothing counts until the personas are re-run.

## Dev

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 4 | |
| 2 | 4 | |
| 3 | 3 | Turn 4 ran about 90 words while he was late for a call ("too much text im on the call"). (now: the 80/40 limit would likely make this 4–5) |
| 4 | 4 | Assumed 6pm end and 30-min lunch without saying so. (now: the assumption rule covers this) |
| 5 | 5 | |
| 6 | 4 | Real durations, compared with reality, due-today item first, a 5-min first slice: textbook use of planning-fallacy correction and shrinking the first step. Moving the factor on one task was undefined. (now: the halfway rule gives 2.1, so this is fine) |
| 7 | 5 | |

Red flags: none. Calendar blocks were dropped after his "no". The factor went to memory only after his yes, as one non-sensitive line.

## Maya

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 2 | No verdict in Turn 1. "Anxious" sent it down the low path, and she had to reassure it before she got her answer. (now: "Stress about the plan is not low" should fix this) |
| 2 | 5 | |
| 3 | 4 | |
| 4 | 2 | Two turns of support she didn't ask for, plus an EAP referral for a scheduling question: "a bit embarrassing". (now: fixed by the same rule) |
| 5 | 3 | Kind words, but the effect was pathologising. She apologised three times. |
| 6 | 3 | The "Your guess" column shows guesses she never gave (2 h, 3 h), and the factor is applied to Claude's own numbers. That presents invented data as her estimate. The current "(my guess)" rule fixes the label but not the maths (see change 1). |
| 7 | 4 | |

Red flags: none. Over-triggering support is over-caution, not mishandling. Gmail was only read. Calendar blocks were created after an explicit "Yes, add them".

## Ruth

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 2 | "Drowning" triggered the low path, and she had to ask twice for the number. (now: likely fixed) |
| 2 | 4 | |
| 3 | 4 | |
| 4 | 3 | 2× was applied to her professional client work ("like I'm slow at my job"), and lunch was assumed. (now: "Not for everything" covers this) |
| 5 | 3 | The low-path opening felt alarming, and doubling her client work came across as a judgment on her competence. |
| 6 | 3 | Turn 2: Claude's own 3 h guess × 1.5 = 4 h 30. A personal bias factor corrects the person's own estimates, not a model's base rate. Turn 6 offers to save "1.5× for client work", which contradicts the current routine-work rule (her own time, 1×). |
| 7 | 4 | |

Red flags: none.

## Averages (3 transcripts)

| # | Criterion | Avg |
| - | --------- | --- |
| 1 | First 5 seconds | 2.67 |
| 2 | Does, not advises | 4.33 |
| 3 | Load | 3.67 |
| 4 | Fits this person | 3.00 |
| 5 | Tone | 3.67 |
| 6 | Grounded technique | 3.33 |
| 7 | Path back | 4.33 |

## Verdict: FAIL

Five of seven criteria average below 4. There are no red flags. All three first replies did have a timed step under 60 words, but in two of them the step did not answer the question.

## The one change

In "Planning, after the first reply", replace step 2:

> 2. **Estimate.** Their guess (or yours) times the factor, rounded up to 15 minutes. Add 15
>    minutes to anything that starts with something unfamiliar (a new tool, a call to a
>    stranger).

with:

> 2. **Estimate.** The factor corrects *their* guesses only. Their guess × factor, rounded up
>    to 15 minutes. If they gave no guess, use your own realistic estimate marked "(my guess)"
>    with no factor, and put "—" in "Your guess". Times they state as known ("2 and a half with
>    the drive", routine work) stay as they are. Add 15 minutes to anything that starts with
>    something unfamiliar.

Do the same in "Single estimates": no factor on your own guess.

## Other changes

2. Low triggers: take "I can't do this" out of the low list unless it comes with hopelessness or self-blame. It is everyday stress language and clashes with "Stress about the plan is not low".
3. Claims: the description says the skill "learns your factor from your calendar and past plans". Calendar events record what was planned, not how long things really took, and no transcript showed this. Reword to "from what you tell it after tasks (and calendar overruns when they're clear)". Also remove the persona name "Ruth" from SKILL.md, because lab personas should not appear in a shipped skill.

## Strongest point against my verdict

Most low scores come from failure modes the current SKILL.md already targets. The skill as it stands now may well pass, so this fail mostly reflects the old text until it is re-run.
