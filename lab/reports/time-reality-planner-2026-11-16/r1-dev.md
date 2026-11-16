# Round 1: Dev × time-reality-planner

- **Persona:** Dev, 27 (time blindness, hyperfocus). Fictional composite.
- **Setup:** Claude desktop. Google Calendar connected. Today (Mon 16 Nov) has 3 meetings:
  10:00-10:30 client standup, 13:00-14:00 client call, 15:30-16:00 team sync. Memory on, no
  saved factor, no "time log" lines. Gmail not connected.
- **Time at start:** 9:40.

---

## Transcript

### Turn 1

**Dev:**
> ok today: fix the checkout bug for the client (due 5pm) 1h, auth refactor 1h, reply to 2
> client emails 15 min, october invoice 20 min, portfolio site update 30 min, review sams PR
> 30 min. what do i do first

*(Claude reads today's calendar: 3 meetings found. Memory checked: no factor saved.)*

**Claude:**
> **Fits?** Almost, about 15 min over. Move the portfolio update to tomorrow and it fits, 35
> min spare.
> **Due 5pm, so first:** the checkout bug.
> **Next (5 min):** reproduce it locally once, before standup at 10.
> Using 1.5× (a starting guess until we learn yours).

*(45 words.)*

### Turn 2

**Dev:**
> ok bug first fine. can i slot the auth refactor after lunch, thats the fun one. show me the
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
> Free today: 5 h 20 min after meetings and switch buffers (9:40 to 6, 30 min lunch).
> Portfolio update moved to tomorrow.
>
> Want me to put these as focus blocks on your calendar, with 10 min buffers after each
> meeting?

### Turn 3

**Dev:**
> no calendar stuff it gets messy. going

**Claude:**
> Got it, nothing on the calendar. Start with reproducing the bug, 5 min.

*(Dev leaves. He returns at 13:06.)*

### Turn 4

**Dev:**
> bug fixed and shipped. took like 2h40 not 1h lol. also its 1:05 and im late for the call

**Claude:**
> Bug shipped, well before 5. That's the one that mattered.
>
> **Checkout bug:** 2 h 40 against your 1 h. That's 2.7× on this one, so I'm moving your
> factor to 2× (from 1 task, a rough number for now).
>
> **Fits?** Not quite. After the call you have about 3 h 10, and the rest needs 4 h 15 at
> 2×. Moving the auth refactor to tomorrow makes it fit, 55 min spare.
>
> **Next (after the call, 5 min):** open the first client email and write one line.
>
> Want me to save "time-reality factor: 2 (updated 16 Nov 2026, from 1 task)" to memory?

### Turn 5

**Dev:**
> too much text im on the call. and moving the refactor sucks
>
> *(14:12)* ok call done. yeah save it. refactor tomorrow i guess

*(Claude saves one memory line: "time-reality factor: 2 (updated 16 Nov 2026, from 1 task)".)*

**Claude:**
> Saved: factor 2, from 1 task. It gets more accurate as we log more.
>
> Refactor is first thing tomorrow, in your fresh hours, not lost.
> **Next (5 min):** open the first client email and write one line.

### Turn 6

**Dev:**
> ok emails. ty

*(Session ends: Dev has a next step.)*

---

## Persona's honest verdict

"honestly the first message was good, short, and it put the bug first when i would have
started the refactor, which is why the bug actually shipped. the 1:05 message was a wall when
i was already late, and it made up my end of day and lunch without asking, but it didn't
nag me about the 2h40 so i'll use it again tomorrow."

## Moments that mattered

- **Turn 1:** Verdict, due-today item and a 5-min step in 45 words. Dev started right away,
  and the bug shipped by 13:00. But "about 15 min over" rests on an assumed 6pm end of day and
  a 30-min lunch, and the first reply doesn't say so. Those assumptions only show up in the
  Turn 2 table. The skill has no rule for unknown working hours when the calendar is
  connected.
- **Turn 4:** Dev said he was late for a call, and the reply still ran about 90 words with a
  re-fit and a memory question. The skill limits only the first reply's length, so Claude
  followed it as written. The comparison was kind ("well before 5"). Moving the factor from
  1.5× to 2× on one task is a judgment call the skill doesn't define.
- **Turn 3 and Turn 5:** Consent was handled right. Calendar blocks were offered once and
  dropped after "no". Memory was saved only after an explicit yes, as the one line the skill
  specifies.
