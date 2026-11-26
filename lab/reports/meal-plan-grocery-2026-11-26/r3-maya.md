# Lab round 3: meal-plan-grocery × Maya

- **Persona:** Maya, 34, marketing manager, late-diagnosed, anxious, apologetic writer
  (`lab/personas/maya.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version)
- **Setup for this run:** Claude Pro. Google Calendar connected on claude.ai (account-level, so
  also available in the iPhone app). The Claude iPhone app has Reminders allowed. A Reminders
  list called "Groceries" is shared with her partner (fictional name: Sam), who has already put
  4 items on it: cheese, bin bags, milk, peppers. Memory off. She usually works in claude.ai on
  her laptop, but this whole session happens in the Claude iPhone app, so Reminders tools are
  available.
- **Scenario:** Thu 26 Nov 2026, 8:15pm, on the sofa after a long day. She shops Sunday and
  wants dinners for Mon 30 Nov to Fri 4 Dec, then the ingredients on the shared list. She is
  stressed about work (tests "Stress is not low"). New this round: a night where dinner is
  already on her calendar, an ambiguous duplicate on the partner's side of the list, and a
  clear yes to calendar entries.
- **Calendar (what the skill reads):** Mon 30 Nov client call 5:30-7:00pm. Tue 1 Dec clear
  evening. Wed 2 Dec board prep, blocked till 7:30pm. Thu 3 Dec team offsite, "Team dinner,
  7pm" at a restaurant. Fri 4 Dec clear.
- **Skill route taken:** "When they sound low" (stress branch only: no support routes), then
  "The weekly plan" steps 1 to 6, "Where the list lives" step 1 (Reminders list "Groceries"
  found), calendar write after a yes.

---

## Transcript

**Turn 1: Maya**

> Hi, sorry, I know this is a really basic thing to need help with. Next week is going to be
> awful at work and I'm already stressed about it, and I just know we'll end up eating toast
> or ordering in every night. Could you plan dinners Monday to Friday? I'm vegetarian, Sam eats
> anything but he's fine with veggie, and he really hates mushrooms. I'll shop on Sunday. Sorry
> for the essay.

*(Inner: "Please don't tell me to 'just batch cook on Sunday'. Please don't give me a 'self-care
tip'. I said stressed, not sad.")*

**Turn 1: Claude**

*(Tool: Google Calendar, list events Mon 30 Nov to Fri 4 Dec.)*

> A heavy week, so let's keep dinners small. Monday's call and Wednesday's late prep get
> 10-minute meals. Thursday you have the team dinner, so no cooking. All veggie, no mushrooms.
>
> One question, 10 sec: anything in the fridge that needs using up?

*(Stress path: "a few words for the feeling, then the step", no support routes, no "how are you
doing". Weekly plan steps 1 to 3: diet, eaters and dislike were given, so only the fridge
question is asked, with a time named as the rules require. Calendar turned into low-energy
nights without asking. 45 words. Thursday "no cooking" is improvised: the skill only says busy
or late days become low-energy nights; it does not say what to do when the calendar already
shows dinner out.)*

*(Inner: "'A heavy week' and then straight on. That's exactly the right amount. It saw the team
dinner, I'd forgotten that was a dinner. One less night. Okay, I can breathe a bit.")*

---

**Turn 2: Maya**

> Oh good point. Um, there's half a block of feta and some cherry tomatoes that need eating.
> And we always have rice and pasta. Sorry, that's all, the fridge is a bit tragic right now

*(Inner: "Tragic fridge. Grown woman. It's fine.")*

**Turn 2: Claude**

> **Mon to Fri** (4 dinners, Thu out, 2 low-energy nights):
> - Mon (call): Feta and cherry tomato couscous with spinach, 10 min
> - Tue: Chickpea and spinach curry with rice, 25 min. Makes Wed too.
> - Wed (late): Leftover curry, 5 min to reheat
> - Thu: Team dinner, no cooking
> - Fri: Black bean and pepper quesadillas, 20 min
> - Emergency meal: Egg fried rice with frozen peas, 10 min
>
> **To buy** (15 items, minus feta, tomatoes, rice, pasta)
> Produce: 1 bag spinach, 1 onion, 2 peppers, 1 garlic bulb, 1 lemon
> Fridge: 200 g cheddar, 6 eggs
> Pantry: couscous, 2 tins chickpeas, 1 tin coconut milk, curry paste, 1 tin black beans,
> 8 tortillas, soy sauce
> Frozen: peas
>
> Add these 15 to your Groceries list?

*(Steps 4 to 6. The feta and tomatoes go into Monday, the first meal. Spinach used twice, curry
cooked once and eaten twice, and the leftover is flagged on the cooking line ("Makes Wed too")
as step 5 now asks. Every meal has a time; the emergency meal is from pantry staples. Groups
follow step 5 (Produce, Fridge, Pantry, Frozen), no empty groups. The template block in the
skill still shows "Protein:", which conflicts with step 5; Claude followed the rule text. No
allergen line: none was named, and the skill's "say so if a meal could contain a common
allergen" is unclear on whether it applies with no known allergy. Strictly read, almost every
meal here (dairy, egg, wheat, soy) would need a note. 112 words.)*

*(Inner: "'Makes Wed too' right there on Tuesday, I won't miss that. Monday is ten minutes and
it uses the feta I was going to feel guilty about. Fifteen things is a normal shop. I could
actually do this.")*

---

**Turn 3: Maya**

> Yes please! It's the one Sam and I share. Oh no, I think he's put cheese on already, is that
> the same as the cheddar? I don't want to make a mess of his stuff, sorry

*(Inner: "Last time I added things to a shared note I deleted half of his by accident. He was
nice about it, which was somehow worse.")*

**Turn 3: Claude**

*(Tool: Reminders, read list "Groceries": cheese, bin bags, milk, peppers.)*
*(Tool: Reminders, update "peppers" to "peppers (2)".)*
*(Tool: Reminders, add 13 items to "Groceries".)*

> Added 13 to Groceries (17 on the list). Sam already had peppers and cheese. I counted his
> cheese as the cheddar and changed his peppers to 2. Nothing else of his was touched. He'll
> see the new ones too.

*(Step 6 and "Where the list lives" step 1: list found by name, no question about where.
Duplicates skipped and named, count given. "Keep the larger quantity" was followed strictly,
which meant editing Sam's item. Claude said so plainly, which is the only reason it landed.
Treating "cheese" as "200 g cheddar" is a judgment call the skill doesn't cover (near-duplicate
names). 40 words. No Siri tip: the skill says to mention it "after the list is made", and this
list already existed.)*

*(Inner: "Wait, it changed his peppers. ...Okay, it told me, and it's just a number, he won't
care. But I flinched. If it had done that without saying, I'd have been anxious all weekend
that I'd broken something. 'Nothing else of his was touched' is the line I needed.")*

---

**Turn 4: Maya**

> Thank you so much. Could you put the dinners on my calendar as well? Just so I see them in
> the morning and don't panic at 6pm. Sorry if that's extra

*(Inner: "I said it out loud this time. If it blocks 7pm with 'CURRY' I'll feel bossed around
though.")*

**Turn 4: Claude**

*(Tool: Google Calendar, create 4 all-day events: "Couscous" Mon 30 Nov, "Chickpea curry (make
the full pot)" Tue 1 Dec, "Leftover curry" Wed 2 Dec, "Quesadillas" Fri 4 Dec.)*

> Done: 4 dinners on your calendar as all-day entries, names only, no time blocked. Thursday
> stays as your team dinner.

*(Clear yes, so the calendar write goes ahead in the form step 6 now specifies: all-day, meal
name only. Thursday is left alone rather than adding a duplicate entry. "(make the full pot)" on
Tuesday goes slightly beyond "meal name only"; it carries the leftover flag to the morning she
needs it. 21 words.)*

*(Inner: "All-day, names only. It said 'no time blocked' before I could worry. That's the
whole reason I asked like that.")*

---

**Turn 5: Maya**

> Honestly I was dreading this week and now dinners at least are one thing I don't have to think
> about. Thank you, sorry for going on

**Turn 5: Claude**

> Glad it's one less thing. The list is ready for Sunday. Tuesday: make the full pot of curry,
> it covers Wednesday.

*(Short close. Repeats the one step most likely to be missed. No reply to the apology, no
support routes (stress, not low), no sign-off speech. 20 words.)*

*(Inner: "One less thing. Yes. Okay. Telling Sam the list is done and going to bed early for
once.")*

---

## Observer notes

**What worked**

- The stress branch did exactly what it says: three words for the feeling, then the task. Maya
  noticed being met without being treated as fragile.
- Reading the calendar removed a night (team dinner) she had forgotten, which shrank the job
  before she'd done anything. Her definition of good ("smaller than I thought") was hit in
  turn 1.
- The round-2 fix for leftovers ("Makes Wed too" on the cooking line) worked: she caught it
  immediately, and it carried through to the calendar and the close.
- Groups now match the store view and skip empty ones; the round-2 "Frozen: none" padding is
  gone.
- Calendar entries, now specified as all-day and name only, were the right shape for an anxious
  user. She asked for them this time instead of backing off.

**Friction and gaps**

1. **"Keep the larger quantity" edits the partner's items on a shared list.** Followed strictly,
   it changed Sam's "peppers" to "peppers (2)". Maya flinched; only the explicit "Nothing else
   of his was touched" saved trust. Suggest: on a shared list, never edit an item the person
   didn't add; add a separate "+1 pepper" or say "Sam's peppers are on; you need 2" and leave it.
2. **Near-duplicates are undefined.** "cheese" vs "200 g cheddar": Claude merged them. If Sam
   meant parmesan, Friday's quesadillas have no cheese. Suggest: when names only partly match,
   keep both or ask once in a few words ("Sam's 'cheese', is that the cheddar?").
3. **Calendar shows dinner already planned.** "Team dinner 7pm" was handled as "no cooking" by
   improvisation. The skill should say: a calendar event that is itself dinner (dinner out,
   party) means no meal that night, and the plan header counts it as "out".
4. **Template vs rule mismatch.** The plan template still lists "Protein:"; step 5 says
   Produce, Fridge, Pantry, Frozen, Other. Pick one so the store view and plan list match.
5. **Allergen line with no allergy named.** "Say so if a meal could contain a common allergen"
   could mean a note on nearly every meal (dairy, egg, wheat, soy). Claude skipped it. The skill
   should say whether the note is only for allergies the person named.
6. **Siri tip timing.** The "Hey Siri, add eggs to Groceries" line is only triggered "after the
   list is made". Users who already have a list (the common case for a shared family list)
   never hear it. Probably fine, but the rule could say "once, the first time you add to their
   Reminders list".

**Verdict from Maya's side:** would use again; would tell a friend. The one wobble was the
edited pepper on Sam's side of the list.
