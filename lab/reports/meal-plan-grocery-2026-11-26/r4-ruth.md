# Lab round 4: meal-plan-grocery × Ruth

- **Persona:** Ruth, 46, part-time bookkeeper, phone only, not technical (`lab/personas/ruth.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 3:
  the permission line now names the button and says why)
- **Setup for this run:** Claude iPhone app. Reminders permission NOT yet granted. No list
  called Groceries, Shopping or Shopping list in Reminders. Memory off. Nothing connected.
- **Scenario:** Thu 26 Nov 2026, 7:45am. Ruth is making breakfast and notices she is out of milk
  and coffee. A few minutes later she remembers bread. About 5:20pm she is in the supermarket,
  and the app opens a new chat. Tests setup friction on a phone, then the store trip.
- **Skill route taken:** "Where the list lives" step 1 (Apple Reminders). No list and no
  access: keep the items in this chat, offer to make the list in one reply. On a yes, the
  permission line first, then make the list, move the items, then the Siri line once. Store
  view, tick-off with one item staying on, bare "k" ends the trip.

---

## Transcript

**Turn 1, Ruth (7:45am, kitchen, toast in, one thumb):**

> out of milk and cofee. put on list pls

**Turn 1, Claude:**
_(No Reminders access yet, so it cannot see any list. Per the skill: never drop the items, keep
them in this chat, offer the list in one reply with a time and a "later". No question beyond
that.)_

> Kept milk, coffee in this chat. Make a Groceries list in Reminders so they're on your phone at
> the store? (1 min, or later)

_(22 words. Items kept first, offer second, time named, "later" is a real option.)_

**Ruth, inner:**

> Fine, it has them. "1 min". Toast takes about that. If it wants a password or an account I'm
> saying later and leaving it in here.

---

**Turn 2, Ruth (7:46am):**

> yes

**Turn 2, Claude:**
_(A yes. Per the skill: say the permission line before making the list, then make it.)_

> Your iPhone will ask about Reminders. Tap the Allow button (it may say Allow Full Access); it's
> how I add to your list.

_(iPhone pop-up appears under the message: "Claude Would Like Full Access to Your Reminders",
buttons "Don't Allow" and "Allow Full Access". Ruth taps "Allow Full Access" in about two
seconds. Claude creates a list called Groceries and adds milk and coffee.)_

> Made a Groceries list in Reminders and moved milk, coffee there (2 on the list). Fastest next
> time: "Hey Siri, add eggs to Groceries."

_(23 words before the pop-up, 22 after. One tap, no typing, no account. Siri line given once,
right after the list is made.)_

**Ruth, inner:**

> It told me the button would say Full Access, and it did, so I just pressed it. No hovering
> this time. There's a tiny voice going "full access to my dentist one and the car insurance
> one too?" but it said it's how it adds to the list, so okay. I'd have liked to know I can
> turn it off again, my daughter always asks me that. Opened Reminders to check: Groceries,
> milk, coffee. Huh. That was actually one minute.

_(Setup friction is down to one tap. Remaining flicker is the word "Full" and not knowing it
can be undone. See note 1.)_

---

**Turn 3, Ruth (7:52am, same chat, buttering toast):**

> oh and bred

**Turn 3, Claude:**
_(Access granted now. Adds straight to the Groceries list. One line, no question.)_

> Added bread (3 on the list).

_(5 words. Typo cleaned without comment.)_

**Ruth, inner:**

> Didn't make a thing of my spelling. Good. That's the whole interaction I want.

---

**Turn 4, Ruth (5:20pm, supermarket entrance, trolley, the app opens a new chat):**

> at the shop what do i need

**Turn 4, Claude:**
_(New chat. Reads the Groceries list in Reminders. Per "At the store": only the list, grouped
by aisle, nothing above it. No saved staples, so nothing under it.)_

> **Fridge:** milk
> **Pantry:** coffee, bread

_(5 words.)_

**Ruth, inner:**

> New chat and it still knew. That's the bit I didn't believe this morning. Three things, I
> can hold three things. I didn't need to scroll for anything.

_(The list survived the new chat because it lives in Reminders, not in the chat. Round 2's
risk is closed on this path.)_

---

**Turn 5, Ruth (5:34pm, at the till queue):**

> got milk n coffee. no bread left on the shelf

**Turn 5, Claude:**
_(Ticks the named items. Bread stays on with no question, no comment on the shop.)_

> Ticked milk, coffee. Bread stays on.

_(6 words.)_

**Ruth, inner:**

> Good, it didn't ask if I wanted to remove the bread. I still need bread. I'll get it at the
> corner shop tomorrow, and it'll be on there.

---

**Turn 6, Ruth (5:36pm, walking to the car):**

> k thx

**Turn 6, Claude:**
_(Bare "k" ends the trip and ticks nothing more. No staples question pending.)_

> Done. Bread stays on.

_(4 words.)_

**Ruth, inner:**

> It said bread twice. Doesn't matter, it's short. I'd use this again. Mostly because it never
> asked me to set anything up I couldn't do with one thumb.

---

## Notes for reviewers

1. **Permission line works now.** Naming "Allow Full Access" removed round 3's hesitation (six
   seconds down to two). The "it's how I add to your list" clause answered "why". Still open:
   Ruth wondered if she could undo it. The skill has "Change access later in iPhone Settings →
   Claude" in the Setup section but not in the on-the-yes line. A three-word add ("you can
   undo it in Settings") could close it, at the cost of length. Low priority; she did not
   refuse.
2. **Turn order on a phone matters.** The pop-up appears under the first half of turn 2. The
   permission line has to stream before the tool call, as the skill says ("before making
   it"), or the pop-up arrives with no explanation. It did here.
3. **New chat at the store passed.** With Reminders as the home, the list was there without
   memory. No "From memory" caveat needed.
4. **Tick-off and trip end followed the rules exactly.** "Bread stays on" twice (turns 5 and
   6) is slightly repetitive but harmless; Ruth noticed and did not mind.
5. **Word counts:** every reply under 60 words; the longest was 23. First reply was not only
   setup (items kept first).
6. **Persona verdict:** would use again. Setup cost: one "yes" and one tap, about one minute.
