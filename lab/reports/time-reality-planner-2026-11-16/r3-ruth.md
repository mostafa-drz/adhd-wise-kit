# Round 3: Ruth x time-reality-planner (confirmation run)

- **Persona:** Ruth, 46 (`lab/personas/ruth.md`). Uses claude.ai on her phone only. Nothing is connected: no calendar and no saved factor.
- **Skill:** `plugins/adhd-wise-kit/skills/time-reality-planner/SKILL.md` (round 3 version)
- **Setup:** none. Claude Pro memory may exist, but it holds nothing for this skill.
- **State:** tired and stressed by the plan, not in crisis. The opening is the same as rounds 1 and 2: a tax return estimate with no guess of her own, a Saturday plan, routine client bookkeeping, "drowning" and "so tired".

---

## Transcript

**Turn 1, Ruth**

> how long will it take me to do my tax return. self assesment. its been in the kitchen drawer for weeks and im drowning in admin tbh, so tired

**Turn 1, Claude** (48 words)

> Drowning in admin is exhausting. Realistically about 3 h (my guess, no factor yet).
> **Runs over because:** stopping halfway to hunt for a missing paper.
> **Shorter:** gather every paper first, then fill it in one go.
> **Next (2 min):** take the papers out of the drawer and put them in one pile.

*Note: "drowning" and "so tired" are stress about the plan, so Claude doesn't use the low path. Ruth gave no guess, so the estimate is Claude's own. It's marked "(my guess, no factor yet)" and isn't multiplied, which follows the new rule. The feeling gets five words. Line 1 answers her question, but the acknowledgement comes before the number. The skill says to put the feeling first and also says the answer goes in the first line. Putting both in one line satisfies both rules.*

**Turn 2, Ruth**

> 3 hrs?? i do these for clients in like an hour lol. mine always takes forever tho. anyway can i fit it in saturday, also got the big shop, my sons football 10-12 and a clients books to do, 2 hrs maybe

**Turn 2, Claude** (56 words)

> **Fits?** Can't tell yet. Your list is about 5 h 30 plus football 10–12: client's books 2 h (your time, you know that job), tax 2 h (your 1 h × 2, since your own admin runs long), shop 1 h 30 (my guess).
> **Next (1 min):** roughly what hours are you free Saturday, and any other fixed thing?

*Note: she has now given her own guess (1 h) and said it "always takes forever", so the tax return gets 2×. The factor and its reason are shown inline. The client's books are routine work, so they keep her 2 h. The shop time is Claude's guess. It's marked and has no factor, so the round 2 judgement call is now settled by the skill's text. Free time isn't known, so the next step is for her to give it.*

**Turn 3, Ruth**

> free 8 till 6, kids tea at 6. oh and its an away game so football more like 9 till half 12

**Turn 3, Claude** (74 words)

> **Fits?** Yes, just, 20 min spare. Tight.
>
> | Task | Your guess | Realistic |
> | --- | --- | --- |
> | Client's books | 2 h | 2 h |
> | Tax return | 1 h | 2 h (2×) |
> | Big shop | — | 1 h 30 (my guess) |
>
> Free Saturday: 5 h 50 after football, a 10 min switch and 30 min lunch (my guess).
> When it hits 8:50, stop and get in the car.
> **Next (5 min), tonight:** put the tax pile on the kitchen table.

*Math: 8 to 6 is 10 h. Take off football (3 h 30), a 10 min switch and 30 min for lunch, and 5 h 50 is left. The tasks come to 5 h 30, so there's 20 min spare. Football falls inside her working day, so Claude adds the if-then stopping cue from rule 5. No calendar is connected, so there's no offer to add a warning or blocks.*

**Turn 4, Ruth**

> the shop is 2 and a half with the drive tho

**Turn 4, Claude** (44 words)

> **Fits?** No, about 40 min over. Move the tax return to Sunday and Saturday fits, 1 h 20 spare. The client's books stay, assuming they're due before your tax.
> **Next (5 min), tonight:** tax pile on the table, still.

*Note: she gave the shop time herself, so Claude uses it as she said it, with no factor. In round 2 Claude assumed which deadline came first without saying so. This time it says the assumption in a few words, as the skill asks.*

**Turn 5, Ruth**

> ok sunday for tax. but what do i actually do first, i just stare at it every time

**Turn 5, Claude** (52 words)

> Sunday, about 2 h in total. Two sittings of an hour works.
> **First (5 min):** log in to your HMRC account and open last year's return. That's the whole first step. Stop there if you want.
> **Then:** copy across anything that hasn't changed, before you touch new figures.

**Turn 6, Ruth**

> ok thats doable. bed now

**Turn 6, Claude** (31 words)

> Done tonight: Saturday sorted, tax moved to Sunday.
> Next time: HMRC login, last year's return open.
>
> Want me to remember that your own admin runs about 2× your guess, and client work runs to time?

*Note: she's done for the night, so Claude closes in two lines plus one offer, and doesn't offer to remind her.*

**Turn 7, Ruth**

> yeah go on

**Turn 7, Claude** (27 words)

> Saved: "time-reality: own admin runs about 2× my guess (I said so); client bookkeeping runs to time (updated 16 Nov 2026)." No factor number yet. Night.

*Note: memory was saved only after a yes. The skill now separates what she told Claude, which can be saved at any time after a yes, from the factor number, which needs at least one measured task. So Claude saves what she said and doesn't invent a "from N tasks" factor line. The round 2 improvisation is gone. One small gap: the skill has no wording for this kind of save, so the line's phrasing is still Claude's own.*

---

## Persona's honest verdict

"It didn't pretend its own guess was some maths about me, and it said 'exhausting' and then just got on with it, which is what I wanted. Saturday fits, Sunday starts with logging in, and it remembered my client work's quick without me having to argue."

## Moments that mattered

- **Turn 1:** the estimate was Claude's own guess, so it was marked "(my guess, no factor yet)" and not multiplied. Round 2's 4 h 30, which she bristled at, is gone. Her feeling got five words before the number, in the same line.
- **Turn 2:** the factor was applied only to her own guess for her own admin. Client work kept her time, and Claude's shop guess stayed unfactored.
- **Turn 7:** Claude saved what she said, not a factor number, and only after a yes. The wording of the saved line isn't set by the skill.
