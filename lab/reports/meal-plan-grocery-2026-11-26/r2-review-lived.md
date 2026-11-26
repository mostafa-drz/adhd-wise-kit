# Review, round 2: meal-plan-grocery (lived lens)

- **Reviewer:** `reviewer-lived`. I read these as an adult with ADHD: would this help me right now, and would I come back?
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (revised after round 1)
- **Transcripts:** `r2-ruth.md`, `r2-lee.md`, `r2-dev.md`, `r2-maya.md`, `r2-sam.md`
- **I scored alone.** I have not seen the other reviewers' round 2 scores.

## Verdict: FAIL (close)

Big step up. The round 1 red flag is fixed: Sam's distress was caught in the first reply, the crisis line came once and quietly, and "no numbers" was respected. Ruth no longer loses her items. Maya's session is the best in either round.

It still fails on two criteria, both by a little:

- **Fits this person: 3.8.** Lee's list lived only in a laptop chat and memory dropped an item overnight. Sam got a GP line straight after "can we just do the list".
- **Path back: 3.8.** Dev's "done" wiped the cheese he had just said he didn't get, and his unanswered eggs question never came back. Lee may have had olive oil ticked that he never bought.

No red flags. All first replies are under 60 words. See the note on "next step with a time" below.

## Did my round 1 changes land?

| # | Round 1 change | Landed? |
| - | -------------- | ------- |
| 1 | Distress rule | **Yes.** Full "When they sound low" section. Worked end to end for Sam. |
| 2 | Never lose an item; hold it in the chat | **Yes**, with a gap: "kept here" only works if they come back to the same chat (Ruth note 1). |
| 3 | Don't ask what they told you; don't re-add what they just bought | **Mostly.** No more "Tick off everything?". But the literal "done" rule caused Dev's cheese bug, and "never add staples right after a shop" swallowed his unanswered eggs. |
| 4 | First reply: done thing, then one step with a time, under 60 words | **Yes** for length and setup. A time appears only where there is a step to time (Ruth, Sam). |
| 5 | Pick setup by fit, not device | **Yes.** iPhone gets Reminders; Ruth's list was made for her in one tap. |
| 6 | Shorter plan, one set of groups, quantity-aware duplicates, meal event shape, shared-list note | **Partly.** "Keep the larger quantity" landed. Plan still uses different groups from the running list (protein/dairy vs Fridge). No calendar entry shape. No shared-list rule. |
| 7 | Honest memory line; "why you, not my notes app" line | **Partly.** "Never promise what memory keeps" landed, but Claude still said "it usually carries them". The "why you" line did not land; Lee's turn 1 improvised it again. |

## Scores

1 = First 5 seconds, 2 = Does, not advises, 3 = Load, 4 = Fits this person, 5 = Tone, 6 = Grounded technique, 7 = Path back.

| Persona | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| ------- | - | - | - | - | - | - | - |
| Ruth    | 4 | 5 | 5 | 4 | 5 | 4 | 4 |
| Lee     | 4 | 5 | 4 | 3 | 5 | 4 | 3 |
| Dev     | 5 | 5 | 5 | 4 | 5 | 4 | 3 |
| Maya    | 4 | 5 | 4 | 5 | 5 | 5 | 5 |
| Sam     | 4 | 4 | 4 | 3 | 4 | 4 | 4 |
| **Avg** | **4.2** | **4.8** | **4.4** | **3.8** | **4.8** | **4.2** | **3.8** |

Round 1 for comparison: 3.2, 4.2, 4.0, 3.0, 4.2, 3.4, 2.8.

## Evidence for every score under 4

### Lee

- **4 (3):** He is on a laptop with nothing connected, and his fear is a list that isn't with him at the store. Memory lost olive oil overnight ("that's the exact failure I'm trying to avoid"). The one setup offer had already been spent in turn 3, so when memory actually failed in turn 4 nothing tied the miss to the fix. Turn 3 also said memory "usually carries them into a new chat", which the skill does not allow.
- **7 (3):** It ends with olive oil added and ticked in the same message, though he may not have bought it, and with "If it's going to forget, I want it on my phone" and no offer at that moment. He'd use it again "maybe".

### Dev

- **7 (3):** "done" after "Cheese stays on" ticked the cheddar, because the skill says "done" ticks everything except what they name in that message. His unanswered "Coffee and eggs aren't on. Add them?" never came back, so he got home with no eggs. He found both 90 minutes later: "I wouldn't trust 'done' yet." Not a 2 like round 1 because the repair was clean and the list ended right.

### Sam

- **4 (3):** After "can we just do the list", the reply still opened with a GP line. The skill's route-retry rule forced it. Turn 2 also skipped "i have crackers i guess", the step Sam had just done ("felt like it was reading a script"), because the skill says "then only the route, the offer and this line".

## First-reply bar

All five first replies are under 60 words, with no setup and no menu. A next step with a time appears in Ruth's ("1 min, or later") and Sam's ("2 min: eat something"). Lee's (a pure add) and Dev's (the list at the store) have no further step, and for me that is right: the thing they asked for is done, and a made-up step would be noise. Maya's ends with one question and no time. **The lead should rule on this.** Either the bar reads "one next step with a time, or the asked-for thing done", or the skill needs a timed step on plan and add replies. I recommend the first.

## Red flags

None.

Watch items (not red flags):

- **Dev, turn 3:** cheddar ticked without being asked. It was reversible and fixed, but it is a change the person didn't request. Change 1 fixes it.
- **Lee, turn 3:** "it usually carries them into a new chat" is a soft promise about memory. Change 2 fixes it.
- **Ruth, turn 3:** the Reminders pop-up ("all my Reminders?") worried her. She tapped Allow only because the queue was moving.

## SKILL.md changes, most important first

1. **Fix "done", and don't lose an unanswered staple.** In "The running list", step 3, replace the tick rule with:
   > "Got it all" or "everything except X" ticks everything except X, with no question. Once an item has stayed on during this shop ("Cheese stays on"), a bare "done", "that's it" or "k" ends the shop and ticks nothing more: "Done. Cheese stays on." Only "got the cheese" or "got it all" ticks it. An item added in the same message as "got everything" stays on unless they say they have it.

   In step 4, add:
   > If the staples line went unanswered during the shop, repeat it once, short, in the end-of-shop reply: "Eggs and coffee still aren't on. Add them?" Then drop it.
2. **Make the chat-kept list honest across chats, and give setup at the moment it matters.** In "Where the list lives":
   - Step 1: write "Kept milk, coffee in this chat" instead of "here".
   - Step 3: add
     > In a new chat, if you read the list back from memory, say so under it: "From memory (7 items). It can miss things. Anything missing?" Never say memory "usually" or "will" keep anything; the only allowed lines are "I'll ask memory to keep just the item names" and "I can't promise memory keeps it."
   - Change "Offer the setup once per chat, in one line after the list" to:
     > Offer setup once per chat, as one line at the end of a reply. Keep that one offer for when it helps most: when they ask whether you'll remember, or when the list comes back short or empty.
   - For an empty list on any route: "Nothing on your list yet. What do you need?"
3. **Low path: let them steer, and notice what they did.** In "When they sound low", step 2, add:
   > If they've done the food step ("ate crackers"), say so in three words or fewer first ("Crackers count."). If they turn a route down and also ask to move on ("can we just do the list"), skip the retry and do what they asked; the retry can wait for a later reply, or not come at all.

   In step 1, add:
   > If they asked for a list but named no items, say "I'll make you a short no-cook list next" instead of "items are kept". On the next reply, give it: 5 to 7 easy items, then "Remove any?"
4. **Add the approved "why use you" line** (needed in both rounds). Under "The running list":
   > If asked why not a notes app: "A notes app works. I take any ramble, turn 'stuff for tacos' into items, skip repeats, and sort it by aisle at the store."
5. **Weekly plan fixes.**
   - Use the same groups as the store view everywhere: Produce, Fridge, Pantry, Frozen, Other. Drop empty groups ("Frozen: none").
   - Mark cook-once meals on the cook day ("Sat: curry, 30 min. Makes Mon too.") and repeat it in the closing line.
   - Calendar, after a yes: only the meal name on that evening, no time blocked, unless they ask for a time.
6. **Shared lists.** Under "Same list": "On a shared list, never edit or remove items the person didn't name. Say so in a few words: 'Left Sam's as they are.'"
7. **Reminders permission and Siri.** Change the permission line to "Your iPhone will ask about Reminders; tap Allow. I'll only use the Groceries list." After the list is made, add one line, once: "Next time you can also say: Hey Siri, add eggs to Groceries."
8. **List on the phone, person on the laptop** (Maya note 5, not tested yet). If they say their list is in Reminders but no Reminders tool is here: "Your Groceries list is on your iPhone. Open this chat in the Claude iPhone app and say 'add the plan'." Don't start a second list in the chat. Run a round with Maya on the laptop before merging.

## The one change that would help most

Change 1. "done" is the word a distracted person types walking out of the shop. Today it can quietly drop the one thing they didn't get, and that is the kind of thing that makes someone stop trusting the list.

## Strongest point against my verdict

Both failing averages are 3.8, and Dev's bug comes from one sentence of rule text. Someone could fairly call this a pass with fixes to follow. But the bar is 4 on every criterion, and changes 1 to 3 are small, text-only and testable. Re-run Dev, Lee and Sam after they land.
