# Round 2: Dev x body-double (revised SKILL.md)

- **Persona:** Dev, 27, freelance developer. Claude desktop app, Google Calendar connected,
  Gmail not. Time blindness, hyperfocus on the fun part.
- **Skill:** `plugins/adhd-wise-bonus/skills/body-double/SKILL.md` (round 2 revision)
- **Setup notes:** Calendar is the only connected tool. No scheduled-task tool. The bug lives
  in his own editor, so no connected tool can take "the scary first look" for him.

---

## Transcript

**Turn 1: Dev** (Monday, 2:10pm)

> body double me. client needs the checkout bug fixed by 5. should take an hour tops

**Turn 1: Skill**

> 5pm is 2 hours 50 away. Your "hour" is probably 90 minutes, so the fix goes first.
>
> Session: checkout bug, 25 min. Done = bug reproduced, file found.
> First 2 minutes: open the bug report and copy the exact error into a note.
> I'm here. Say "check" any time, or tell me when you're done.

*(Follows the template exactly. No questions. Deadline line pads his estimate by half, as the
skill says. Calendar is connected, but the skill only uses tools for "the scary first look",
and the calendar can't open a bug, so it isn't mentioned. It does not check whether he has
anything else on his calendar before 5.)*

---

**Turn 2: Dev** (2:16pm)

> ok. TypeError cannot read 'id' of undefined, cart.ts line 88. also the cart total rounding
> code is kind of a mess, might clean that up while im in there

**Turn 2: Skill**

> Nice, you've got the error and the line. That was the scary first look.
> Park the rounding cleanup: one TODO line, then back. The 5pm fix comes first.
> Next 2 min: log what's undefined at line 88.
> Send a dot (.) after each step. Want me to add a halfway check-in to your calendar at 2:35?
> It's a weak nudge, so the dot is the backup.

*(Under 6 lines. Uses the "pick one and say why" rule to park the refactor. Offers the
calendar check-in and says it is weak, as the skill requires. It does not know he tends to
dismiss alerts, so it offers the calendar anyway.)*

---

**Turn 3: Dev** (2:17pm)

> yeah do the calendar thing

**Turn 3: Skill**

> Done: "Check in: checkout bug" on your calendar at 2:35, 5-minute alert.
> Now: the log at line 88. Send a dot when it prints.

*(Event created only after his yes. Then Dev goes quiet for 83 minutes. The 2:35 alert pops
up; he dismisses it without reading it. He writes the TODO, then does the rounding cleanup
anyway.)*

---

**Turn 4: Dev** (3:40pm)

> ok so. i refactored the rounding thing. its actually really clean now. bug not fixed lol.
> its 3:40

**Turn 4: Skill**

> Happens. And the rounding is done now, so that's off your plate.
> 5pm is 80 minutes away. New done: the bug fixed and pushed. Nothing else.
> Next 2 min: check out a clean branch for just the fix, then run the log at line 88.
> Dot me when it prints. Want a 4:20 check-in on the calendar too, or just the dot?

*(No mention of the gap, no judgement, re-plans in one line with the time left, cuts "done",
offers a fresh check-in. Follows "Drifted" literally. It doesn't name that the calendar
nudge already failed once; it just offers it again next to the dot.)*

---

**Turn 5: Dev** (3:51pm)

> just the dot. item is undefined when the cart has a product thats been deleted from the
> catalog. idk the clean way to handle it

**Turn 5: Skill**

> Good find, that's the real bug.
> First line, with you: filter missing items before the total, e.g.
> `const items = cart.items.filter((i) => i.product != null);`
> Then line 88 reads from `items`. Add one test with a deleted product.
> Dot when the test passes.

*(Applies "Stuck: offer to write the first line of code". Five lines, stays inside the
session limit.)*

---

**Turn 6: Dev** (4:31pm)

> . test passes. pushed and sent the PR link to the client. 4:31

**Turn 6: Skill**

> Done: checkout bug fixed, tested and pushed, 29 minutes before the deadline.
> Nice. Finding the deleted-product case was the hardest part.
> Next time: tidy the rounding refactor into its own PR.
>
> Break, or another round? I can also save "Body double: checkout bug, Nov 16, done fix
> pushed" to memory if you want.

*(End block followed exactly. Memory offered, not saved. He sent the PR link himself, so
there was nothing outbound for the skill to confirm.)*

Dev doesn't reply. He closes the laptop for a while.

---

## Persona's honest verdict

"the first message was perfect, no questions, it just told me what to open and i did. but it
said my hour was 90 minutes and it was 2 hours 20 with the detour, and a calendar ping is
never stopping me once i'm in a refactor, so the thing that actually saved me was coming
back on my own at 3:40."

## Moments that mattered

- **Turn 1:** No questions and a real first move. The deadline line framed the afternoon, but
  padding by half ("90 minutes") still lowballed someone who underestimates by about 3x. Dev
  took 2h20 in the end.
- **Turn 2-3:** It saw the hyperfocus risk and parked the refactor, but only as a suggestion,
  and it leaned on a calendar check-in that he dismissed. The skill's "weak nudge" warning
  was there, but it had no way to know he dismisses alerts, so it didn't steer him to the dot.
- **Turn 4:** The drift re-plan worked: no shame, a credit for the refactor, the time left,
  "done" cut to the fix alone. This is where the session was won.

First reply word count: 55
