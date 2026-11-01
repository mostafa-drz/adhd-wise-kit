---
name: meal-plan-grocery
description: >-
  Decides what to eat this week so you don't have to: a realistic meal plan that fits your
  calendar (easy meals on busy nights), uses what you already have, and turns into one
  grocery list sorted by store aisle. Use for "what should I eat", "meal plan", "grocery
  list", "I never know what to cook" or "help me plan food for the week".
metadata:
  side_effects: true
  trigger: "Deciding what to eat, planning meals for the week, or making a grocery list."
  tags: "adhd, meal-planning, groceries, decision-fatigue, calendar, cooking, desktop, code"
---

# Meal Plan + Grocery List

Deciding what to eat, every day, is a surprising amount of decisions. This skill makes
them once a week, sized to your real energy, and hands you one list for the store.

Rules for every reply: the plan first, short, no shame, plain words. **Never place an
order or add to a cart without a yes.**

## The flow

1. **Ask little.** Use memory for known preferences (diet, allergies, dislikes, who's
   eating, budget) if available. Otherwise ask at most two questions in one message:
   "Any foods to avoid, and how many people?" Then plan.
2. **Read the week.** With a calendar connected, mark busy or late days as "low-energy
   nights" (10-minute or no-cook meals). Without one, assume two low-energy nights.
3. **Use what's there.** Ask once: "Anything in the fridge that needs using up?" Build
   the first meals around it.
4. **Plan.** Dinners for 5 to 7 nights (they choose; default 5, leaving room for
   leftovers or eating out). Reuse ingredients across meals so the list stays short.
   Every meal has a time ("20 min") and one line of steps; full recipe only on request.
   Include one "emergency meal" from pantry staples.
5. **Grocery list.** One list, grouped by aisle (produce, protein, dairy, pantry,
   frozen), with quantities, minus what they already have.
6. **Save.** Offer to save the list to notes or a task app, and to put meals on the
   calendar, only after a yes. With memory and a yes, save preferences, not the plan.

## What it looks like

```
**This week** (5 dinners, 2 low-energy nights):
- Mon (busy): <meal>, 10 min
- Tue: <meal>, 25 min
- ...
- Emergency meal: <pantry meal>

**Grocery list**
Produce: ...
Protein: ...
Pantry: ...

Want me to save the list to your notes?
```

## Safety

Respect allergies strictly and say so if a meal could contain a common allergen.
Nutrition is general guidance, not medical or dietary advice; for medical diets, suggest
checking with a professional.
