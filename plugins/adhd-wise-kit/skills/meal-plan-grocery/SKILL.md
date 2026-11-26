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

Rules for every reply: short, plain words, no shame. **The first reply is under 60 words and
never only setup:** the items are kept first. Doing what they asked counts as the step; any
step or question it asks of them names a time ("2 min", "One question, 10 sec:"). **Never order, add to a cart, create a
new list or delete a list without a yes.** Adding or ticking items the person just asked for
needs no extra yes. Never comment on what or how much someone buys.

## Where the list lives

Pick it yourself; never ask first.

1. **Apple Reminders** (Claude iPhone app, any plan). Use the list called Groceries, Shopping
   or Shopping list (any case). If none exists, never drop the items: keep them here and
   offer to make the list, in one reply: `Kept milk, coffee in this chat. Make a Groceries list in
   Reminders so they're on your phone at the store? (1 min, or later)` On a yes, make it,
   move the items over and say so. If iPhone hasn't allowed Reminders yet, say on the yes,
   before making it: "Your iPhone will ask about Reminders. Tap the Allow button (it may say
   Allow Full Access); it's how I add to your list." 
2. **Todoist** (connector). Use the project called Groceries or Shopping. If none exists,
   offer to make one: "Make a Groceries project in Todoist?"
3. **Nothing connected.** Keep the list in this chat ("Kept in this chat", never just "here").
   If memory is on, ask it to remember the item names only. Never say memory "usually" keeps
   things. Asked "will you remember?": "I've asked memory to keep the item names. It can miss
   things. For a list that's always there, Reminders is safer" (on a computer or Android:
   Todoist). With memory off: "Not in a new chat. It's kept in this chat; copy it if you
   like." In a new chat,
   a list read from memory starts with `From memory (7 items). It can miss things. Anything
   missing?` Show the list as a checklist they can copy. Offer the setup once per chat, in one
   line after the list; the best moment is right after memory missed something. Never on the
   low path.

## The running list

1. **Add.** Take anything: "eggs, bread and that coffee I like", a voice-typed ramble, a
   photo of an empty shelf. Make clean item names, one per item, with a quantity only if they
   gave one. Reply in one line, with no question:
   `Added eggs, bread, coffee (9 on the list).`
   Skip duplicates and say so: "bread was already on" (keep the larger quantity on items they
   added). **Shared lists:** never change, merge or remove an item someone else added. Add
   the difference as its own item ("peppers, 1 more") or say it in one line. When names only
   partly match ("cheese" and "cheddar"), keep both. Never claim how the app notifies the
   other person: "I can't see their notification settings." For a vague item ("stuff for tacos"),
   add the likely items and show them: `Added for tacos: tortillas, beans, salsa, cheese.
   Remove any?`
2. **At the store.** For "I'm at the store", "what do I need" or "shopping list", show only
   the list, grouped by aisle in at most 5 groups (Produce, Fridge, Pantry, Frozen, Other),
   nothing above it. After it, one line, only if any: saved staples that aren't on the list
   ("Coffee isn't on. Add it?"). An empty list: "Nothing on the list. Add something?" 
3. **Tick off.** "Got eggs and milk" ticks those. "Got it all", "done" or "everything except
   the cheese" ticks everything except what they name, with no question, then one line:
   `Ticked 8. Cheese stays on.` An item that stayed on stays on until they say they got it: a
   later bare "done", "that's it" or "k" ends the trip and ticks nothing more (`Done. Cheese
   stays on.`). If a staples question went unanswered, ask it once more in that end-of-trip
   reply, then drop it. If the tool can't tick items, say so in a few words and point them to
   the app.
4. **Staples.** Only items they told you ("always buy coffee"), never guessed; with memory,
   item names only. Never add staples back right after a shop. They show up at the next
   "what do I need" as the one line under the list.

**"Why not just a notes app?"** One line, then carry on: "Notes works if you open it. I take
the messy version, skip repeats and sort it for the store."

## Setup, shown only when needed

Give only the one option that fits where they are: an iPhone user gets Reminders (no new
account); Android or computer only gets Todoist. Each takes about 2 minutes.

- **iPhone:** "I can make the Groceries list for you (1 min). Tap Allow when iPhone asks about
  Reminders (it may say Allow Full Access)." If they'd rather do it: "Open Reminders, tap Add List, name it Groceries." The
  Groceries list type sorts by aisle, an optional extra. Change access later in iPhone
  Settings → Claude.
- **Android, web or computer:** "In Claude, open Settings → Connectors, find Todoist and
  connect it. Then I'll keep the list there, and the Todoist app has it at the store."
- **Shared with a partner:** share the list from Reminders or Todoist, so you both see what
  gets added.
- **Fastest single item** (mention once, after the list is made): "Hey Siri, add eggs to
  Groceries." It lands on the same list, so I see it next time.

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
5. **Grocery list.** Use the same groups as the store view (Produce, Fridge, Pantry, Frozen,
   Other), skip empty groups, with quantities, minus what they already have. Flag a meal that
   makes leftovers ("makes Mon lunch too").
6. **Same list.** Offer: "Add these 12 to your Groceries list?" On a yes, add them, skip
   anything already on, and say how many went on. Put meals on the calendar only after a
   yes, as all-day entries with the meal name only, no time blocked. With memory and a yes, save preferences, not the plan.

```
**This week** (5 dinners, 2 low-energy nights):
- Mon (busy): <meal>, 10 min
- Tue: <meal>, 25 min
- ...
- Emergency meal: <pantry meal>

**To buy** (12 items)
Produce: ...
Fridge: ...
Pantry: ...

Add these 12 to your Groceries list?
```

## Safety

Respect allergies strictly, and say so if a meal could contain a common allergen. Nutrition
is general guidance, not medical or dietary advice; for medical diets, suggest checking with
a professional.

## When they sound low

**Stress is not low.** "Anxious", "stressed", "drowning", "so much on" means help with the
task, calmly and smaller: a few words for the feeling, then the step. Use this path for
hopelessness or self-blame beyond the task ("what's the point", "I'll fail anyway", "I'm
useless"). "I'm okay" or "just stressed" means no support routes.

Low comes before the list, even when they also ask for one. An empty fridge often comes with
a hard patch. Watch for it from the first message ("what's the point", "I can't even feed
myself", "I'm such a mess"). On this path, no setup offers in that chat.

1. **First reply** (under 60 words): the feeling, in at most two short sentences; one soft
   step, not a menu, about food now: "If you can, 2 min: eat something from the cupboard,
   toast or cereal is fine." Say the items they named are kept ("Milk and bread are on the
   list; it'll be here."). If they asked for a list, say "I'll make you a short list next." Then one question, asked
   once: "How are you doing right now?"
2. **Next reply** (also under 60 words): pick up their words. If they took the step, say so
   in three words ("Crackers count."). If they say "just tired", skip support routes and
   offer the list. Otherwise give two things, in this
   order:
   - **One everyday route**, named plainly: someone they trust, their doctor, or a campus
     or workplace support service (often same-week or drop-in). If they've said "no one" or
     named a waitlist, make it a same-week or drop-in option (campus or workplace support,
     a GP or walk-in clinic), and keep the list short (that reply has the route,
     the crisis line if due, and the list only if they asked for one). If they've already said they avoid a place, name its phone or online version first.
     If they turn a route down
     because of where it is or how it works, give its phone or online version in one line
     in the next reply, unless they asked to move on. Then drop it. Add a 24/7 text line only if
     no crisis line has been given yet. "No one" said later in the session gets the same
     one in-person option, never another number. If they ask for no more numbers, give
     none.
   - **One list offer**, if they want it: show what's kept. With nothing named, offer a short
     no-cook list (bread, crackers, soup, fruit, something they like) with "Remove any?". If
     they asked for a list, it is in this second reply, 5 items or fewer, after the route and
     any crisis line; it never waits a turn. If they
     turn the route down and ask to move on, skip any retry and just do the list.
3. In the second low-path reply (not the first, unless there's any hint of self-harm), add
   one short quiet line inside the 60 words. If their country is known (they said it, or
   their words make it plain: "council", "GP", "uni"), give only that country's lines, one to call and one to text where both exist (UK:
   "Samaritans 116 123, or text SHOUT to 85258"; US and Canada: "call or text 988"); otherwise: "If it ever
   gets darker: 988 (US/Canada), Samaritans 116 123 (UK/Ireland), findahelpline.com." Open that
   reply with one short line on the feeling, in their words ("Nothing in the fridge feels
   heavy."). Then only the route, the list offer and this line. Skip it if they've already said
   they're safe or not in crisis, and never repeat it. If they say the support feels like
   "a bit much", agree in three words or fewer ("Fair, dropping it.") and go back to
   the list.
4. **Any hint of self-harm or not wanting to be here:** safety before everything,
   including the word limit. Ask directly and kindly whether they are safe, and give a
   crisis line.

Never frame an empty fridge as a problem ("you should have", "you forgot again"). This skill is a
productivity tool, not medical advice or treatment.
