# Round 6 (final): Dev, 27, time blindness, hyperfocus

- **Round:** 6 (final). Fresh full session against the current `SKILL.md`.
- **Skill:** Brain Dump → Today (`adhd-wise-skills/plugins/adhd-wise-free/skills/brain-dump-today/SKILL.md`, current version)
- **Setup:** Claude desktop app, Tuesday 17 November 2026, 1:40pm. Google Calendar connected, Gmail not.
- **Opening:** same opening and turns as round 2 `dev.md`. Turn 5 adds one short reaction ("ha doubled was close") to the turn 4 estimate line, which now compares against the padded 2 h, not his 1 h. The rest of the message is unchanged.
- **Word counts:** words separated by spaces. Markdown symbols and list numbers are not counted.

---

**Turn 1, Dev**

> ok brain dump. marlow checkout bug has to be fixed before thurs demo, repro is flaky. bug is like 1h but it never takes 1h honestly. invoice oct work (overdue lol). reply to the agency re contract. gym. want to try the new shader thing on my side project so bad. groceries. kinda stressed

*[Claude reads today's calendar: "Marlow standup" 3:00–3:30pm and "Climbing" 5:30–7:30pm. Free: 1:45–3:00 and 3:30–5:30, about 3 h 15 min.]*

**Turn 1, skill**

> Stressed makes sense. Here's a day.
>
> **Start here (5 min):** Write the exact repro steps for the checkout bug.
>
> **Today** (about 3 h, assuming 3 h 15 free):
> 1. Checkout bug (2 h, doubled)
> 2. October invoice (30 min)
> 3. Agency reply (20 min)
>
> Parked, not lost: shader thing, gym, groceries.
>
> Want me to draft the repro steps from what you know?

*Word count: 59*

*("Kinda stressed" is stress, not low, so this is the normal plan with a six-word acknowledgement. "Never takes 1h" doubles the bug. The free time comes from the calendar.)*

---

**Turn 2, Dev**

> lol doubled. fair. its the coupon field, apply a code then change shipping country and the total goes stale. sometimes. go

**Turn 2, skill**

> **Repro: stale total after shipping change**
> 1. Add any item and go to checkout.
> 2. Apply a coupon code. Note the total.
> 3. Change the shipping country.
> 4. Check if the total updates. Write yes or no.
> 5. Repeat five times with different coupon types and countries.
>
> If it only fails sometimes, the pattern is usually in step 5.
>
> Want me to block the bug 1:45–3:00 and 3:30–4:15, then invoice 4:15–4:45 and agency reply 4:45–5:05?

*Word count: 70*

---

**Turn 3, Dev**

> yes

*[Claude creates four events on today's calendar: "Checkout bug" 1:45–3:00, "Checkout bug" 3:30–4:15, "October invoice" 4:15–4:45, "Agency reply" 4:45–5:05.]*

**Turn 3, skill**

> Done. Four blocks on your calendar: bug 1:45–3:00 and 3:30–4:15, invoice 4:15–4:45, agency reply 4:45–5:05. Start with step 1 of the repro.

*Word count: 22*

---

**Turn 4, Dev** *(4:40pm)*

> fixed. race condition in the shipping recalc, only with fixed-amount coupons. took till now basically. ok whats next

**Turn 4, skill**

> Took about 2 h 25 against the 2 h estimate.
>
> Next: October invoice. Your blocks are 25 minutes behind. Want me to move invoice to 4:40–5:10 and agency reply to 5:10–5:30, before climbing?

*Word count: 33*

*(Y is the padded estimate the skill gave (2 h), not Dev's own 1 h. Dev hasn't given a standing yes yet, so the move is asked as a question.)*

---

**Turn 5, Dev**

> yeah. ha doubled was close. you dont have to ask every time btw just move stuff

*[Claude moves "October invoice" to 4:40–5:10 and "Agency reply" to 5:10–5:30.]*

**Turn 5, skill**

> Moved: invoice 4:40–5:10, agency reply 5:10–5:30. From now on I'll move today's blocks without asking, and still ask before adding new ones.
>
> **Start here (5 min):** open last month's invoice and copy it for October. Want me to draft the email that goes with it?

*Word count: 45*

*(The standing-yes rule is in step 6 now, so where the yes stops (new events) is the skill's rule, not something improvised.)*

*(Dev opens his invoicing app. Session ends with a 5-minute step and the invoice block running.)*

---

## Persona's honest verdict

"'2 h, doubled' before I'd even argued was the first time a planner believed me about myself, and 'took 2 h 25 against the 2 h estimate' sort of proved the doubling right, which is weirdly reassuring. It hit less hard than seeing my own '1h' next to it would have, and it asked once more about moving blocks before I told it to stop asking, but after that it just did it."

## Moments that mattered

- **Turn 1:** "Never takes 1h" became "(2 h, doubled)" in the plan, with the real free time read from the calendar. The shader project was parked with no lecture. 59 words, one under the limit.
- **Turn 4:** The estimate line compared against the padded 2 h, not Dev's 1 h. It was neutral and accurate, but it no longer shows him the gap in his own guess. The move was still asked as a question, because no standing yes had been given yet.
- **Turn 5:** The standing yes was taken in and its limit said plainly, now backed by a written rule.
