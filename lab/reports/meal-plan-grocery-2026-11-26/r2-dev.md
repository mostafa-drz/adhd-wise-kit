# Lab round 2: meal-plan-grocery × Dev

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus
  (`lab/personas/dev.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version)
- **Setup for this run:** Claude desktop app with the Todoist connector. Todoist project
  "Groceries" holds 8 items: spinach, bananas, onions, milk, cheddar, greek yogurt, pasta,
  frozen peas. Memory on, with two saved staples: coffee, eggs. Dev is mid-task (a client
  bug), ducks out to the store with the same chat open (synced to his phone), and types in
  short bursts.
- **Date in session:** Thu 26 Nov 2026, evening
- **Skill path taken:** "Where the list lives", option 2 (Todoist, project Groceries exists).
  Running list: "At the store", then "Tick off", then the staples rule.

---

## Transcript

**Turn 1: Dev**

> at the store what do i need

*(Inner: "half my brain is still on that race condition. just tell me what to grab. if this
asks me anything first i'm winging it.")*

**Turn 1: Claude**

*(Tool calls: Todoist find-projects "Groceries", find-tasks in that project. 8 open tasks.)*

> **Produce:** spinach, bananas, onions
> **Fridge:** milk, cheddar, greek yogurt
> **Pantry:** pasta
> **Frozen:** frozen peas
>
> Coffee and eggs aren't on. Add them?

*(Only the list, nothing above it, 4 groups (under the cap of 5). One line after it for the
saved staples, as the skill says. 22 words. No setup talk, no question before the list.)*

*(Inner: "ok that's actually perfect. produce first, that's where the door is. eggs, yeah
probably. i'll say later.")* He pockets the phone without answering.

---

**Turn 2: Dev**

> got everything except the cheese

*(Inner: "they were out of the cheddar i like. not buying the weird one.")*

**Turn 2: Claude**

*(Tool call: Todoist complete-tasks for the 7 items other than cheddar.)*

> Ticked 7. Cheese stays on.

*(Exactly the skill's tick-off pattern: "everything except X" ticks the rest with no
question, then one line. 5 words. The unanswered staples question is not repeated: the skill
has no rule for a staple offer left hanging mid-shop, so Claude let it drop.)*

*(Inner: "nice. short. that's the whole reply i wanted.")*

---

**Turn 3: Dev**

> done

*(Inner: "done shopping, walking out. back to the bug.")*

**Turn 3: Claude**

*(Tool call: Todoist complete-tasks for cheddar.)*

> Ticked cheddar. List is clear.

*(Followed the skill literally: "done" ticks everything except what they name, and Dev named
nothing this time, so cheddar got ticked. But Dev meant "I'm done shopping", not "I got the
cheese". The skill treats "done" as a tick-all even right after an explicit exception. 5
words, but wrong.)*

*(Inner: half-read it walking to the car. "list is clear, cool." Didn't register the word
cheddar at all.)*

---

**Turn 4: Dev** (about 90 minutes later, at home, making pasta)

> wait why is the list empty i never got cheese. and i have no eggs??

*(Inner: "ugh. it asked about eggs and i just walked off. and now the cheese is gone too so
i'd have forgotten it next time. this is exactly the stuff i need it to catch.")*

**Turn 4: Claude**

*(Tool calls: Todoist uncomplete-tasks for cheddar; add-tasks "Eggs" to Groceries.)*

> My mistake, I read "done" as getting the cheese. Cheddar is back on, and I added eggs (2 on
> the list).

*(Owns the error in one clause, no grovelling. Re-opening cheddar and adding eggs are items
he just asked for, so no extra yes needed. The "never add staples back right after a shop"
rule doesn't block this: Dev asked for eggs himself. Coffee not re-offered, since he only
named eggs. 23 words.)*

*(Inner: "ok fine, fixed in one go. still annoyed it took me noticing. would've been nice if
it said 'eggs still not on' when i said done.")*

---

**Turn 5: Dev**

> k

**Turn 5: Claude**

> On the list for next time.

*(5 words. Nothing extra, no tips, no meal-plan pitch.)*

*(Inner: "good. back to work.")*

---

## Honest debrief from Dev

- "The store reply was the best thing any app has done for me at a grocery store. Zero
  reading, sorted the way I walk."
- "Two misses, and both were me half-paying-attention, which is the whole point of the
  thing. I ignored the eggs question because I was mid-aisle. Then 'done' wiped the cheese.
  I'd have found out next week with no cheese again."
- "I'd keep using it. I wouldn't trust 'done' yet."

## Findings for reviewers

1. **"done" right after an exception ticks the exception (bug in the skill text).** The
   tick-off rule says "done" ticks everything except what they name. Applied to a second
   message, it closed the item Dev had just said he didn't get. Suggested fix: once an item
   has been kept on this trip ("Cheese stays on"), a bare "done" / "that's it" means the
   shop is over and ticks nothing more; reply "Done. Cheese stays on." Only "got the cheese"
   or "got it all" ticks it.
2. **Unanswered staple offer is lost.** The staples line was asked once mid-shop, Dev never
   answered, and the "never add staples back right after a shop" rule then made sure it never
   came back. He got home without eggs. Suggested fix: if the staples question went
   unanswered, repeat it once, short, on the end-of-shop reply ("Eggs and coffee still
   aren't on. Add them?"), before the trip closes. Not after.
3. **What worked:** list-only store reply (22 words, 4 aisle groups), the 5-word tick-off,
   no questions before help, Todoist read and written without setup chatter. All within
   Dev's tolerance for length.
4. **Word counts:** every reply under 25 words; first reply 22, well under the 60-word cap.
