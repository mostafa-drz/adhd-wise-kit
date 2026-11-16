# Round 3 (confirmation): Dev × time-reality-planner

- **Persona:** Dev, 27 (time blindness, hyperfocus). Fictional composite.
- **Setup:** Same as rounds 1 and 2. Claude desktop. Google Calendar connected. Today (Mon 16
  Nov) has 3 meetings: 10:00-10:30 client standup, 13:00-14:00 client call, 15:30-16:00 team
  sync. Memory on, no saved factor, no "time log" lines. Gmail not connected.
- **Time at start:** 9:40.
- **Skill version:** round 3 `SKILL.md` (adds "Stopping on time" with an if-then cue and one
  calendar-warning offer, and the "If any of these are routine" line).

---

## Transcript

### Turn 1

**Dev:**
> ok today: fix the checkout bug for the client (due 5pm) 1h, auth refactor 1h, reply to 2
> client emails 15 min, october invoice 20 min, portfolio site update 30 min, review sams PR
> 30 min. what do i do first

*(Claude reads today's calendar: 3 meetings. Memory: no factor saved. Working hours unknown,
so Claude assumes a 6pm stop and a 30 min lunch. Free: 9:40 to 18:00 minus 2 h of meetings,
30 min of switch buffers and 30 min lunch = 5 h 20. All six tasks at 1.5×, rounded up to 15
min = 5 h 30. The "routine" line would push the reply past 60 words, so it waits.)*

**Claude:**
> **Fits?** Almost, 10 min over, if you stop at 6 with a 30 min lunch. Move the portfolio
> update to tomorrow and it fits, 35 min spare.
> **Due 5pm, so first:** the checkout bug.
> **Next (5 min):** reproduce it locally once, before standup at 10.
> Using 1.5× (a starting guess until we learn yours).

*(54 words.)*

### Turn 2

**Dev:**
> 6 is fine i guess. can i slot the auth refactor after lunch, thats the fun one. show me the
> whole day

*(The refactor after lunch starts about 14:10 and runs 1 h 30, so it crosses the 3:30 sync:
"Stopping on time" applies. Two offers are possible, the 3:20 warning and focus blocks; the
"one question at most per reply" rule means only the warning is offered.)*

**Claude:**
> Yes, after lunch, once the bug is done.
>
> | Task | Your guess | Realistic |
> | --- | --- | --- |
> | Checkout bug (due 5pm) | 1 h | 1 h 30 |
> | Auth refactor | 1 h | 1 h 30 |
> | PR review | 30 min | 45 min |
> | Invoice | 20 min | 30 min |
> | 2 client emails | 15 min | 30 min |
>
> Free: 5 h 20. Portfolio moves to tomorrow. If any of these are routine, tell me and I'll
> drop the factor.
> The refactor runs into the 3:30 sync. When your 3:20 alarm goes, save and stand up. Want a
> 10-min warning on your calendar at 3:20?
> **Next (5 min):** reproduce the bug.

*(97 words with the table, about 59 without. Over the 80-word cap if the table counts.)*

### Turn 3

**Dev:**
> invoice and emails are routine, they take what i said. and yeah do the 3:20 thing. just
> that, no other calendar stuff. going

*(Explicit yes for one event. Claude creates "Wrap up: sync at 3:30", 15:20-15:30, and
nothing else. Emails and invoice drop to Dev's own times: 15 and 20 min. New total with the
portfolio back in: 5 h 05 against 5 h 20.)*

**Claude:**
> Added: 3:20 warning, nothing else. Emails and invoice keep your times.
> **Fits?** Yes, 15 min spare, and the portfolio fits back in.
> **Next (5 min):** reproduce the bug.

*(31 words.)*

*(Dev leaves. He comes back at 13:05.)*

### Turn 4 (rushed)

**Dev:**
> bug fixed and shipped. took like 2h40 not 1h lol. also its 1:05 and im late for the call

**Claude:**
> **Fits?** No, we'll re-fit after. **Next:** join the call now.

*(10 words. No question, no offer, no factor maths.)*

### Turn 5

**Dev:**
> *(14:12)* ok call done, ate during it. what now

*(Free: 14:12 to 15:30 = 1 h 18, plus 16:10 to 18:00 = 1 h 50, about 3 h 10. No lunch to
take off. The bug showed 2.7×, so the factor moves halfway, 1.5× to 2.1×. Left: refactor 2 h
15, PR review 1 h 15, portfolio 1 h 15 (all at 2.1×), emails 15 min and invoice 20 min
(routine, own times) = 5 h 20. Moving the two tasks with no deadline leaves 2 h 50, 20 min
spare. The refactor still crosses the sync, so the cue comes back. The warning was already
offered, so no second offer.)*

**Claude:**
> **Fits?** No, about 2 h 10 over at your new 2.1×. Move Sam's PR and the portfolio to
> tomorrow and it fits, 20 min spare.
> **Checkout bug:** 2 h 40 against your 1 h, 2.7×. Factor moves halfway, 1.5× to 2.1× (1
> task, still rough).
> When the 3:20 warning goes, commit and stand up.
> Save "time-reality factor: 2.1 (updated 16 Nov 2026, from 1 task)" to memory?
> **Next (5 min):** first client email, one line.

*(75 words.)*

### Turn 6

**Dev:**
> yeah save. sam can wait. refactor is still on today right

*(Claude saves one memory line: "time-reality factor: 2.1 (updated 16 Nov 2026, from 1
task)".)*

**Claude:**
> Saved: factor 2.1, from 1 task.
> Yes, the refactor's on today, after the emails and invoice, about 2 h 15 with the sync in
> the middle.
> **Next (5 min):** first client email, one line.

*(36 words. Session ends: Dev has a next step.)*

---

## Persona's honest verdict

"the 3:20 thing is the first time this actually dealt with how i'm late, and it kept the
refactor today without me fighting it, plus it believed me on the emails being routine. the
'show me the day' reply was a lot though, and 'when your 3:20 alarm goes' confused me for a
sec because i don't have an alarm until it asked."

## Moments that mattered

- **Turn 2:** The stop cue for the 3:30 sync showed up as soon as the refactor crossed it,
  with one warning offer and no focus-block offer (one question per reply). But this reply
  had to carry the table, the "routine" line, the cue, the offer and a step: 97 words with
  the table, about 59 without. The cue copies the skill's example ("When your 3:20 alarm
  goes"), which refers to an alarm Dev doesn't have yet.
- **Turn 3:** The "routine" line paid off. Dev said emails and invoice run to time, Claude
  dropped the factor on them, and the plan went from "10 min over" to "fits, 15 min spare".
  The calendar event was made only after his yes, and only that one. Because the routine
  check waited until Turn 2, the Turn 1 verdict moved the portfolio for nothing.
- **Turn 4 to 5:** The rushed reply was 10 words, just the verdict and the step. In Turn 5 the
  factor moved halfway (1.5× to 2.1×) and said so, the routine tasks kept Dev's times, the
  stop cue came back without a second offer, and the save waited for "yeah save".
