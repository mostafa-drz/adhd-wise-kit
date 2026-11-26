# Lab round 1: meal-plan-grocery × Dev

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus, writes short and
  lowercase (`lab/personas/dev.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md`
- **Setup for this run:** Claude desktop with the Todoist connector. Todoist project
  "Groceries" holds 8 open items: bananas, spinach, onions, milk, cheddar, greek yogurt, pasta,
  frozen peas. Memory on, with staples saved: coffee, eggs (item names only).
- **Scenario:** Thu 26 Nov 2026, about 7:15pm. Dev left a client bug half-fixed to grab food
  before the shop shuts. Same chat continued on his phone (Claude app, same account; the list
  lives in Todoist so it is the same either way). He reads every reply standing in an aisle,
  basket in one hand.
- **Skill route taken:** "Where the list lives" step 2 (Todoist project Groceries exists). Then
  "The running list" steps 2 (at the store), 3 (tick off) and 4 (staples come back).

---

## Transcript

**Turn 1, Dev (store entrance, still thinking about the bug):**
> at the store what do i need

**Turn 1, Claude:**
*(Reads Todoist project Groceries: 8 open items. Per step 2: only the list, at most 5 aisle
groups, nothing above it. Then one line on staples not on the list: coffee and eggs.)*

> **Produce:** bananas, spinach, onions
> **Fridge:** milk, cheddar, greek yogurt
> **Pantry:** pasta
> **Frozen:** frozen peas
>
> Coffee and eggs aren't on. Add them?

*(31 words. No greeting, no preamble. Readable in one glance.)*

**Dev, inner:**
> oh nice. that's it, that's the list. produce first, cool, i'm literally standing in it.
> coffee yes obviously, i'd have been raging tomorrow at 8am with no coffee. "add them" though,
> i'm here, i'll just grab them. whatever, yes is faster than thinking.

---

**Turn 2, Dev:**
> ya

**Turn 2, Claude:**
*(Adds coffee and eggs to Todoist Groceries. Neither was on, so no duplicate note.)*

> Added coffee, eggs (10 on the list).

**Dev, inner:**
> good. didn't need the count but fine. ok go.

*(About 9 minutes pass. Dev shops. The cheese shelf is empty.)*

---

**Turn 3, Dev (at the till queue):**
> got everything except the cheese

**Turn 3, Claude:**
*(Per step 3, "Got X" ticks those. "Everything except the cheese" = the other 9 items. Completes
9 tasks in Todoist; cheddar stays open.)*

> Ticked 9. Cheddar stays on.

**Dev, inner:**
> perfect. that's exactly what i wanted. cheddar stays, i'll get it at the corner shop or
> forget forever, either way it's on the list.

---

**Turn 4, Dev (walking out, typing with a thumb):**
> done

**Turn 4, Claude:**
*(Step 3 says: on "done", ask once, "Tick off everything? Anything you didn't find stays on."
Following the skill strictly, Claude asks, even though only cheddar is still open and Dev
already said he didn't get it.)*

> Tick off everything? Anything you didn't find stays on.

**Dev, inner:**
> what. i literally just told you. there's one thing left and it's the cheese i didn't get.
> "anything you didn't find stays on" so... is this asking if i want to tick the cheese? is
> it going to tick the cheese if i say yes? i don't know what yes does here. i was done.
> this is the moment where i close the app.

---

**Turn 5, Dev:**
> no cheese stays

**Turn 5, Claude:**
*(Nothing to tick. Shop is finished, so step 4 fires: one line offering staples back.)*

> Cheddar stays on. Coffee and eggs are staples. Add them back?

**Dev, inner:**
> add them back?? i bought them eleven minutes ago. you told me to add them, i added them, i
> bought them, now they go back on? so next time the list says coffee when i have a full bag?
> that's how i end up with four bags of coffee. or i stop trusting the list. ok i'm not
> answering this. car.

*(Dev does not reply. Chat ends. Todoist: cheddar open, coffee and eggs completed and not
re-added.)*

---

## Observations (for the reviewers)

1. **Turns 1 to 3 were close to ideal for Dev.** Short, no questions before help, list grouped
   by where he was standing, and "Ticked 9. Cheddar stays on." matched what he meant.
2. **Turn 4 asked a question the conversation had already answered.** Step 3 says to ask
   "Tick off everything?" on "done" with no exception for when the person has just ticked
   items. With only the not-found item left, the question was confusing: Dev could not tell
   whether "yes" would tick the cheese. This was the one point where he nearly left. Possible
   rule: if everything except items the person named as not found is already ticked, skip the
   question and reply "All done. Cheddar stays on."
3. **Turn 5's staples line read as wrong.** Step 4 ("After a shop is ticked off: Coffee and
   eggs are staples. Add them back?") offers to put back items he bought minutes ago. For
   Dev it made the list feel untrustworthy (risk of buying duplicates). The rule's intent is
   unclear: re-add now, or remind at the next shop? Turn 1's "aren't on. Add them?" already
   covers staples at the next shop, so step 4 may be redundant.
4. **Turn 1's staples offer while at the store** was mildly odd ("i'm here, i'll just grab
   them") but cheap. A softer wording at the store could be "Coffee and eggs aren't on, in
   case you need them." Not a blocker.
5. **Counts:** "(10 on the list)" was ignored but harmless.
6. **Surface note:** the scenario is Claude desktop, but nobody is at a store on a desktop.
   This worked only because the same chat continued on the phone and the list lives in
   Todoist. The skill does not assume a device here, which is right.
7. **No rule broken:** nothing ordered, no list created or deleted, no comment on what he
   bought, adds and ticks were only items he asked for.
