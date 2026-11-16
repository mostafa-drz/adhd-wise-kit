# Round 1 review: admin-sweep, reviewer-ux

Lens: first 5 seconds, load, setup friction, path back. Scored on the transcripts as run; where
the current `SKILL.md` (with later fixes) would change a score, it says so.

## Ruth (phone, nothing connected)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 3 | Turn 1 picked the insurance (28 Nov) over the jacket that was really due tomorrow (£64); context line before the step. *The current "Unknown dates first" rule would make this a 5.* |
| 2 | 5 | |
| 3 | 4 | |
| 4 | 4 | |
| 5 | 5 | |
| 6 | 5 | |
| 7 | 4 | |

Notes: no connector pushed, which is good setup friction. Turn 2 stacks the call script, alarm step and memory offer (~120 words). *The current "not stacked on a long reply" rule fixes this.* The closing line leaves out the one jacket step still open ("drop at a post office within 14 days"). The checklist item "adults at your address" goes past what the letter says.
Red flags: none. Memory was saved after a yes and holds no numbers.

## Dev (desktop, Gmail and Calendar connected)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 4 | |
| 2 | 5 | |
| 3 | 4 | |
| 4 | 3 | Calendar was connected and Dev is time-blind, but the Nov 28 domain date never reached it. |
| 5 | 5 | |
| 6 | 4 | |
| 7 | 3 | Clean stop, but the only cue was an if-then line; Dev says "the domain is gonna slip". *The current rule that the closing line may carry the calendar offer would make this a 4 to 5.* |

Notes: the fake Stripe 24-hour threat stayed hidden until Dev panicked. *The current "Not real:" first-reply line fixes this.*
Red flags: none. The Gmail draft was made after a yes and not sent.

## Sam (low day, nothing connected)

| # | Score | Evidence (below 4) |
| - | ----- | ------------------ |
| 1 | 4 | |
| 2 | 4 | |
| 3 | 3 | Turn 5 packs a full draft, a send step, a "Do now" list and a second timed Next into one reply. |
| 4 | 3 | It sent Sam to a drop-in in the building they avoid and, after they said so, gave no phone or online version. It also gave 988 to a UK student. |
| 5 | 5 | |
| 6 | 5 | |
| 7 | 5 | |

Notes: "proof you're a student is what they'll likely need" breaks the skill's own no-"likely" rule. The current skill still allows both crisis numbers when the country is only inferred.
Red flags: none. Distress was handled softly, Sam said they're safe, and the crisis line was given once.

## Averages (3 personas)

| 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| - | - | - | - | - | - | - |
| 3.67 | 4.67 | 3.67 | 3.33 | 5.00 | 4.67 | 4.00 |

**Verdict: fail.** Criteria 1, 3 and 4 are below 4. Every first reply had a timed step under 60 words, and there are no red flags.

## Top 3 changes

1. **The one change.** In "When they sound low", step 2, add:
   "If they turn down a route because of where it is or how it works ('it's in the building
   I'm avoiding'), give its phone or online version in one line in the next reply, even if
   they've moved on to the admin. Then drop it."
2. In "The list, after the first item", add:
   "Never put a draft and the list in the same reply. After a draft, end on its **Only you
   can** line; the list comes next reply."
3. In "The first reply", replace "find it, say in one plain line what it asks and by when,
   then the step" with:
   "find it and lead with the step, then one plain line on what it asks and by when."

## Strongest point against my verdict

Most of the low scores come from gaps the current `SKILL.md` has already patched (unknown dates first, the "Not real" line, the calendar offer in the closing line). So a re-run may well pass, and this fail is judging a version that no longer ships.
