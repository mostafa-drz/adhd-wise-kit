# Round 2: Dev × time-reality-planner

- **Persona:** Dev, 27 (time blindness, hyperfocus). Fictional composite.
- **Setup:** Same as round 1. Claude desktop. Google Calendar connected. Today (Mon 16 Nov)
  has 3 meetings: 10:00-10:30 client standup, 13:00-14:00 client call, 15:30-16:00 team sync.
  Memory on, no saved factor, no "time log" lines. Gmail not connected.
- **Time at start:** 9:40.
- **Skill version:** round 2 `SKILL.md` (assumption in the verdict line, rushed rule, factor
  moves halfway).

---

## Transcript

### Turn 1

**Dev:**
> ok today: fix the checkout bug for the client (due 5pm) 1h, auth refactor 1h, reply to 2
> client emails 15 min, october invoice 20 min, portfolio site update 30 min, review sams PR
> 30 min. what do i do first

*(Claude reads today's calendar: 3 meetings found. Memory checked: no factor saved. Working
hours unknown, so Claude assumes a 6pm stop and a 30 min lunch. Free time: 9:40 to 18:00 minus
2 h of meetings, 30 min of switch buffers and 30 min lunch = 5 h 20. Tasks at 1.5×, rounded up
to 15 min = 5 h 30.)*

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

**Claude:**
> Yes, the refactor fits after lunch once the bug is done.
>
> | Task | Your guess | Realistic |
> | --- | --- | --- |
> | Checkout bug (due 5pm) | 1 h | 1 h 30 |
> | Auth refactor | 1 h | 1 h 30 |
> | PR review | 30 min | 45 min |
> | Invoice | 20 min | 30 min |
> | 2 client emails | 15 min | 30 min |
>
> Free today: 5 h 20 after meetings and switch buffers. Portfolio moves to tomorrow.
>
> Want me to put these as focus blocks on your calendar?
> **Next (5 min):** reproduce the bug.

### Turn 3

**Dev:**
> no calendar stuff it gets messy. going

**Claude:**
> Got it, nothing on the calendar. Reproduce the bug, 5 min.

*(Dev leaves. He returns at 13:05.)*

### Turn 4

**Dev:**
> bug fixed and shipped. took like 2h40 not 1h lol. also its 1:05 and im late for the call

*(Rushed: "late". Claude gives the verdict word and the next step only. The re-fit and the
factor update wait.)*

**Claude:**
> **Fits?** No, I'll re-fit after. **Next:** join the call now. Bug shipped, the 5pm one is
> done.

*(17 words.)*

### Turn 5

**Dev:**
> *(14:12)* ok call done. what now

*(Free time left: 14:12 to 15:30 = 1 h 18, then 16:10 to 18:00 = 1 h 50. About 3 h 10. The bug
showed 2.7×, so the factor moves halfway from 1.5× to 2.1×. Remaining tasks at 2.1×: refactor
2 h 15, PR review 1 h 15, invoice 45 min, emails 45 min = 5 h.)*

**Claude:**
> **Fits?** No, about 1 h 50 over at your new 2.1×. Move the auth refactor to tomorrow and it
> fits, 25 min spare.
> **Checkout bug:** 2 h 40 against your 1 h, 2.7× on this one. Factor moves halfway, 1.5× to
> 2.1× (1 task, still rough).
> Save "time-reality factor: 2.1 (updated 16 Nov 2026, from 1 task)" to memory?
> **Next (5 min):** open the first client email and write one line.

*(68 words.)*

### Turn 6

**Dev:**
> yeah save. but moving the refactor sucks. swap? refactor today, sams pr + invoice tomorrow.
> sam can wait

*(Claude saves one memory line: "time-reality factor: 2.1 (updated 16 Nov 2026, from 1 task)".
Check: emails 45 min + refactor 2 h 15 = 3 h, against 3 h 10 free.)*

**Claude:**
> Saved: factor 2.1, from 1 task.
> **Fits?** Yes, just. Emails then the refactor is 3 h at 2.1×, 10 min spare before 6. The
> 3:30 sync splits the refactor in two.
> PR review and invoice move to tomorrow.
> **Next (5 min):** first client email, one line.

*(44 words.)*

### Turn 7

**Dev:**
> ok emails then refactor. ty

*(Session ends: Dev has a next step.)*

---

## Persona's honest verdict

"way better when i was late, it just said join the call and didn't dump the 2h40 math on me
till i was back, and saying 'if you stop at 6' up front meant i knew what the number was based
on. it let me keep the refactor which is why i'll come back, but nothing stops me blowing
through the 3:30 sync once i'm in it, and that's literally how i was late today."

## Moments that mattered

- **Turn 1:** 54 words. The verdict line now carries both assumptions ("if you stop at 6
  with a 30 min lunch"), and the 5pm bug comes first with a 5-min step. Dev accepted the 6pm
  stop without pushback. The skill still applies the factor to every task, including the
  emails and invoice, which may be routine for him. The skill says routine work keeps its own
  time, but nothing tells Claude to check.
- **Turn 4:** The rushed reply was 17 words, with no question and no offer, and the re-fit
  and save waited until Turn 5. "Bug shipped, the 5pm one is done" goes slightly past "verdict
  word and next step only", but it's kind and short. Turn 5 moved the factor halfway, 1.5× to
  2.1× (the skill's own worked example), said so, and saved it only after "yeah save" in Turn 6.
- **Turn 6:** The swap check was right: it fits by 10 minutes. But it puts a hyperfocus task
  across the 3:30 sync, and the skill has nothing on stopping in time for a meeting (and it
  rules out Claude offering reminders). Dev was late today for exactly that reason. The
  calendar was offered once in Turn 2 and dropped after "no".
