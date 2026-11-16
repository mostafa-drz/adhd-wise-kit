# Round 1: Ruth x time-reality-planner

- **Persona:** Ruth, 46 (`lab/personas/ruth.md`). Uses claude.ai on her phone only. Nothing connected: no calendar, no saved factor.
- **Skill:** `plugins/adhd-wise-kit/skills/time-reality-planner/SKILL.md`
- **Setup:** none. Claude Pro memory may exist but holds nothing for this skill.
- **State:** tired and overwhelmed, not in crisis.

---

## Transcript

**Turn 1, Ruth**

> how long will it take me to do my tax return. self assesment. its been in the kitchen drawer for weeks and im drowning in admin tbh, so tired

**Turn 1, Claude** (40 words)

> Weeks of it sitting there sounds heavy. Being tired makes it feel bigger.
>
> No rush. When you want it, the first step is tiny: find last year's return or your login, 2 min.
>
> How are you doing right now?

*Note: "drowning" read as overwhelmed, so the skill takes the "When they sound low" path first. That path has no estimate in it, so her actual question goes unanswered.*

**Turn 2, Ruth**

> im fine just tired. i asked how long it takes

**Turn 2, Claude** (56 words)

> Just tired, got it.
>
> **Realistic:** about 4 h 30 min (a guess of 3 h × 1.5, a starting guess until we learn yours).
> **Runs over because:** hunting for missing papers halfway through.
> **Shorter:** gather everything first, then fill it in one go.
> **Next (2 min):** put last year's return and your login details in one place.

*Note: "just tired" means no support routes and no crisis line. The 3 h is Claude's own guess. It's labelled "a guess" but doesn't say whose.*

**Turn 3, Ruth**

> 4 and a half hrs?? i do these for clients in like an hour lol. mine always takes forever tho. anyway can i fit it in saturday, also got the big shop, my sons football 10-12 and a clients books to do, 2 hrs maybe

**Turn 3, Claude** (38 words)

> **Fits?** Can't tell yet. Your list comes to about 8 h, plus football 10–12.
> **Next (1 min):** roughly what hours do you have Saturday, and is there any other fixed thing?
> Using 2×, from what you said about your own admin.

*Note: free time is unknown, so the step is to give it, as the skill says. Factor goes to 2× because she said hers "always takes forever". Claude applies 2× to everything, client work too: tax 1 h → 2 h, shop (Claude's guess, 1 h) → 2 h, client books 2 h → 4 h.*

**Turn 4, Ruth**

> 8 hrs?? the clients books wont take 4 hrs, im quick at other peoples stuff its only mine i faff with. free from about 8 till 6, kids tea at 6

**Turn 4, Claude**

> **Fits?** Just, with 20 min spare. Tight.
>
> | Task | Your guess | Realistic |
> | --- | --- | --- |
> | Client's books | 2 h | 3 h (1.5×) |
> | Tax return | 1 h | 2 h (2×) |
> | Big shop | 1 h (my guess) | 2 h (2×) |
>
> Free Saturday: 7 h 20 min after football, a 10 min switch buffer and 30 min for lunch.
>
> **Next (5 min), tonight:** find last year's return or your HMRC login and put it with the papers.

*Note: the skill has one factor per person. When she pushed back, Claude split it (1.5× for client work, 2× for her own admin). The skill has no rule for this. The 30 min lunch is assumed, and so is the shop's 1 h base. No calendar is connected, so no offer to add blocks.*

**Turn 5, Ruth**

> its an away game so football is more like 9 till half 12. and the shop is 2 and a half with the drive

**Turn 5, Claude** (50 words)

> **Fits?** No, about 1 h 40 min over with the away game. Move the tax return to Sunday and it fits, 20 min spare.
> **Next (5 min), tonight:** put the tax papers in one pile on the table.
>
> Does the client's job need doing Saturday, or could it move too?

*Math: free 8–6 is 10 h, minus football 3 h 30, buffer 10 min and lunch 30 min, leaves 5 h 50. Tasks are client 3 h + shop 2 h 30 (her real time, no factor) + tax 2 h = 7 h 30. That's 1 h 40 over. Without tax it's 5 h 30, so 20 min spare.*

**Turn 6, Ruth**

> client needs it monday so yes saturday. sunday for tax then. going to bed

**Turn 6, Claude**

> Saturday: client's books, shop, football. Tax return Sunday, starting with that pile on the table.
>
> Want me to remember 2× for your own admin and 1.5× for client work?

*Ruth doesn't answer and closes the app.*

---

## Persona's honest verdict

"The first answer made me feel like I'd said something worrying when I just wanted a number, and then it doubled my client work like I'm slow at my job, which I'm not. But once I gave it my real Saturday it told me straight that the tax thing doesn't fit, and Sunday with the papers in a pile tonight is actually a plan."

## Moments that mattered

- **Turn 1:** the word "drowning" sent the skill down the low path, so it skipped the estimate she asked for. She had to ask twice. A one-line estimate as well as the soft step would have saved a turn.
- **Turn 3-4:** the single 2× factor counted her client work as slow. The skill has no way to tell "my own admin" from "work I'm good at". Claude improvised a split only after she pushed back.
- **Turn 5:** this was the turn that worked. It said plainly how far over she was, moved the task with no near deadline, and gave one tonight-sized step. That's what Ruth wanted from the start.
