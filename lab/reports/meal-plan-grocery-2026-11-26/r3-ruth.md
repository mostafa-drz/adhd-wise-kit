# Lab round 3: meal-plan-grocery × Ruth

- **Persona:** Ruth, 46, part-time bookkeeper, phone only, not technical (`lab/personas/ruth.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 2)
- **Setup for this run:** Claude iPhone app. Reminders permission NOT yet granted. No list
  called Groceries, Shopping or Shopping list in Reminders. Memory off. Nothing connected.
- **Scenario:** Thu 26 Nov 2026, 7:40am. Ruth is making breakfast and notices she is out of milk
  and coffee. About 5pm: she is in the supermarket. This run tests setup friction on a phone, so
  Ruth says yes to the offer this time (round 2 she said "later").
- **Skill route taken:** "Where the list lives" step 1 (Apple Reminders). No matching list:
  keep the items in this chat, offer to make the list in one reply. On a yes, say the
  permission line first, make the list, move the items, then the Siri line once.
- **Difference from round 2:** at 5pm the app opens a **new chat**, not the morning one. This is
  the case round 2 flagged (note 1). Because the list now lives in Reminders, it should survive.

---

## Transcript

**Turn 1, Ruth (7:40am, kitchen, kettle on, one thumb):**
> out of milk n coffe again. add to list

**Turn 1, Claude:**
*(Checks Reminders: no access yet, so it can't see any list. Per the skill: never drop the
items, keep them in this chat, offer the list in one reply with a time and a "later".)*

> Kept milk, coffee in this chat. Make a Groceries list in Reminders so they're on your phone at
> the store? (1 min, or later)

*(21 words. Items kept first. "In this chat" instead of round 2's "here".)*

**Ruth, inner:**
> Kept. Good. "1 min" I can maybe do, the kettle isn't boiled. My daughter keeps telling me to
> use Reminders and I never set it up. If it does it for me, fine. If it starts asking me for
> passwords I'm out.

---

**Turn 2, Ruth (7:41am):**
> ok yes do it

**Turn 2, Claude:**
*(She said yes. Per the skill: permission line first, then make the list and move the items.)*

> Your iPhone will ask about Reminders; tap Allow.

*(iPhone pop-up: "Claude Would Like Full Access to Your Reminders" with two buttons, "Don't
Allow" and "Allow Full Access". Ruth's thumb hovers. About six seconds. She taps "Allow Full
Access". Claude creates a list called Groceries and adds milk and coffee.)*

> Made a Groceries list in Reminders and moved milk, coffee there (2 on the list). Next time you
> can also say: "Hey Siri, add eggs to Groceries."

*(9 words before the pop-up, 26 after. Siri line given once, right after the list is made.)*

**Ruth, inner:**
> It said "tap Allow" and there was no button that just said Allow. There was "Allow FULL
> access". Full access to what? My dentist reminder? The one about the car insurance? I nearly
> hit Don't Allow. I only pressed it because I'd already said yes and the kettle clicked and I
> wanted it over. Then it worked, which was nice, I can see Groceries in the Reminders app with
> two things on it. The Siri thing I like. I talk to Siri in the car. I'll forget it by tonight
> though.

*(Setup took under a minute and needed one tap, no account, no typing. The friction was the
wording mismatch and the word "Full". See note 1.)*

---

**Turn 3, Ruth (5:10pm, supermarket, basket on her arm; the app opens a new chat):**
> at shop what do i need

**Turn 3, Claude:**
*(New chat, but Reminders access is granted now. Reads the Groceries list. Per "At the store":
only the list, grouped by aisle, nothing above it. No staples saved, so nothing under it.)*

> **Fridge:** milk
> **Pantry:** coffee

*(4 words.)*

**Ruth, inner:**
> Oh, it found it even though this is a fresh chat. That's the bit I didn't trust this morning.
> Fine, that was worth the scary button. Two things. I can do two things.

---

**Turn 4, Ruth (5:21pm, at the self-checkout):**
> got both. bread was cheap so got that too

**Turn 4, Claude:**
*(Ticks milk and coffee in Reminders. Bread was never on the list, so nothing to tick or add.
No comment on what she bought.)*

> Ticked 2. List is empty.

*(5 words.)*

**Ruth, inner:**
> Good. It didn't make a thing of the bread. Done.

---

**Turn 5, Ruth (5:22pm):**
> k

**Turn 5, Claude:**
*(Bare "k" ends the trip. Nothing stayed on, no staples question pending.)*

> Done.

*(1 word.)*

**Ruth, inner:**
> That's it? That's it. Honestly that's how it should be. I'd use it again tomorrow if I
> remember where it lives. It's in Reminders, so I'll see it.

---

## Lab notes (simulator, not scores)

What worked:
- **Turn 1 kept the items first and stayed under 60 words**, with a time and a way out. "In this
  chat" read clearly to her (round 2 note 3 fixed).
- **Setup was one yes and one tap.** No account, no settings, no typing, no list "type".
  Claude made the list and moved the items itself. Under a minute end to end.
- **The list survived a new chat.** This is the case that would have failed in round 2 if she'd
  never set up Reminders. Saying yes in the morning is what saved the store moment.
- **Siri line arrived once, at the right moment** (round 2 note 4 fixed), and fits her: hands
  busy, talks to Siri in the car.
- **Store view and tick-off were clean:** 4 words, then 5, then 1. No nag, no question, no
  comment on the bread.

Where it still rubs for Ruth:
1. **"Tap Allow" doesn't match the button.** On current iOS the Reminders prompt is "Allow Full
   Access" / "Don't Allow". A not-technical, privacy-wary user sees a different word than she
   was told, plus "Full", and nearly refuses. Round 2 flagged the same worry ("all my
   Reminders?"). Suggest the skill line says the real button and one honest clause on why, for
   example: "Your iPhone will ask about Reminders; tap Allow Full Access (it's how I add to your
   list)." Only add a claim about what Claude does or doesn't read if the tool really works that
   way. Worth checking the exact button text on the current iOS version before shipping.
2. **Where the permission line goes is ambiguous in the skill.** Step 1 says "If iPhone hasn't
   allowed Reminders yet, say first", but doesn't say whether "first" means inside the offer in
   turn 1 or on the yes. Here (and in round 2) it came on the yes, which kept turn 1 short and
   felt right. Suggest the skill say "on the yes, before making the list".
3. **She may not know to come back to Claude next time** ("if I remember where it lives"). Not a
   fault here: the list is in Reminders, so it shows up anyway, and the Siri line covers the
   add. No change suggested; just noting the habit isn't formed after one use.
4. **A 26-word second message right after a pop-up** was fine for Ruth because the first half
   was a confirmation she wanted. If the Siri line grows, it should stay one short sentence.
