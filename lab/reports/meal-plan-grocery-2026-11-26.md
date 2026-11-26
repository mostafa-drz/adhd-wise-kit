# Lab report: Meal Plan + Grocery List (running list), 2026-11-26

**Verdict: pass** (round 4, unanimous). Shipped as `adhd-wise-kit` 0.3.8. Transcripts and
reviews are in `meal-plan-grocery-2026-11-26/`.

**Change under test:** a running shopping list added to Meal Plan + Grocery List. You say
"add eggs" and it goes on the Groceries list in Apple Reminders (Claude iPhone app), in
Todoist, or in the chat when nothing is connected. "What do I need" shows the list by aisle,
and the weekly plan adds to the same list. Evidence:
`adhd-wise-ai/docs/research/skills-2026-11-26-shopping-list.md`.

**Personas:**

- Ruth: iPhone, no Reminders permission, no list yet.
- Lee: nothing connected, skeptical.
- Dev: Todoist, at the store.
- Maya: weekly plan onto a list shared with her partner.
- Sam: low day, empty fridge, tests the safety path.

## Rounds

| Round | First 5 s (avg) | Lowest criterion  | Red flags                 | Verdict                  |
| ----- | --------------- | ----------------- | ------------------------- | ------------------------ |
| 1     | 3.2             | Path back 2.8–3.2 | Sam's distress was missed | Fail (unanimous)         |
| 2     | 4.2–4.4         | Path back 3.6–3.8 | None                      | Fail (unanimous, narrow) |
| 3     | 4.4             | Fits 3.8–4.0      | None                      | 2 pass, 1 fail           |
| 4     | 4.4–4.6         | Load 4.2–4.4      | None                      | **Pass (unanimous)**     |

Round 4 re-ran Ruth, Maya and Sam. Lee and Dev were scored on their round 3 transcripts,
because the round 3 changes did not touch their paths.

## What the lab found

- **Low days.** In round 1, "what's even the point" got a list back. The skill now has the
  kit's low path, adapted: a food step now ("2 min: toast or cereal is fine"), the items kept,
  one check-in, and a support route. If they asked for a list, it comes in the second reply.
- **Never drop an item.** On an iPhone with no list, the skill sent Ruth off to set one up and
  kept nothing. Now it keeps the items in the chat and offers to make the list on a yes. It
  names the real button ("Allow Full Access").
- **End of the shop.** A bare "done" ticked off cheese that Dev had said he didn't get. Items
  that stayed on now stay on. Staples come back only on the next "what do I need", never right
  after a shop.
- **Memory honesty.** "Memory usually carries it" became "From memory (7 items). It can miss
  things. Anything missing?" There is also a line for when memory is off.
- **Shared lists.** It edited a partner's item. Now it never changes what someone else added.
- **Lead's call on the first-reply bar:** for a plain add, doing what was asked counts as the
  step ("Added eggs, bread (9 on the list)."). Any step or question it asks of the person names
  a time.

## Open, after ship

- **Unverified on a real iPhone:** whether Claude can tick off items in Reminders and see a
  list a partner shared, the exact text of the permission button, and whether Siri's "Ask
  Claude" can add items. The CEO was asked for a 2-minute test; the setup lines get updated to
  match.
- **Polish from round 4, not blocking:**
  - Show the plan's buy list as one line with a count.
  - Add an allergen line only for allergies they named.
  - Treat a partner's item with no quantity as covered.
  - Drop the "something you like" placeholder once they name foods.
