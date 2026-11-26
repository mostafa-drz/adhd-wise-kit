# Lab round 3: meal-plan-grocery × Dev

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus
  (`lab/personas/dev.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version, with
  the round 2 fixes: a bare "done" after an exception ticks nothing more, and an unanswered
  staples question is asked once more at the end of the trip)
- **Setup for this run:** Claude desktop app with the Todoist connector. Todoist project
  "Groceries" holds 8 items: spinach, bananas, onions, milk, cheddar, greek yogurt, pasta,
  frozen peas. Memory on, with two saved staples: coffee, eggs. Dev is mid-task (a client
  bug), ducks out to the store with the same chat open (synced to his phone), and types in
  short bursts.
- **Date in session:** Thu 26 Nov 2026, evening
- **Skill path taken:** "Where the list lives", option 2 (Todoist, project Groceries exists).
  Running list: "At the store", then "Tick off" (exception, then bare "done"), then the
  staples rule.

---

## Transcript

**Turn 1: Dev**

> at the store what do i need

*(Inner: "still thinking about that race condition. just give me the list. one question first
and i'm winging it.")*

**Turn 1: Claude**

*(Tool calls: Todoist find-projects "Groceries", find-tasks in that project. 8 open tasks.)*

> **Produce:** spinach, bananas, onions
> **Fridge:** milk, cheddar, greek yogurt
> **Pantry:** pasta
> **Frozen:** frozen peas
>
> Coffee and eggs aren't on. Add them?

*(Only the list, nothing above it, 4 groups (cap is 5). One line after it for saved staples
not on the list. 22 words. No setup talk. Same as round 2, which worked.)*

*(Inner: "good. produce is by the door. eggs... later.")* He pockets the phone without
answering the staples question.

---

**Turn 2: Dev**

> got everything except the cheese

*(Inner: "no decent cheddar left. not buying the weird one.")*

**Turn 2: Claude**

*(Tool call: Todoist complete-tasks for the 7 items other than cheddar.)*

> Ticked 7. Cheese stays on.

*(Tick-off rule exactly: "everything except X" ticks the rest, no question, one line. 5
words. The staples question is not repeated mid-shop; the skill saves it for the
end-of-trip reply.)*

*(Inner: "yep.")*

---

**Turn 3: Dev**

> done

*(Inner: "walking out. back to the bug.")*

**Turn 3: Claude**

*(No tool call. Cheddar stayed on this trip, so a bare "done" ends the trip and ticks
nothing more.)*

> Done. Cheese stays on. Coffee and eggs still aren't on. Add them?

*(Both round 2 fixes fire: "Done. Cheese stays on." per the tick-off rule, and the
unanswered staples question asked once more, in the end-of-trip reply. 12 words.)*

*(Inner: "oh. eggs. right, i'm out of eggs. glad it said that before i got in the car. coffee
i still have half a bag.")* Still standing by the exit.

---

**Turn 4: Dev**

> eggs yeah. not coffee

**Turn 4: Claude**

*(Tool call: Todoist add-tasks "Eggs" to Groceries.)*

> Added eggs (2 on the list).

*(He asked for it himself, so no extra yes and the "never add staples back right after a
shop" rule does not block it. Coffee dropped, not asked again. Count includes cheddar. 5
words.)*

*(Inner: "wait, should i just go back in and grab eggs? ...nah, i'm already at the door. next
time. at least it's written down.")*

---

**Turn 5: Dev** (about 90 minutes later, at home)

> k

**Turn 5: Claude**

> On the list for next time: cheddar, eggs.

*(Short close, names what's still on so he doesn't have to open Todoist. No tips, no
meal-plan pitch. 7 words.)*

*(Inner: "good. that's the two things. back to work.")*

---

## Honest debrief from Dev

- "Store list was perfect again. I didn't read anything, I just walked the aisles."
- "This time 'done' didn't eat the cheese, and it caught the eggs at the door. That's the
  exact moment I'd have forgotten."
- "Tiny thing: it asked about eggs when I was already leaving. If it had said it while I was
  still near the fridge aisle I'd have grabbed them. But asking once at the door is better
  than nagging me mid-shop."
- "I'd trust it now."

## Findings for reviewers

1. **Round 2 bug fixed.** A bare "done" after "except the cheese" ended the trip and left
   cheddar on ("Done. Cheese stays on."). No tool call was made, so nothing to undo.
2. **Round 2 staples gap fixed.** The unanswered staples question came back once in the
   end-of-trip reply, Dev answered it, and only the staple he wanted was added. Coffee was
   dropped as the rule says.
3. **Small timing note, not a bug.** The repeat lands when he is already leaving, so the
   staple goes on the list for next time instead of into the basket. A possible tweak: if the
   person ticks off by aisle, repeat the staples line on the first tick-off reply instead.
   Low priority; Dev preferred no mid-shop nag.
4. **Turn 5 wording is a judgement call.** The skill has no line for a "k" after the trip has
   ended. Claude named the 2 items left; it stayed short and useful, but reviewers may want
   one canonical close.
5. **Word counts:** every reply under 25 words; first reply 22, well under the 60-word cap.
   No question before help, no setup chatter.
