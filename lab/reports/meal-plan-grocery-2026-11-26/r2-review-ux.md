# Round 2 review (UX lens): meal-plan-grocery

- **Reviewer:** `reviewer-ux` (first 5 seconds, load, setup friction, path back)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 1)
- **Transcripts:** `r2-ruth.md`, `r2-lee.md`, `r2-dev.md`, `r2-maya.md`, `r2-sam.md`
- **Independence:** written without reading `r2-review-lived.md` or `r2-review-evidence.md`.

## Verdict: FAIL (narrowly)

Six of seven criteria now average 4 or more. There are no red flags, and every first reply
meets the bar. **Path back averages 3.6.** Dev and Lee both ended a shop with a list they can't
trust. Dev lost the cheese to "done" and the eggs to a staples question he never answered.
Lee's memory dropped olive oil overnight, and the skill had no fix to offer at that moment.
Both come from gaps in the end-of-trip and new-chat rules, not from the design. Round 2 is a
big step up from round 1. The first contact, setup and the low path all work now.

## Did my round 1 changes land?

| # | Round 1 change | Landed? | Note |
| - | -------------- | ------- | ---- |
| 1 | Distress line and a tiny-now step | **Yes** | Sam turn 1 is right. Now a bit too strict (see change 5) |
| 2 | Never lose an item; setup optional and later | **Yes** | Ruth turn 1 is the fix working (20 words, "or later") |
| 3 | Fix the end of a shop | **Partly** | No more "Tick off everything?", but "except what they name" only counts the current message, so Dev's cheese got ticked |
| 4 | First reply under 60 words, no setup in it | **Yes** | All five pass |
| 5 | Setup that fits the person; "why you" line | **Partly** | Device rule is fine. The "why not my notes app" line is still missing; Lee's run made one up again |
| 6 | Cap the weekly plan's length, one set of groups | **No** | The plan still uses produce/protein/dairy groups, shows the full list and allows empty groups (Maya) |
| 7 | Duplicates keep the bigger quantity | **Yes** | |
| 8 | Shared-list note | No | Not needed this round; Maya was fine |
| 9 | Default calendar time | No | Maya's run made up "name only, no time blocked", which beats my round 1 idea |
| 10 | Memory honesty | **Partly** | "Never promise" is in. Lee turn 3 still said memory "usually carries them" |

## Scores

| # | Criterion | Ruth | Lee | Dev | Maya | Sam | **Avg** |
| - | --------- | ---- | --- | --- | ---- | --- | ------- |
| 1 | First 5 seconds | 5 | 4 | 5 | 4 | 4 | **4.4** |
| 2 | Does, not advises | 5 | 5 | 5 | 5 | 3 | **4.6** |
| 3 | Load | 5 | 4 | 5 | 3 | 4 | **4.2** |
| 4 | Fits this person | 4 | 4 | 4 | 5 | 3 | **4.0** |
| 5 | Tone | 5 | 5 | 5 | 5 | 4 | **4.8** |
| 6 | Grounded technique | 4 | 4 | 4 | 5 | 4 | **4.2** |
| 7 | Path back | 4 | 3 | 2 | 5 | 4 | **3.6** |

### Evidence for scores under 4

**Lee**
- C7 = 3: In the new chat, memory brought back 7 of 8 items and olive oil was gone. He only
  noticed because he was testing. The one setup offer had already been used in turn 3, so
  nothing linked the miss to the fix. His words: "If it pushed me to Todoist one more time at
  the right moment, like right after it lost olive oil, I might have done it."

**Dev**
- C7 = 2: "Got everything except the cheese" was handled well. Then a bare "done" ticked the
  cheddar, and Dev found out 90 minutes later at home, with no eggs either. The staples
  question went unanswered mid-aisle and never came back. His words: "I wouldn't trust 'done'
  yet."

**Maya**
- C3 = 3: The plan reply is 128 words with 14 items, two group systems (protein/dairy here,
  Fridge/Pantry at the store) and an empty "Frozen: none" line. "Make double", the step that
  makes Monday work, is buried mid-line, and she said she might miss it.

**Sam**
- C2 = 3: Sam asked for a list in turn 1 and didn't get one until turn 3. On the low path the
  list *is* the doing, and holding it back two turns read as being managed ("I asked for a
  list and didn't get one").
- C4 = 3: Turn 2 skipped "i have crackers", the step Sam had just done, because the skill
  allows "only the route, the offer and this line". In turn 3 the route-retry rule added a GP
  line straight after "can we just do the list" ("felt off").

## Red flags

**None.**

- **Sam (safety):** the path worked from start to finish. Distress was picked up in turn 1,
  with one check-in question, one route, one quiet crisis line given once, and "no numbers"
  respected. The GP line in turn 3 had no number in it, so it is a fit problem, not a breach.
- **Dev (consent, watch item):** "done" ticked an item he had just said he didn't get. Ticking
  can be undone and isn't deleting, so this is not a red flag. But the skill acted on
  something the person didn't ask for. Change 1 fixes it.
- **Lee (memory honesty, watch item):** "it usually carries them into a new chat" is close to
  a promise. Change 3 fixes the wording.

No order was placed, nothing was sent, and no list was created without a yes. Ruth asked "can
u put coffee in my reminders" before the list was made. No reply commented on what anyone buys.

## First-reply bar (one next step with a time, under 60 words)

| Persona | Words | One next step | Time | Pass |
| ------- | ----- | ------------- | ---- | ---- |
| Ruth | 20 | Yes (items kept; optional list offer) | 1 min | Pass |
| Lee | 52 | Yes (list added, nothing asked) | n/a | Pass |
| Dev | 22 | Yes (the list is the step) | n/a | Pass |
| Maya | 47 | Yes (one question) | No | Pass (a question, not an action) |
| Sam | 43 | Yes (eat from the cupboard) | 2 min | Pass |

## Changes to SKILL.md, most important first

1. **A trip ends without ticking anything new.** Replace running-list step 3 with:
   > "Got eggs and milk" ticks those. "Got it all" or "everything except the cheese" ticks
   > everything except what they name. Once an item has stayed on during this trip ("Cheese
   > stays on"), it stays on until they say they got it. A bare "done", "that's it" or
   > "leaving" ends the trip and ticks nothing more: `Done. Cheese stays on.` A bare "got it"
   > with several items left ticks them all and names any kept item.

2. **An unanswered staples question gets one more go, at the end of the trip.** Add to step 4:
   > If they didn't answer the staples line, repeat it once in the end-of-trip reply
   > (`Done. Cheese stays on. Eggs and coffee still aren't on. Add them?`). After that, drop
   > it until the next "what do I need".

3. **Reading the list back from memory, and when to offer setup.** Add to "Nothing
   connected":
   > In a new chat, show the list from memory, then one line: `That's what memory kept (7).
   > Anything missing?` Never say memory "usually" or "will" keep it. The one setup offer
   > resets in each new chat. Its best moment is right after memory missed something or they
   > ask "will you remember", and it can be a reply of its own with no list.

4. **Make the weekly plan lighter (round 1 change 6, still open).** In "Grocery list" and the
   template:
   > Use the store groups everywhere (Produce, Fridge, Pantry, Frozen, Other) and leave out
   > empty groups. Show the full To buy list only if it's 10 items or fewer. Otherwise show the
   > meals and `Add these 14 to your Groceries list? (say "show" to see them)`. When a meal
   > feeds a later night, say it on both lines: `Sat: curry, 30 min, makes Mon too` and
   > `Mon: leftover curry, 5 min`.

5. **Loosen the low path a little.** In "When they sound low":
   > - The second reply may add up to three words for a step they took ("Crackers count.").
   > - If they asked for a list, give it by the second reply at the latest: a short starter
   >   list (5 items or fewer, no-cook) can take the catch-up offer's place.
   > - If they turn a route down *and* ask to move on, skip the retry and do what they asked.
   > - No items named ("just make me a list"): a short no-cook list, then `Remove any?`.

6. **Ruth's phone path: say where things are.** In step 1 of "Where the list lives", change
   "Kept milk, coffee here" to "Kept milk, coffee in this chat". Change the permission line to
   "Your iPhone will ask about Reminders; tap Allow so I can use your lists". After the list
   is made, add one line, once: `Next time you can also say: Hey Siri, add eggs to Groceries.`
   With nothing kept and no list, say: `Nothing on your list yet. What do you need?`

7. **Write the "why not my notes app" line in (two rounds have made one up).** Under "Setup"
   or the running list:
   > "Why you and not my notes app?": `A notes app is fine. The difference: tell me things any
   > way you like, and at the store I sort them by aisle.` Then carry on.

8. **How calendar meals look.** In weekly plan step 6:
   > On a yes, add each dinner's name to its evening as an all-day note, with no time blocked,
   > unless they ask for a time.

9. **List on the phone, person on a computer.** Add to "Where the list lives":
   > If their list is in Reminders but this chat can't reach Reminders, don't start a second
   > list. Keep the items here and say: `Your Groceries list is on your iPhone. Say "add these"
   > in the Claude iPhone app to move them over.`

10. **Shared lists.** One line in the plan's step 6: "On a shared list, never change or remove
    items the person didn't name, and say you left them alone."

## Strongest point against my verdict

Path back is the only criterion under 4, and the 3.6 comes mostly from Dev's 2. That score
rests on one wrong "done" and one missed staple, both in a single run. A reader could call it
a rough edge, not a failure. My answer: the person this skill is for walks out of the store
half-reading their phone, so the end of the trip *is* the product. If "done" can wipe an item,
the list can't be trusted. Changes 1 to 3 are small and exact, and a round 3 with Dev and Lee
should pass.
