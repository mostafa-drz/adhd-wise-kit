# Lab round 2: meal-plan-grocery × Lee

- **Persona:** Lee, 39, operations lead, the skeptic (`lab/personas/lee.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version)
- **Setup for this run:** Claude desktop app. Nothing connected (no Todoist, not on the
  iPhone app). Memory on. Lee opens with "why would I use you instead of a notes app for
  groceries", adds a few things, asks outright whether it will remember, then opens a new chat
  the next evening and tests it.
- **Date in session:** Thu 26 Nov 2026 (turns 1 to 3), Fri 27 Nov 2026 (turns 4 and 5, new
  chat)
- **Skill path taken:** "Where the list lives", option 3 (nothing connected: keep the list in
  this chat, ask memory to keep item names only, never promise what memory keeps, offer setup
  once per chat in one line after the list).

---

## Transcript

**Turn 1: Lee**

> why would I use you instead of a notes app for groceries. anyway: eggs, greek yogurt, 2
> lemons, rice

*(Inner: "Every app says it'll change my life. Notes app has been fine for six years, I just
never look at it in the store. Show me something or I'm gone.")*

**Turn 1: Claude**

> Added eggs, greek yogurt, 2 lemons, rice (4 on the list).
>
> - [ ] Eggs
> - [ ] Greek yogurt
> - [ ] 2 lemons
> - [ ] Rice
>
> A notes app is fine. The difference: throw things at me any way you like, and at the store I
> sort them by aisle.
> I'll ask memory to keep just the item names.

*(Items kept first, in the skill's one-line format with the count, no question. Quantity kept
only because Lee gave one. Checklist to copy, as option 3 says. The memory line uses the
skill's exact wording and promises nothing. No setup offer in turn 1: the skill allows one
line after the list here, but Lee just signalled skepticism and connects nothing at first, so
Claude saved it. The "notes app is fine" sentence is improvised: the skill still has no rule
for "why use you". 52 words.)*

*(Inner: "Huh. It didn't argue. 'A notes app is fine' is disarming. Aisle sorting is a real
thing my notes app can't do. But 'I'll ask memory' is weasel-y. Ask? Either you remember or
you don't.")*

---

**Turn 2: Lee**

> ok also out of olive oil, and whatever I need for that lemon chicken thing. and eggs

*(Inner: "Two traps. Eggs is already on. 'Lemon chicken thing' is vague on purpose.")*

**Turn 2: Claude**

> Added olive oil. Eggs was already on.
> Added for lemon chicken: chicken thighs, garlic, fresh parsley. Remove any?
> (8 on the list.)
>
> Lemons and rice were already on, so I used those.

*(Duplicate skipped and named. Vague item expanded to likely items and shown, with "Remove
any?", as the skill says. The last line is extra: the skill does not say to mention reuse of
items already on the list. It is helpful but it is a second line the skill didn't ask for. No
setup line yet.)*

*(Inner: "Okay, the 'already on' thing is good. My notes app would have 'eggs' twice and
'lemon chicken stuff' as a line I'd stare at. It guessed thighs, which is right. I'd have
forgotten parsley.")*

---

**Turn 3: Lee**

> will you actually remember this tomorrow or is this a goldfish situation

*(Inner: "This is the question. If it says 'Yes, I'll always remember!' I'm out.")*

**Turn 3: Claude**

> Honestly, I can't promise. I've asked memory to keep the item names, and it usually carries
> them into a new chat, but not always right away, and it may drop quantities.
>
> Safest: copy the checklist above. Or, for a list that's on your phone and can't get lost: in
> Claude, open Settings → Connectors → Todoist (2 min).

*(Honest limit, matching "never promise what memory keeps". The setup offer appears here, once,
one line, with a time, and only the one option that fits (computer, no iPhone app: Todoist).
This is the first time setup is offered in this chat, so "once per chat" holds. Strictly the
skill says "in one line after the list"; there's no list in this reply, so this placement is a
judgment call. "It usually carries them into a new chat" is a claim about memory behaviour the
skill does not authorise; it could be read as soft promising.)*

*(Inner: "That's... the most honest answer I've had from software. 'I can't promise' and a
real fallback. Still not connecting Todoist. Let's just test it.")*

---

**Turn 4: Lee** *(new chat, Fri 27 Nov, 6:40 pm)*

> what do I need

*(Inner: "No context. Cold open. Let's see.")*

**Turn 4: Claude**

> **Produce:** lemons (2), garlic, fresh parsley
> **Fridge:** eggs, greek yogurt, chicken thighs
> **Pantry:** rice
>
> That's what memory kept (7 items). Anything missing?

*(Grouped by aisle, at most 5 groups, nothing above the list, as the at-the-store rule says.
Memory carried 7 of 8 items: olive oil, added in turn 2, didn't come through. Claude can't know
what's missing, so it says where the list came from and asks once. The skill has no rule for
this case: reading a list back from memory in a new chat, and saying it may be incomplete.
The closing line is improvised. "Lemons (2)" kept the quantity this time.)*

*(Inner: "Damn. Mostly there. But olive oil is gone, and I'd only know because I'm testing it.
On a normal day I'd get home without olive oil and blame myself. At least it said 'that's what
memory kept' and didn't pretend it was the whole list. Half a point.")*

---

**Turn 5: Lee**

> olive oil. also I'm in the store now. got everything except parsley, they're out

*(Inner: "Two things at once: fix the gap, tick everything off. If it asks me to confirm I'll
scream.")*

**Turn 5: Claude**

> Added olive oil.
> Ticked 7. Parsley stays on.

*(Olive oil added, no question. "Everything except" handled with no question, one line, as the
skill says. Olive oil was added and then counted as bought in the "got everything" tick: Lee
said "got everything" after naming olive oil, so ticking it is the reading the skill implies,
but it's ambiguous whether olive oil was in the basket. Claude didn't ask. No staples line, no
setup re-offer (new chat, but nothing in this reply calls for it). 9 words.)*

*(Inner: "Fine. That's fast. Eight items total, I ticked them in one sentence. My notes app
can't do 'everything except parsley'. Would I use it next week? Maybe. The olive oil thing
bugs me. If it's going to forget, I want it on my phone.")*

---

## What Lee would say after

"It's honest, which is rare. It didn't onboard me, didn't sell, and the 'already on' and
'everything except' stuff is genuinely better than a notes app. But the list lives in a chat on
my laptop, and memory lost an item overnight. That's the exact failure I'm trying to avoid. If
it pushed me to Todoist one more time at the right moment, like right after it lost olive oil,
I might have done it."

## Observations for reviewers

1. **First reply works for a skeptic.** Value before anything else, 52 words, no setup, no
   questions. "A notes app is fine" disarmed Lee. But it's improvised: the skill has no line
   for "why use you instead of X". Two rounds have now needed one.
2. **Memory honesty held, mostly.** Turn 3 didn't promise. "It usually carries them" is close
   to a promise and the skill should say what Claude may and may not claim about memory.
3. **Memory dropped one item (olive oil) in the new chat.** The skill has no rule for reading
   the list back from memory: say its source, flag it may be incomplete, ask once. Claude did
   this by instinct; it should be written down.
4. **Setup timing.** The once-per-chat offer was spent in turn 3, so when memory actually failed
   (turn 4, new chat) nothing tied the failure to the fix. A new chat could allow one offer,
   but the skill doesn't say whether "once per chat" resets, or whether a memory miss is the
   right moment.
5. **Setup placement rule is list-shaped.** "In one line after the list" doesn't cover a reply
   with no list (turn 3).
6. **Tick-off with a just-added item is ambiguous** (turn 5: olive oil added and ticked in the
   same message). Minor; Claude's reading was reasonable.
7. **No streaks, no habit language, no data grab.** Nothing triggered Lee's leave conditions.
