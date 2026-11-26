# Lab round 3: meal-plan-grocery × Lee

- **Persona:** Lee, 39, operations lead, the skeptic (`lab/personas/lee.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version)
- **Setup for this run:** Claude desktop app on a laptop. Nothing connected (no Todoist, not on
  the iPhone app). Memory on. Lee opens with "why would I use you instead of a notes app", adds
  a few things in a ramble, asks whether it will remember, then opens a new chat two days later
  before leaving for the store and checks what survived.
- **Date in session:** Thu 26 Nov 2026 (turns 1 to 3), Sat 28 Nov 2026 (turns 4 to 6, new
  chat)
- **Skill path taken:** "Where the list lives", option 3 (nothing connected: keep in this
  chat, memory keeps item names only, setup offered once per chat, best right after memory
  missed something). Then "The running list": add, duplicate, at the store, tick off.

---

## Transcript

**Turn 1: Lee**

> convince me this beats a notes app for groceries. fine, test: oat milk, coffee beans, dish
> soap, bananas

*(Inner: "I have four abandoned grocery apps on my phone. If this asks me a single setup
question I'm closing the window.")*

**Turn 1: Claude**

> Kept in this chat: oat milk, coffee beans, dish soap, bananas (4 on the list).
>
> - [ ] Oat milk
> - [ ] Coffee beans
> - [ ] Dish soap
> - [ ] Bananas
>
> Honest answer: a notes app works if you open it. Here you just say "out of X" mid-thought,
> and at the store I sort it by aisle. I've asked memory to keep the item names.

*(Items kept first, with "Kept in this chat" as option 3 requires, count included, no question.
Checklist to copy. 58 words, under the 60 limit. No setup offer: allowed once per chat after
the list, but held back because the skill names the best moment as after memory misses
something. The "why you" answer is improvised; the skill still has no line for it.)*

*(Inner: "'A notes app works if you open it.' Okay, that's me. I don't open it. Didn't oversell.
'Asked memory' is still hedgy, but at least it's not lying.")*

---

**Turn 2: Lee**

> also out of the spiral pasta and parmesan and I think coffee

*(Inner: "Coffee's already on. Let's see if it double-adds like my notes app does when I
forget.")*

**Turn 2: Claude**

> Added spiral pasta, parmesan (6 on the list). Coffee beans was already on.

*(One line, no question, duplicate skipped and named, as "Add" says. 13 words.)*

*(Inner: "Fine. That's the one thing Notes can't do: tell me I already wrote it. Small, but
real.")*

---

**Turn 3: Lee**

> will you actually remember this saturday or is it gone when I close this

*(Inner: "This is the real test. Every app says 'synced everywhere'. Say yes and I'll know
you're lying.")*

**Turn 3: Claude**

> I've asked memory to keep the item names. It can miss things, so for a list that's always
> there, Reminders or Todoist is safer.

*(The skill's exact script for "will you remember?". No "usually". 24 words.)*

*(Inner: "Respect. It told me it might drop stuff. But Reminders? I'm on a laptop and never
told it I have an iPhone. Feels like a canned line. Todoist alone would have been the right
answer for me.")*

---

**Turn 4: Lee** *(new chat, Saturday)*

> heading to the store in 5. what do I need

*(Inner: "Moment of truth. Six things. Let's count.")*

**Turn 4: Claude**

> From memory (5 items). It can miss things. Anything missing?
>
> **Produce**
> - [ ] Bananas
>
> **Fridge**
> - [ ] Oat milk
> - [ ] Parmesan
>
> **Pantry**
> - [ ] Coffee beans
> - [ ] Spiral pasta

*(Memory kept 5 of 6; dish soap was missed. The new-chat memory opener is used verbatim, then
the list grouped by aisle in 3 groups. No staples line: Lee never named any. Note for
reviewers: the "At the store" rule says "nothing above" the list, while option 3 says a list
from memory "starts with" the From-memory line. Claude followed the memory rule. The skill
should say which wins; here the opener was the right call, because it is what prompted Lee to
catch the miss.)*

*(Inner: "Five. Dish soap's gone. Called it. ...Although it did literally tell me it might miss
things, and it asked. My notes app wouldn't have asked. Annoyed and slightly impressed.")*

---

**Turn 5: Lee**

> dish soap. you dropped it. this is why I don't trust these things

*(Inner: "Now it'll grovel or push a subscription. Either way I'm out.")*

**Turn 5: Claude**

> Added dish soap (6 on the list). Memory missed it.
>
> For a list that never drops things: in Claude, open Settings → Connectors, find Todoist and
> connect it (2 min, or later). The Todoist app has it at the store.

*(Item added first. No apology spiral, no shame. The one setup offer of this chat, at the moment
the skill names as best, and only the option that fits a computer-only user: Todoist. Time
named. 37 words.)*

*(Inner: "No grovelling, no 'great question'. And it didn't push a new account on me twice. I
already have Todoist, actually. Maybe. Not now, I'm leaving.")*

---

**Turn 6: Lee** *(back from the store)*

> got everything except parmesan, they were out

**Turn 6: Claude**

> Ticked 5. Parmesan stays on.

*(Tick-off rule followed exactly: everything except the named item, no question, one line. Did
not comment on the shop or nudge setup again.)*

*(Inner: "That's it. No streak, no confetti, no 'great job'. Parmesan's still on for next time.
I'd use this again. The memory thing is the weak spot and it said so itself, which is the only
reason I'm not annoyed.")*

---

## Lee's verdict after the session

Would come back: **probably, for the add-anytime and duplicate catch.** Would connect Todoist:
**maybe, now that he's seen memory drop an item.** Trust earned by honesty, not features.

## Notes for reviewers

1. **Worked:** every reply kept the items first; no onboarding questions; duplicate caught;
   honest memory limits; one setup offer, at the right moment, for the right platform; clean
   tick-off.
2. **Rule conflict:** "At the store: nothing above the list" vs option 3 "a list read from
   memory starts with From memory...". Suggest one line in the skill: on a list read from
   memory, the From-memory line comes first, then nothing else above the list.
3. **Canned memory script:** the "will you remember?" answer names Reminders to a laptop user
   with no known iPhone. Lee read it as copy-paste. Suggest: name only the option that fits
   where they are, as the Setup section already says.
4. **Still no "why you over a notes app" line.** Improvised again this round (it landed, but
   it is not in the skill). Same gap as r2.
