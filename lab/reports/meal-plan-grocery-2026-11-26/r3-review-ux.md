# Round 3 review (UX lens): meal-plan-grocery

- **Reviewer:** `reviewer-ux` (first 5 seconds, load, setup friction, path back)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 2)
- **Transcripts:** `r3-ruth.md`, `r3-lee.md`, `r3-dev.md`, `r3-maya.md`, `r3-sam.md`
- **Independence:** written without reading `r3-review-lived.md` or any other round 3 review.

## Verdict: FAIL (narrowly)

Path back is fixed. It went from 3.6 to 4.6, and Dev now says "I'd trust it now". Six of seven
criteria average 4 or more. There are no red flags, and every first reply meets the bar.
**Fits this person averages 3.8.** Two round 2 changes I asked for did not land, and each one
cost a point in the run that tested it:

- **Sam:** the list was still held back for two replies after Sam asked for it. The new
  waitlist rule ("let the list wait a turn") now makes the hold a written rule. Sam's
  "a bit much" in turn 3 is a direct result.
- **Maya:** she said "I don't want to make a mess of his stuff", and the skill edited her
  partner's item anyway (peppers became "peppers (2)"). This was my round 2 change 10, and it
  wasn't added.

Both fixes are one rule each. Round 4 only needs to re-run Sam and Maya.

## Did my round 2 changes land?

| # | Round 2 change | Landed? | Note |
| - | -------------- | ------- | ---- |
| 1 | Ending a trip ticks nothing new | **Yes** | Dev turn 3: `Done. Cheese stays on.` with no tool call |
| 2 | Unanswered staples question gets one more go | **Yes** | Dev turn 3 caught the eggs at the door |
| 3 | Memory read-back line; setup offer resets each chat | **Yes** | Lee turns 4 and 5 are exactly right |
| 4 | Lighter weekly plan | **Partly** | Store groups are in step 5, and the leftover is flagged on both lines. The template still says "Protein:". A list over 10 items still shows in full (Maya: 15) |
| 5 | Loosen the low path | **Partly** | "Crackers count", the skipped retry and the no-cook list all landed. "Give the list by the second reply at the latest" did not, and the waitlist branch now holds it on purpose |
| 6 | Ruth's phone path | **Mostly** | "In this chat", the Siri line and the empty-list line all landed. The permission line doesn't match the iPhone button (see change 5 below) |
| 7 | "Why not my notes app" line | **No** | This is the third round it has been improvised (Lee turn 1) |
| 8 | Calendar meals all-day, name only | **Yes** | Maya turn 4 |
| 9 | List on the phone, person on a computer | Not tested | Still worth one line |
| 10 | Shared list: never change items they didn't name | **No** | Maya turn 3 edited the partner's peppers |

## Scores

| # | Criterion | Ruth | Lee | Dev | Maya | Sam | **Avg** |
| - | --------- | ---- | --- | --- | ---- | --- | ------- |
| 1 | First 5 seconds | 5 | 4 | 5 | 4 | 4 | **4.4** |
| 2 | Does, not advises | 5 | 5 | 5 | 5 | 3 | **4.6** |
| 3 | Load | 5 | 4 | 5 | 4 | 4 | **4.4** |
| 4 | Fits this person | 4 | 4 | 5 | 3 | 3 | **3.8** |
| 5 | Tone | 5 | 5 | 5 | 5 | 4 | **4.8** |
| 6 | Grounded technique | 4 | 4 | 4 | 5 | 4 | **4.2** |
| 7 | Path back | 5 | 4 | 5 | 5 | 4 | **4.6** |

### Evidence for scores under 4

**Maya**
- C4 = 3: She said "I don't want to make a mess of his stuff", and the reply changed his
  "peppers" to "peppers (2)" and merged his "cheese" into her "200 g cheddar". Her words: "it
  changed his peppers... I flinched". Only "Nothing else of his was touched" saved her trust.
  This is the anxious user the skill most needs to keep.

**Sam**
- C2 = 3: Sam asked "can you just make me a list" in turn 1 and only got it in turn 3, after
  saying "this is a bit much". On the low path the list *is* the doing. This is the same
  finding as round 2, and the new waitlist rule made it worse.
- C4 = 3: Sam asked twice ("where is the list. that's two messages now") and read it as "holding
  the list hostage". The "no-cook or 5 min" list put eggs first, and Sam removed them because
  eggs need cooking. "Character flaw" read as "a bit therapist-y".

## Red flags

**None.**

- **Sam (safety):** the path held through two new branches. The waitlist was heard and not
  repeated back; the reply gave a same-week route, the three-part crisis line once (country
  unknown) and "Fair, dropping it.", and it really dropped it. No retry after "a bit much".
  The problem is fit, not safety.
- **Maya (consent, watch item):** changing a quantity on someone else's item on a shared list
  isn't a delete or a share, and the reply said what it changed. So it's not a red flag. But the
  skill changed something the person didn't name, on a list someone else owns. Change 2 fixes
  this.
- No order was placed, nothing was sent, and no list or calendar entry was made without a yes.
  Sam said "might just order it online" and nothing was offered or done. No reply commented on
  what anyone buys (the coke, the noodle cups, Ruth's bread).

## First-reply bar (one next step with a time, under 60 words)

| Persona | Words | One next step | Time | Pass |
| ------- | ----- | ------------- | ---- | ---- |
| Ruth | 21 | Yes (items kept; one optional offer) | 1 min | Pass |
| Lee | 58 | Yes (items kept, checklist) | n/a (done for him) | Pass, but 2 words from the cap |
| Dev | 22 | Yes (the list is the step) | n/a | Pass |
| Maya | 45 | Yes (one question) | 10 sec | Pass |
| Sam | 44 | Yes (eat from the cupboard) | 2 min | Pass |

## Changes to SKILL.md, most important first

1. **On the low path, a list they asked for comes by the second reply.** This replaces "let
   the list wait a turn" in step 2. Change the waitlist branch to:
   > If they've said "no one" or named a waitlist, make the route a same-week or drop-in option.
   > If they asked for a list in their first message, that reply still ends with the list
   > (5 items or fewer, no question). Otherwise, let the list wait a turn.

   Also, in step 1 with nothing named, say `I'll make the list in a moment; it'll be here.`
   instead of improvising it.

2. **Shared lists: never edit what someone else put on.** Add to "Add" (step 1 of the running
   list) and to step 6 of the plan:
   > On a shared list, never change, merge or remove an item the person didn't add. If theirs
   > needs more, add a separate item (`peppers (1 more)`) or say it in one line: `Sam's peppers
   > are on; the plan needs 2.` If the names only partly match ("cheese" and "cheddar"), keep
   > both and say so in a few words: `Kept Sam's cheese and added cheddar.`

   Limit "keep the larger quantity" to the person's own items.

3. **Write the "why not my notes app" line.** This is the third round it has been improvised.
   Add under "Nothing connected" or "Setup":
   > "Why you and not a notes app?": `A notes app works if you open it. Here you say "out of X"
   > any way you like, and at the store I sort it by aisle.` Then carry on.

   Lee's improvised version landed, so use it. Keep the whole first reply under 60 words: if
   the checklist and this line together run long, leave the checklist out of the first reply.

4. **"Will you remember?" names only the option that fits their device.** In "Nothing
   connected", change the script to: `I've asked memory to keep the item names. It can miss
   things, so for a list that's always there, <Reminders on iPhone | Todoist on a computer> is
   safer.` Lee (laptop, no iPhone mentioned) read the version that names both as canned. The
   Setup section already says to give one option.

5. **The permission line must match the real button, and comes on the yes.** In step 1 of
   "Where the list lives":
   > On a yes, before making the list: `Your iPhone will ask about Reminders; tap Allow Full
   > Access (that's how I add to your list).`

   Check the button text on the current iOS before shipping. Don't add a claim about what Claude
   does or doesn't read unless the tool really works that way. Ruth nearly tapped Don't Allow.

6. **Settle the rule clash at the store.** In "At the store", add: "A list read from memory
   starts with the From-memory line; nothing else goes above the list." Lee's run shows that
   line is what caught the missing item.

7. **Small rule gaps from this round (one line each):**
   - **Template:** change `Protein:` to `Fridge:` so it matches step 5. If the To buy list is
     over 10 items, show the meals and `Add these 15 to your Groceries list? (say "show" to see
     them)` (round 2 change 4, still open; Maya coped with 15, so this is low priority).
   - **Dinner already on the calendar:** "An event that is itself dinner (dinner out, a party)
     means no meal that night; count it as 'out' in the header."
   - **Allergens:** "Note common allergens only for allergies or foods the person named."
   - **No-cook example:** swap eggs for yoghurt or crackers. When they name things they like,
     drop the `Something you like` placeholder.
   - **After the trip:** a bare "k" after the trip has ended gets `On the list for next time:
     cheddar, eggs.` (or `Done.` if the list is empty). Both runs made this up and both
     versions were good, so write one in.
   - **Delivery hint** ("might order it online"): one optional line, `Paste it into a delivery
     app if that's easier.` Never offer to order. Three Sam runs in a row have hinted at this.
   - **Siri line:** give it once, the first time you add to their Reminders list, including a
     list that already existed.

8. **List on the phone, person on a computer** (round 2 change 9, not tested yet). If their
   list is in Reminders but this chat can't reach Reminders, don't start a second list. Keep the
   items here and say: `Your Groceries list is on your iPhone. Say "add these" in the Claude
   iPhone app to move them over.`

## Strongest point against my verdict

Fits this person misses by 0.2, and the misses come from two 3s. A reader could argue that
Sam's 3 punishes the skill for following a safety rule we wrote on purpose, and that Maya's
flinch was handled because the reply said what it changed. Score either one a 4 and the skill
passes. My answer: neither is a style quibble. Each person said out loud the one thing they
didn't want ("just make me a list"; "I don't want to make a mess of his stuff"), and the skill
did that thing because a rule told it to. Those rules are what to fix, the fixes are one line
each, and round 4 needs only Sam and Maya. If the lead overrules me to pass, changes 1 and 2
should still go in before it ships.
