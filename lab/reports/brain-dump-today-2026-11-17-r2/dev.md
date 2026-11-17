# Round 2: Dev, 27, time blindness, hyperfocus

- **Skill:** Brain Dump → Today (`adhd-wise-skills/plugins/adhd-wise-free/skills/brain-dump-today/SKILL.md`, round 2 version)
- **Setup:** Claude desktop app, Tuesday 17 November 2026, 1:40pm. Google Calendar connected, Gmail not.
- **Opening:** same situation as round 1 (a client checkout bug before a demo, his "like 1h" estimate that never holds, an overdue invoice, an agency reply, a side project he wants to play with). The round 1 transcript files were not at the given path, so this opening is rebuilt from the round 1 report.
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
> **Today** (about 3 h, assuming 3 free):
> 1. Checkout bug (2 h, doubled)
> 2. October invoice (30 min)
> 3. Agency reply (20 min)
>
> Parked, not lost: shader thing, gym, groceries.
>
> Want me to draft the repro steps from what you know?

*Word count: 57*

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

> Took about 2 h 25 against your 1 h.
>
> Next: October invoice. Your blocks are 25 minutes behind. Want me to move invoice to 4:40–5:10 and agency reply to 5:10–5:30, before climbing?

*Word count: 32*

---

**Turn 5, Dev**

> yeah. you dont have to ask every time btw just move stuff

*[Claude moves "October invoice" to 4:40–5:10 and "Agency reply" to 5:10–5:30.]*

**Turn 5, skill**

> Moved: invoice 4:40–5:10, agency reply 5:10–5:30. I'll move today's blocks without asking from now on, and still ask before adding new ones.
>
> **Start here (5 min):** open last month's invoice and copy it for October. Want me to draft the email that goes with it?

*Word count: 45*

*(Dev opens his invoicing app. Session ends with a 5-minute step and the invoice block running.)*

---

## Persona's honest verdict

"'2 h, doubled' before I even said anything else is the first time a planner has believed me about myself, and 'took 2 h 25 against your 1' stung in a useful way. Being asked again to move a block I'd already said yes to was one question too many, but it learned."

## Moments that mattered

- **Turn 1:** "never takes 1h" turned into "(2 h, doubled)" in the plan itself. The shader project was parked with no lecture. Under 60 words, with the real free time read from the calendar.
- **Turn 4:** "Took about 2 h 25 against your 1 h." The one-line comparison landed. The skill then asked for consent again to move events it had already created.
- **Turn 5:** Dev gave a standing yes to moves, and the skill said where that yes stops: new events still need asking. The skill has no rule for a standing yes, so this was improvised.
