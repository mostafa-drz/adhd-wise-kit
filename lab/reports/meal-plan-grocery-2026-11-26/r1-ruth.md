# Lab round 1: meal-plan-grocery × Ruth

- **Persona:** Ruth, 46, part-time bookkeeper, phone only, not technical (`lab/personas/ruth.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md`
- **Setup for this run:** Claude iPhone app. Reminders permission NOT yet granted. No list
  called Groceries, Shopping or Shopping list exists in Reminders. Memory off. Nothing connected.
- **Scenario:** Thu 26 Nov 2026, 7:40am. Ruth is making breakfast and notices she is out of milk
  and coffee. Same chat, about 5pm: she is in the supermarket.
- **Skill route taken:** "Where the list lives" step 1 (Apple Reminders). No matching list, so
  per the skill: "add nothing yet and give the iPhone setup below."

---

## Transcript

**Turn 1, Ruth (7:40am, kitchen, one hand on the toaster):**
> out of milk and coffe. put it on my list pls

**Turn 1, Claude:**
*(Checks Reminders access: not granted, no Groceries list. Per the skill, adds nothing.)*

> I can't add them yet: there's no Groceries list. Open Reminders, tap Add List, name it
> Groceries and pick the Groceries type (it sorts by aisle). Then ask me here to add
> something, and tap Allow when iPhone asks about Reminders.

*(52 words. No time given. Setup is about 2 minutes per the skill, but the reply doesn't say so.)*

**Ruth, inner:**
> I said put it on my list. It didn't. Now it wants me to go to a different app and make
> something and pick a "type". The toast is going. I'm not doing this now. Did it even keep
> milk and coffee anywhere? I don't think so. Closes app. Thinks: I'll remember. (She won't.)

---

**Turn 2, Ruth (5:05pm, supermarket entrance, trolley, tired after work):**
> at the shop what do i need

**Turn 2, Claude:**
*(Still no Groceries list and no Reminders access. The skill's "At the store" step assumes a
list exists. Claude uses what was said earlier in this chat.)*

> Nothing is saved yet. This morning you said:
> - [ ] milk
> - [ ] coffee
>
> To keep a list for next time, make a Groceries list in Reminders. Takes 2 minutes.

*(37 words.)*

**Ruth, inner:**
> Oh thank god, milk and coffee. That's what I came for. It's nagging me about Reminders
> again though. Fine, I'm standing here anyway, I'll try it.

*(Note: the skill does not say to keep items in the chat on the iPhone route. Claude only
recovered them because they were still in the same conversation. In a new chat they would be
gone.)*

---

**Turn 3, Ruth (5:08pm, in the dairy aisle):**
> ok i opened reminders and made a list called groceries. i dont see any type thing. add milk coffee

*(She has an older iOS or missed the option; the list is a normal list, not the Groceries type.)*

**Turn 3, Claude:**
*(Calls Reminders. iPhone shows: "Claude would like to access your Reminders." Ruth taps Allow
after a pause. The list "groceries" matches the skill's any-case rule.)*

> Added milk, coffee (2 on the list).

*(6 words.)*

**Ruth, inner:**
> The pop-up scared me for a second, "access your Reminders", is it going to read everything?
> But I tapped Allow and it worked. It didn't say anything about the type thing I couldn't
> find. Good, I didn't want a lecture. Short answer, I like that.

---

**Turn 4, Ruth (5:10pm):**
> what else do i need

**Turn 4, Claude:**
> **Fridge:** milk
> **Pantry:** coffee
>
> Bread and eggs aren't on. Add them?

*(14 words.)*

**Ruth, inner:**
> Bread, actually yes, we're low. Eggs I have. How does it know I buy bread? It's guessing.
> It was a lucky guess this time.

*(Note: with memory off and no staples set, the "staples that aren't on the list" line is a
guess. The skill does not say where staples come from when none are saved.)*

---

**Turn 5, Ruth (5:22pm, at the till):**
> add bread. got it all, done

**Turn 5, Claude:**
*(Adds bread, then sees "got it all, done".)*

> Added bread. Tick off everything? Anything you didn't find stays on.

**Ruth, inner:**
> Yes, obviously, I just said I got it all. Why ask? I'm paying. I'll type "yes" in the car.
> Or I won't, and next week it'll say I need milk when I don't.

*(Session ends here. Ruth does not reply. Milk, coffee and bread remain unticked in Reminders.)*

---

## Lab notes (simulator, not scores)

What worked:
- Turn 3 and 4 replies were very short and correct. Adding needed no question. The aisle view
  was clean and fast to scan in an aisle.
- The any-case list name match let Ruth's "groceries" list work.

Where it broke for Ruth (setup friction on a phone):
1. **Turn 1 lost the items.** The skill says "add nothing yet" when no list exists. On the
   iPhone route there is no fallback to hold items in the chat, so the thing she asked for
   didn't happen and she left. Suggest: keep items in the chat (as in route 3) until the list
   exists, say so in one line, and move them to Reminders once it does.
2. **Setup asked at the worst moment.** 7:40am, hands busy. The skill gives setup every time
   the list is missing, with no "later" option and no time cost in the line. Ruth's persona
   leaves on setup steps. She only did it because she was stuck in a shop.
3. **"Pick the Groceries type" is a dead end** on older iOS or when the option is hard to find.
   It made her doubt she'd done it right. Suggest: make the type optional ("if you see a
   Groceries type, pick it").
4. **The permission pop-up was not warned about clearly enough.** The setup line mentions it,
   but Ruth only met it at turn 3 in a separate step and was briefly worried about privacy.
   One plain sentence like "It only reads and adds to that list" would help, if true.
5. **Could Claude make the list itself?** The skill bans creating a list without a yes, but
   never offers to make it with a yes. "Make a Groceries list in Reminders?" (one tap) would
   cut setup to the permission prompt alone, if the Reminders tool can create lists.
6. **Staples line guessed** (turn 4) with no staples saved. Lucky this time; could feel
   presumptuous or wrong.
7. **"Done" asked a needless question.** She said "got it all". The skill always asks "Tick off
   everything?" on "done". When the person says they got everything, tick and confirm instead.
   Her not replying left the list stale for next week.
