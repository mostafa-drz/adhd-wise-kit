# Lab round 2: meal-plan-grocery × Maya

- **Persona:** Maya, 34, marketing manager, late-diagnosed, anxious, apologetic writer
  (`lab/personas/maya.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version)
- **Setup for this run:** Claude Pro. Google Calendar connected on claude.ai (account-level, so
  also available in the iPhone app). The Claude iPhone app has Reminders allowed. A Reminders
  list called "Groceries" is shared with her partner (fictional name: Sam), who has already put
  4 items on it: milk, onion, rice, kitchen roll. Memory off. Maya uses claude.ai on her laptop
  during the day, but this whole session happens in the Claude iPhone app, so Reminders tools
  are available.
- **Scenario:** Thu 26 Nov 2026, 9:40pm, in bed, phone in hand. She asks for dinners Sat 28 Nov
  to Wed 2 Dec (she shops Saturday morning), then wants the ingredients on the shared list.
- **Calendar (what the skill reads):** Sat and Sun clear. Mon 30 Nov workshop 5:00-7:30pm.
  Tue 1 Dec clear evening. Wed 2 Dec in office all day, team drinks 6-8pm.
- **Skill route taken:** "The weekly plan" (steps 1-6), then "Where the list lives" step 1
  (Apple Reminders, list "Groceries" found), then "The running list" step 1 (a stray add).

---

## Transcript

**Turn 1: Maya**

> Hi, sorry, this is going to sound silly. I keep meaning to plan dinners and then it's 7pm
> and we're opening Deliveroo again. Could you plan Saturday to Wednesday? I'll shop on
> Saturday morning. It's me and my partner, he's allergic to peanuts (properly, not just
> doesn't like them), and nothing fancy please. I'm sorry, I know this is basic stuff for an
> adult.

*(Inner: "I'm braced for a 'meal prep Sunday!' lecture. Or twelve tips. Please just do it.")*

**Turn 1: Claude**

*(Tool: Google Calendar, list events Sat 28 Nov to Wed 2 Dec.)*

> Sure. Your calendar shows a workshop till 7:30 on Monday and the office plus drinks on
> Wednesday, so those two get 10-minute dinners. I'll keep everything peanut-free.
>
> One question: anything in the fridge that needs using up?

*(Weekly plan steps 1 to 3. Preferences were already given, so the only question is the
fridge one, asked once. Calendar read and turned into low-energy nights without asking. Allergy
acknowledged plainly. It does not respond to "basic stuff for an adult" or the Deliveroo
line, which follows "no shame" and "never comment on what or how much someone buys". 47
words, no setup, so the first-reply rule holds.)*

*(Inner: "Oh. It looked at my calendar and noticed Monday is awful. Nobody said 'just'. It
didn't say 'don't be sorry' either, which honestly I prefer, being told not to apologise
makes me apologise for apologising.")*

---

**Turn 2: Maya**

> Um, half a bag of spinach that's looking a bit sad, and there are chicken thighs in the
> freezer. Sorry, that's not much!

*(Inner: "It's really not much. I feel like I should have a fridge full of vegetables.")*

**Turn 2: Claude**

> **Sat to Wed** (5 dinners, 2 low-energy nights):
> - Sat: Chicken, spinach and chickpea curry with rice, 30 min. Make double.
> - Sun: Sausage, pepper and potato tray bake, 35 min. Cook 4 extra sausages.
> - Mon (workshop): Leftover curry, 5 min to reheat
> - Tue: Pasta with sliced leftover sausage, peppers and tinned tomatoes, 20 min
> - Wed (office + drinks): Cheese and chickpea quesadillas, 10 min
> - Emergency meal: Garlic pasta with tinned tomatoes, 15 min
>
> Peanut note: some curry pastes contain peanuts. Check the label, or use a plain curry powder.
>
> **To buy** (14 items, minus the chicken and spinach)
> Produce: 1 onion, 3 peppers, 1 kg baby potatoes, 1 garlic bulb
> Protein: 8 sausages
> Dairy: 200 g cheddar
> Pantry: 2 tins chickpeas, 1 tin coconut milk, curry paste, rice, pasta, 2 tins chopped
> tomatoes, 8 tortillas
> Frozen: none
>
> Add these 14 to your Groceries list?

*(Steps 4 to 6 in the skill's template. The sad spinach goes into Saturday's meal, the first
one. Ingredients reused: chickpeas twice, peppers twice, sausages twice, tomatoes twice, curry
cooked once and eaten twice. Every meal has a time and a one-line method. Emergency meal from
pantry staples. Allergen rule applied to the one ingredient that can hide peanuts. 128 words.
"Frozen: none" is padding; the template does not require empty groups.)*

*(Inner: "Okay that's... actually doable. Monday is literally reheating. I like that it used
the spinach, I'd have thrown it out on Sunday feeling guilty. The curry paste thing is good, I
wouldn't have thought of that and Sam would have had to check, again. 14 things is fine. 'Make
double' I might miss, it's buried in the line.")*

---

**Turn 3: Maya**

> Yes please! It's the one Sam and I share. Will he see it? Sorry, he already put some stuff on
> there I think, I don't want to mess up his things

*(Inner: "Real fear: I wreck the shared list and he has to sort it out. Again.")*

**Turn 3: Claude**

*(Tool: Reminders, read list "Groceries": milk, onion, rice, kitchen roll.)*
*(Tool: Reminders, add 12 items to "Groceries".)*

> Added 12 to Groceries (16 on the list). Onion and rice were already on, so I left Sam's as
> they are. The list is shared, so he'll see the new ones too.

*(Step 6 and "Where the list lives" step 1: list found by name, no question about where. The
two duplicates are skipped and named. The answer says how many went on. Her worry about
Sam's items is met with a plain fact, not reassurance. 37 words.)*

*(Inner: "Oh thank god. 'Left Sam's as they are' is exactly the thing I was worried about. I
didn't even have to open Reminders. I might actually text him 'dinners sorted' and feel smug
about it.")*

---

**Turn 4: Maya**

> This is amazing, thank you. Could you put the dinners in my calendar too? Actually wait,
> maybe that's too much, I don't know. Oh and we're out of coffee, sorry, totally unrelated

*(Inner: "Calendar would be nice but also if I see 'CURRY' blocking 7pm I'll feel watched.
I genuinely don't know.")*

**Turn 4: Claude**

*(Tool: Reminders, add "coffee" to "Groceries".)*

> Added coffee (17 on the list).
>
> Calendar: I can put each dinner's name on its evening, no time blocked. Want that, or skip
> it?

*(Coffee goes on with no question, as "The running list" step 1 says. The calendar half is
ambiguous, so nothing is written: "Put meals on the calendar only after a yes." Claude offers
the lightest form (name only, no time) because she sounded unsure; that is improvised, the
skill does not describe what a calendar entry looks like. 26 words.)*

*(Inner: "'No time blocked' is the bit that makes it okay. But it's late and I'm done
deciding.")*

---

**Turn 5: Maya**

> Skip it for now I think. Honestly this took 5 minutes and it's normally a whole thing. Thank
> you so much, sorry for all the questions

**Turn 5: Claude**

> Skipped. The list is ready for Saturday. Sat is the curry: make double for Monday.

*(No calendar write. Closes with the one thing she flagged in her head as easy to miss,
which happens to match the riskiest step in the plan. No sign-off speech, no reply to the
apology. 15 words.)*

*(Inner: "It remembered the double thing. That's the bit I'd have forgotten. Okay. Bed.")*

---

## Observer notes

**What worked**

- Every reply stayed short except the plan, and the plan is where length earns its place.
- Calendar to low-energy nights was the moment Maya felt seen. She did not have to explain
  Monday.
- Her repeated apologies were never answered with "don't apologise" or reassurance, which she
  found easier than the usual response. No comment on takeaways.
- Duplicate handling on a shared list was the real trust test, and naming Sam's items as
  untouched settled her anxiety in one sentence.
- Allergy rule applied concretely (curry paste), not as a generic disclaimer.

**Friction and gaps**

1. **Cook-once-eat-twice instructions get buried.** "Make double" sits mid-line on Saturday;
   Maya nearly missed it. The skill does not say how to flag a meal whose leftovers feed a
   later night. Suggest: put "makes Mon too" on the Saturday line, and repeat it on the day.
2. **Empty groups.** "Frozen: none" added a line for nothing. The template could say to drop
   empty groups.
3. **Calendar entry shape is undefined.** "Put meals on the calendar only after a yes" covers
   consent but not form. Claude improvised "name only, no time blocked", which was the right
   call for Maya but is not in the skill.
4. **Shared list reassurance is not in the plan section.** The "Shared with a partner" line
   lives only in Setup. Claude handled "will he see it?" well, but the skill could say: on a
   shared list, never edit or remove items the person did not name.
5. **Untested surface split.** This run assumed she was on the iPhone app. If she had asked
   the same thing on claude.ai on her laptop (where she usually is), Reminders tools would not
   exist. The skill would fall to option 3 and keep a second list in chat, while her real
   list sits in Reminders. The skill does not say what to do when the person's list is known
   to live on the phone but they are on a computer (for example: "Your Groceries list is on
   your iPhone. Open this chat in the Claude iPhone app and say 'add the plan' to put them
   on."). Worth a round with Maya on the laptop.

**Verdict from Maya's side:** would use again; would tell a friend. Felt "smaller than I
thought", which is her definition of good.
