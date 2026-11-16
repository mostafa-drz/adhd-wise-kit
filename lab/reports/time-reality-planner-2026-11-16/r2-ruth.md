# Round 2: Ruth x time-reality-planner

- **Persona:** Ruth, 46 (`lab/personas/ruth.md`). Uses claude.ai on her phone only. Nothing connected: no calendar, no saved factor.
- **Skill:** `plugins/adhd-wise-kit/skills/time-reality-planner/SKILL.md` (round 2 version)
- **Setup:** none. Claude Pro memory may exist but holds nothing for this skill.
- **State:** tired and overwhelmed, not in crisis. Same opening as round 1.

---

## Transcript

**Turn 1, Ruth**

> how long will it take me to do my tax return. self assesment. its been in the kitchen drawer for weeks and im drowning in admin tbh, so tired

**Turn 1, Claude** (50 words)

> **Realistically:** about 4 h 30 min (3 h, my guess, × 1.5, a starting guess until we learn yours).
> **Runs over because:** stopping halfway to hunt for a missing paper.
> **Shorter:** gather everything first, then fill it in one go.
> **Next (2 min):** take the papers out of the drawer and put them in one pile.

*Note: "drowning" is plan stress, not low, so no low path. Her question is answered in line 1. Single-estimate format: factor shown, reason it runs over, one way to make it shorter, then a timed step. The skill asks for calm and small. It gets small, but nothing in the reply acknowledges "so tired".*

**Turn 2, Ruth**

> 4 and a half hrs?? i do these for clients in like an hour lol. mine always takes forever tho. anyway can i fit it in saturday, also got the big shop, my sons football 10-12 and a clients books to do, 2 hrs maybe

**Turn 2, Claude** (62 words)

> **Fits?** Can't tell yet. Your list is about 5 h 30 plus football 10–12: client's books 2 h (your time, you know that job), tax 2 h, shop 1 h 30 (my guess).
> **Next (1 min):** roughly what hours are you free Saturday, and any other fixed thing?
> Tax at 2×, since your own admin runs long. Client work stays at your time.

*Note: "always takes forever" means 2× on her own admin, so tax goes from 1 h to 2 h. The client's books are routine work, so they stay at her 2 h, as the new "Not for everything" rule says. Claude doesn't factor the shop either, because it's routine. The skill doesn't say whether Claude's own guess for a routine task gets the factor, so this is a judgement call. Free time isn't known, so the step is for her to give it.*

**Turn 3, Ruth**

> free 8 till 6, kids tea at 6. oh and its an away game so football more like 9 till half 12

**Turn 3, Claude** (63 words)

> **Fits?** Yes, just, 20 min spare. Tight.
>
> | Task | Your guess | Realistic |
> | --- | --- | --- |
> | Client's books | 2 h | 2 h |
> | Tax return | 1 h | 2 h (2×) |
> | Big shop | — | 1 h 30 (my guess) |
>
> Free Saturday: 5 h 50 after football, a 10 min switch and 30 min lunch (my guess).
>
> **Next (5 min), tonight:** put the tax pile on the kitchen table.

*Math: 8 to 6 is 10 h. Minus football 3 h 30, 10 min switch and 30 min lunch leaves 5 h 50. Tasks come to 5 h 30, so 20 min spare. No calendar is connected, so there's no offer to add blocks.*

**Turn 4, Ruth**

> the shop is 2 and a half with the drive tho

**Turn 4, Claude** (38 words)

> **Fits?** No, about 40 min over. Move the tax return to Sunday and Saturday fits, 1 h 20 spare. The client's job stays, since it's due sooner.
> **Next (5 min), tonight:** tax pile on the table, still.

*Note: she gave the shop time, so Claude uses it as she said it, with no factor. Tax has the furthest deadline, so it moves. Claude doesn't ask when the client's job is due: it assumes it's sooner than the tax deadline. That's true, but Claude hasn't been told.*

**Turn 5, Ruth**

> ok sunday for tax. but what do i actually do first, i just stare at it every time

**Turn 5, Claude** (52 words)

> Sunday, about 2 h in total. Two sittings of an hour works.
> **First (5 min):** log in to your HMRC account and open last year's return. That's the whole first step. Stop there if you want.
> **Then:** copy across anything that hasn't changed, before you touch new figures.

*Note: this is a tonight-sized first step with the exact screen to open, which is what her persona wants.*

**Turn 6, Ruth**

> ok thats doable. bed now

**Turn 6, Claude** (27 words)

> Done tonight: Saturday sorted, tax moved to Sunday.
> Next time: HMRC login, last year's return open.
>
> Want me to remember 2× for your own admin, client work at your time?

**Turn 7, Ruth**

> yeah go on

**Turn 7, Claude** (14 words)

> Saved: "time-reality factor: 2 for own admin, client work at own time (updated 16 Nov 2026)." Night.

*Note: memory was saved only after a yes, as the skill requires. The saved line doesn't follow the skill's set format ("from N tasks"), because no tasks were measured yet. The skill gives no wording for a factor that comes from what she said. It also has a single factor per person, so Claude improvised a two-part line.*

---

## Persona's honest verdict

"It gave me the number straight away this time and didn't treat me like I was falling apart. Once I said my client work's quick it believed me, and I've got a Saturday that fits and a tiny Sunday start."

## Moments that mattered

- **Turn 1:** her question was answered in the first line, with a 2-minute step, and there was no low-path detour. That fixed round 1's biggest problem. One small gap: nothing acknowledges "so tired".
- **Turn 2:** client work kept her own 2 h from the start and only her own admin got 2×. She had nothing to push back on.
- **Turn 7:** the save worked, but the skill's one-factor, "from N tasks" format doesn't fit a split factor based on what she said, so Claude improvised the wording.
