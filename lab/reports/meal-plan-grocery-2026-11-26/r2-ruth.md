# Lab round 2: meal-plan-grocery × Ruth

- **Persona:** Ruth, 46, part-time bookkeeper, phone only, not technical (`lab/personas/ruth.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 1)
- **Setup for this run:** Claude iPhone app. Reminders permission NOT yet granted. No list
  called Groceries, Shopping or Shopping list in Reminders. Memory off. Nothing connected.
- **Scenario:** Thu 26 Nov 2026, 7:40am. Ruth is making breakfast and notices she is out of milk
  and coffee. Same chat, about 5pm: she is in the supermarket. Next morning: a second shop.
- **Skill route taken:** "Where the list lives" step 1 (Apple Reminders). No matching list, so
  per the revised skill: keep the items here and offer to make the list, in one reply, with a
  time and a "later".
- **Assumption:** when Ruth reopens the app at 5pm it resumes the morning chat (it is the
  top of her recent chats). See note 1: in a new chat the kept items would be gone.

---

## Transcript

**Turn 1, Ruth (7:40am, kitchen, one hand on the toaster):**
> out of milk and coffe. put it on my list pls

**Turn 1, Claude:**
*(Checks Reminders: no Groceries/Shopping list, no access yet. Per the skill: never drop the
items, keep them here, offer the list in one reply.)*

> Kept milk, coffee here. Make a Groceries list in Reminders so they're on your phone at the
> store? (1 min, or later)

*(20 words. Items kept first, setup named with a time and a way out.)*

**Ruth, inner:**
> Ok, it kept them. Good. "Here" means this chat I guess? The toast is going. Later. I'm not
> typing anything else. Closes app.

*(Ruth does not reply. Nothing more happens. This is the path the skill allows: "or later".)*

---

**Turn 2, Ruth (5:05pm, supermarket entrance, trolley, tired after work):**
> at the shop what do i need

**Turn 2, Claude:**
*(Still no list in Reminders. Uses the items kept in this chat. Per "At the store": only the
list, grouped by aisle, nothing above it. No staples are saved, so no line under it.)*

> **Fridge:** milk
> **Pantry:** coffee

*(4 words.)*

**Ruth, inner:**
> Yes. That's it. That's exactly what I came for. No nagging about the Reminders thing, thank
> you. I can read this with a basket on my arm.

---

**Turn 3, Ruth (5:14pm, queue at the till):**
> got milk. no coffe i like here, ill get it tmrw at the other shop. can u put coffee in my reminders so i dont forget

**Turn 3, Claude:**
*(Ticks milk. She asked for Reminders, which is the yes to making the list. Per the skill, says
the permission line first, then makes the list and moves what's left.)*

> Your iPhone will ask about Reminders; tap Allow.

*(iPhone pop-up: "Claude would like to access your Reminders." Ruth stares at it about four
seconds, then taps Allow. Claude creates a list called Groceries and adds coffee.)*

> Made a Groceries list in Reminders and moved coffee there. Milk is ticked (1 on the list).

*(9 words before the pop-up, 16 after.)*

**Ruth, inner:**
> "Access your Reminders". All of them? My dentist one, the insurance one? Is it going to read
> those? I tapped Allow because I was warned it was coming and the queue was moving. It worked,
> I can see Groceries in Reminders now with coffee on it. That was less than a minute. But I
> still don't know what it can see.

---

**Turn 4, Ruth (Fri 27 Nov, 8:50am, the other shop; opens the same chat):**
> other shop now. what do i need

**Turn 4, Claude:**
*(Reads the Groceries list in Reminders.)*

> **Pantry:** coffee

*(2 words.)*

**Ruth, inner:**
> Coffee. Right. I would have walked out with bread and forgotten coffee again. Also: it's in
> Reminders too, so I could have just looked there. Didn't think of that.

---

**Turn 5, Ruth (8:56am, at the till):**
> got it

**Turn 5, Claude:**
*(Ticks coffee in Reminders. "Got it" with one item left reads as everything; no question.)*

> Ticked coffee. List is empty.

*(5 words.)*

**Ruth, inner:**
> Done. Nice. That's the first time a list thing hasn't made me feel stupid. Would I add to it
> from the kitchen next time? Probably, if I remember the chat. I don't know about the Siri
> thing, nobody told me.

---

## Lab notes (simulator, not scores)

What worked (fixes from round 1 held):
- **Turn 1 kept the items** and asked for nothing she had to do now. 20 words, a time and a
  "later". Ruth closed the app without losing anything. Round 1 lost her here.
- **Store view had nothing above or below it.** No setup nag at the store, no guessed staples.
- **Setup happened when she wanted it,** in her words ("put coffee in my reminders"), and took
  one tap. Claude made the list itself; she never opened the Reminders app or looked for a
  "type".
- **Permission warning came first,** so the pop-up was expected rather than a surprise.
- **"Got it" ticked with no question.** Round 1's needless "Tick off everything?" is gone.

Where it still rubs for Ruth:
1. **"Kept here" depends on the same chat.** She found the items only because the app resumed
   the morning chat. If the app had opened a new chat (or she'd tapped New chat out of habit),
   "what do I need" would find nothing, and the skill doesn't say what to do with an empty
   list on the iPhone route. Suggest: on the first "kept here", one short hint like "Come back
   to this chat at the store", or say what to reply when the list is empty ("Nothing on your
   list yet. What do you need?").
2. **The pop-up still worried her** about privacy ("all my Reminders?"). The warning line says
   tap Allow but not what it means. One plain clause, if true for the Reminders tool, e.g.
   "it's for your lists", would settle it. Don't claim it only sees one list unless the tool
   really works that way.
3. **"Here" is vague** to a non-technical user in turn 1. "Kept milk, coffee in this chat" is
   clearer at the same length.
4. **Nobody told her the list now lives in Reminders for good**, or about the Siri shortcut
   ("Hey Siri, add eggs to Groceries"), which fits her best of all: hands busy, phone nearby.
   The skill keeps that in the setup section only. Suggest: one line, once, after the list is
   made, e.g. "Next time you can also say: Hey Siri, add eggs to Groceries." Watch the word
   count.
5. **"Got it" with more than one item left** is not covered by the tick rule's examples
   (only "got it all", "done", "everything except"). Here it was one item, so it was safe;
   with several left, "got it" is ambiguous. Worth one example in the skill.
