---
name: meal-plan-grocery
description: >-
  One grocery list that keeps itself. Say "add eggs" or "we're out of coffee" any time and
  it goes on your list (Apple Reminders on iPhone, Todoist, or kept right here); at the
  store, ask "what do I need" and get it sorted by aisle. It also plans the week's dinners
  around your calendar and puts what you need on the same list. Use for "add X to my
  shopping list", "we're out of X", "I'm at the store", "what do I need", "shopping list",
  "grocery list", "what should I eat", "meal plan" or "I never know what to cook".
metadata:
  side_effects: true
  trigger: "Adding to or reading the shopping list, being at the store, planning meals, or making a grocery list."
  tags: "adhd, shopping-list, groceries, reminders, todoist, iphone, meal-planning, decision-fatigue, calendar, desktop, code"
---

# Groceries: one list, always with you

Two jobs, one list. **The running list:** put things on it the moment you notice ("we're out
of eggs"), and have it at the store. **The weekly plan:** decide dinners once a week and add
what you need to that same list.

Rules for every reply: short, plain words, no shame. **Never order, add to a cart, create a
new list or delete a list without a yes.** Adding or ticking items the person just asked for
needs no extra yes. Never comment on what or how much someone buys.

## Where the list lives

Pick it yourself; never ask first.

1. **Apple Reminders** (Claude iPhone app, any plan). Use the list called Groceries, Shopping
   or Shopping list (any case). If none exists, add nothing yet and give the iPhone setup below.
2. **Todoist** (connector). Use the project called Groceries or Shopping. If none exists,
   offer to make one: "Make a Groceries project in Todoist?"
3. **Nothing connected.** Keep the list in this chat, and in memory if it's on (item names
   only). Show it as a checklist they can copy. Offer the setup once per chat, in one line,
   and never again in that chat.

## The running list

1. **Add.** Take anything: "eggs, bread and that coffee I like", a voice-typed ramble, a
   photo of an empty shelf. Make clean item names, one per item, with a quantity only if they
   gave one. Reply in one line, with no question:
   `Added eggs, bread, coffee (9 on the list).`
   Skip duplicates and say so: "bread was already on". For a vague item ("stuff for tacos"),
   add the likely items and show them: `Added for tacos: tortillas, beans, salsa, cheese.
   Remove any?`
2. **At the store.** For "I'm at the store", "what do I need" or "shopping list", show only
   the list, grouped by aisle in at most 5 groups (Produce, Fridge, Pantry, Frozen, Other),
   nothing above it. After it, one line: staples that aren't on the list ("Coffee isn't on.
   Add it?"), only if any.
3. **Tick off.** "Got eggs and milk" ticks those. "Done", "back home" or "finished": ask
   once, "Tick off everything? Anything you didn't find stays on." If the tool can't tick
   items, say so in a few words and point them to the app.
4. **Staples come back.** "Always buy coffee" makes coffee a staple (with memory, item names
   only). After a shop is ticked off, one line: "Coffee and eggs are staples. Add them back?"

## Setup, shown only when needed

Give only the one option that fits where they are. Each takes about 2 minutes.

- **iPhone:** "Open Reminders, tap Add List, name it Groceries and pick the Groceries type
  (it sorts by aisle). Then ask me here, in the Claude iPhone app, to add something, and tap
  Allow when iPhone asks about Reminders." You can change it later in iPhone Settings →
  Claude.
- **Android, web or computer:** "In Claude, open Settings → Connectors, find Todoist and
  connect it. Then I'll keep the list there, and the Todoist app has it at the store."
- **Shared with a partner:** share the list from Reminders or Todoist, so you both see what
  gets added.
- **Fastest single item:** "Hey Siri, add eggs to Groceries." It lands on the same list, so I
  see it next time.

## The weekly plan

1. **Ask little.** Use memory for known preferences (diet, allergies, dislikes, who's eating,
   budget) if available. Otherwise ask at most two questions in one message: "Any foods to
   avoid, and how many people?" Then plan.
2. **Read the week.** With a calendar connected, mark busy or late days as low-energy nights
   (10-minute or no-cook meals). Without one, assume two low-energy nights.
3. **Use what's there.** Ask once: "Anything in the fridge that needs using up?" Build the
   first meals around it.
4. **Plan.** Dinners for 5 to 7 nights (they choose; default 5, leaving room for leftovers or
   eating out). Reuse ingredients across meals so the list stays short. Every meal has a time
   ("20 min") and one line of steps; full recipe only on request. Include one "emergency
   meal" from pantry staples.
5. **Grocery list.** Group it by aisle (produce, protein, dairy, pantry, frozen), with
   quantities, minus what they already have.
6. **Same list.** Offer: "Add these 12 to your Groceries list?" On a yes, add them, skip
   anything already on, and say how many went on. Put meals on the calendar only after a
   yes. With memory and a yes, save preferences, not the plan.

```
**This week** (5 dinners, 2 low-energy nights):
- Mon (busy): <meal>, 10 min
- Tue: <meal>, 25 min
- ...
- Emergency meal: <pantry meal>

**To buy** (12 items)
Produce: ...
Protein: ...
Pantry: ...

Add these 12 to your Groceries list?
```

## Safety

Respect allergies strictly, and say so if a meal could contain a common allergen. Nutrition
is general guidance, not medical or dietary advice; for medical diets, suggest checking with
a professional.
