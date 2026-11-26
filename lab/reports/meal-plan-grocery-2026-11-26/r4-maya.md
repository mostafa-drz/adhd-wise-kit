# Lab round 4: meal-plan-grocery × Maya

- **Persona:** Maya, 34, marketing manager, late-diagnosed (inattentive), anxiety alongside,
  long apologetic messages (`lab/personas/maya.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md` (current version),
  followed strictly for every Claude reply
- **Setup for this run:** Claude Pro. Google Calendar connected on claude.ai (account-level, so
  the iPhone app can read it too). The Claude iPhone app has Reminders allowed. A Reminders
  list called "Groceries" is shared with her partner (fictional name: Jonah), who has already
  put 5 items on it: milk, eggs, cheddar, bin bags, onions. Memory off. She normally works in
  claude.ai on her laptop; this session is in the Claude iPhone app, so Reminders tools are
  available.
- **Scenario:** Thu 26 Nov 2026, 9:40pm, in bed, phone only. She is tired, not distressed. She
  shops Saturday and wants dinners for Mon 30 Nov to Fri 4 Dec, then the ingredients on the
  shared list. New this round: she gives no diet info up front (tests "ask at most two
  questions"), she volunteers fridge leftovers in her answer, a partial-name match on the
  partner's side (onions vs red onions), and a question the skill does not cover (will her
  partner get notified).
- **Calendar (what the skill reads):** Mon 30 Nov offsite, back around 7:30pm. Tue 1 Dec clear
  evening. Wed 2 Dec 1:1 with her director 6:00-7:30pm. Thu 3 Dec dentist 5:15pm (done by 6).
  Fri 4 Dec clear.
- **Skill route taken:** "The weekly plan" steps 1 to 6, "Where the list lives" step 1
  (Reminders list "Groceries" found), "The running list" step 1 (a single add), calendar write
  after a yes. Not the low path: tired, no self-blame beyond the task.

---

## Transcript

**Turn 1: Maya**

> Hi! Sorry, this is probably a silly thing to ask an AI at 10pm. I keep meaning to plan
> dinners and then it's Wednesday and we're eating cereal again. Could you plan next week's
> dinners, Monday to Friday? And then I'd love it if the stuff could go on the Groceries list
> I share with Jonah, if that's even possible from here? No worries if not.

*(Inner: "Please don't send me a 'Meal Prep 101' with 12 tips. And please don't make me fill
in a form about macros.")*

**Turn 1: Claude**

*(Tool: Google Calendar, list events Mon 30 Nov to Fri 4 Dec.)*

> Yes, I can do both. Monday's offsite and Wednesday's late 1:1 get 10-minute dinners.
>
> Two questions, 15 sec: any foods to avoid, and is it just you and Jonah?

*(31 words. Weekly plan step 1: memory off and nothing given, so exactly two questions in one
message, with a time named. Step 2: calendar read without asking; two busy evenings become
low-energy nights. "Never only setup": the reply already shows the calendar work and answers
her "is that even possible". The fridge question (step 3) is held for the next turn so the
message stays at two questions. Thursday's 5:15 dentist is correctly not treated as late.)*

*(Inner: "Oh. It already looked at my week. I didn't have to explain Monday. Two questions,
fine, I can do two questions.")*

---

**Turn 2: Maya**

> Just the two of us! I really can't stand coriander, sorry, I know people love it. Jonah
> doesn't eat pork. Oh and there's half a bag of spinach and some feta and Greek yogurt in the
> fridge that I keep feeling guilty about, if that helps at all. Sorry, I'm rambling.

*(Inner: "I mentioned the spinach because it's been staring at me for four days. If it ignores
it I'll feel stupid for saying it.")*

**Turn 2: Claude**

> **This week** (5 dinners, 2 low-energy nights):
> - Mon (offsite): Spinach and feta omelette with toast, 10 min. Eggs, spinach, feta, done.
> - Tue: Chicken thigh traybake with sweet potato and red onion, yogurt-garlic sauce, 35 min.
>   Makes Wed dinner too.
> - Wed (late 1:1): Leftover chicken wraps with spinach and yogurt, 10 min.
> - Thu: Pasta with spinach, feta, cherry tomatoes and garlic, 20 min.
> - Fri: Chickpea and coconut curry with rice, 25 min. No coriander. Makes Sat lunch too.
> - Emergency meal: pasta with jarred pesto and a handful of spinach, 10 min.
>
> Uses up your spinach, feta and yogurt first. No pork, no coriander anywhere. Common
> allergens: eggs (Mon), dairy (Mon to Thu), gluten (toast, wraps, pasta).
>
> **To buy** (15 items)
> Produce: sweet potatoes 3, red onions 2, cherry tomatoes 1 punnet, garlic 1 bulb, spinach 1
> bag, lemon 1
> Fridge: chicken thighs 6, eggs 6
> Pantry: bread 1 loaf, wraps 1 pack, pasta 500g, chickpeas 2 tins, coconut milk 1 tin, curry
> paste 1 jar, rice 1 bag
>
> Add these 15 to your Groceries list?

*(Weekly plan steps 3 to 5 and the template. Step 3, "ask once" about the fridge, was
answered before it was asked, so the skill skipped it and built Mon, Wed and Thu around her
leftovers. Ingredients reused (spinach x4, yogurt x2, feta x2, chicken x2) so the list stays at
15. Each meal has a time and one line. Leftover flags on Tue and Fri. Spinach still on the
list because half a bag will not cover four meals; this is a judgement call the skill does not
spell out. Allergen line added per "say so if a meal could contain a common allergen". No
comment on her guilt about the spinach, no "you should".)*

*(Inner: "It used the spinach. It used ALL of it. And Wednesday is leftovers, so I literally
don't cook on my worst night. The allergen line is a bit much for me, but I get why it's
there. Fifteen items is fine.")*

---

**Turn 3: Maya**

> Yes please!! Will Jonah's stuff get messed up? He already put a few things on.

*(Inner: "Last time I tried an app that 'synced' it wiped his list and he was annoyed for a
day.")*

**Turn 3: Claude**

*(Tool: Reminders, read list "Groceries": milk, eggs, cheddar, bin bags, onions. Then
Reminders, add 14 items to "Groceries".)*

> Added 14 to Groceries (19 on the list). Eggs were already on from Jonah, so I left his.
> His onions stay as they are; red onions went on as their own item. Nothing of his was
> changed.

*(Weekly plan step 6 and running list step 1, shared-list rules: duplicate skipped and named,
partner's item untouched, partial match ("onions" vs "red onions") kept as two items. Eggs:
she needs 6, his item has no quantity, so the skill did not edit his item and did not add
"eggs, 6 more" either; it treated eggs as covered. The skill says "add the difference as its
own item" when quantities differ, but his item has no quantity, so there is no difference to
add. Defensible, but the rule does not say this case. Cheddar was not touched (nothing in the
plan needs it). No question asked; 41 words.)*

*(Inner: "'Nothing of his was changed.' That's the sentence I needed. I'm not going to have to
apologise to him tomorrow.")*

---

**Turn 4: Maya**

> Amazing, thank you. Sorry, one more: can you put the dinners on my calendar? But please no
> times or alarms, I swipe those away and then feel bad. Oh and we're out of dish soap.

*(Inner: "If it puts a 6pm 'COOK DINNER' alarm on my phone I will delete the whole thing.")*

**Turn 4: Claude**

*(Tool: Reminders, add "dish soap" to "Groceries". Tool: Google Calendar, create 5 all-day
events, Mon 30 Nov to Fri 4 Dec, titles only: "Spinach feta omelette", "Chicken traybake",
"Chicken wraps (leftovers)", "Spinach feta pasta", "Chickpea curry"; no reminders.)*

> Added dish soap (20 on the list). Your 5 dinners are on your calendar as all-day entries,
> meal name only. No times, no alarms.

*(Weekly plan step 6: calendar written only after an explicit yes, all-day, meal name only,
nothing blocked. Running list add in one line with the count, no question. "Adding items the
person just asked for needs no extra yes." 25 words. The Siri tip ("Hey Siri, add eggs to
Groceries") was not offered: the skill says to mention it once "after the list is made", and
here the list already existed. Unclear whether it should have come here.)*

*(Inner: "No alarms. It listened. Okay, this is the first evening admin thing this week that
didn't make me feel worse.")*

---

**Turn 5: Maya**

> This is honestly so helpful. Will Jonah get a notification that I added stuff? I don't
> want to spam him at 10pm lol

*(Inner: "Small thing, but I don't want him waking up to 15 pings and thinking I'm being
passive-aggressive about the shopping.")*

**Turn 5: Claude**

> I can't see his notification settings. Shared Reminders lists usually don't ping for each
> item; he'll see them next time he opens Groceries.

*(Not covered by the skill. The reply stays short and honest: it says what it can't see rather
than promising "he won't be notified". "Usually" is a hedge about Apple's behaviour, not about
memory, so it does not break the "never say memory usually keeps things" rule. No setup offer,
no extra tips, no closing question.)*

*(Inner: "Good enough. I'll just text him 'list's updated, sorry' tomorrow. Done. Going to
sleep.")*

---

## Persona's honest verdict

> "It did the scary bit, which for me is deciding. I said two things I was embarrassed about,
> the guilt spinach and not wanting alarms, and it just quietly used both. The only part I
> skimmed was the allergen line. I'd use this every Thursday."

Would she come back next week: yes. Would she pay for it on this showing: "probably, if it
remembers I hate coriander so I don't have to say it again." (Memory was off this run.)

## Rule check

| Rule                                                       | Held? | Note                                                                 |
| ---------------------------------------------------------- | ----- | -------------------------------------------------------------------- |
| First reply under 60 words, not only setup, time named     | Yes   | 31 words; calendar work shown; "Two questions, 15 sec"               |
| Weekly plan: at most two questions in one message          | Yes   | Fridge question skipped because she answered it unprompted          |
| Calendar busy/late days become low-energy nights           | Yes   | Mon and Wed; Thu 5:15 dentist correctly not counted                  |
| Every meal has a time and one line; emergency meal         | Yes   |                                                                      |
| Reuse ingredients, list minus what they have               | Yes   | 15 items; spinach still bought (half bag not enough)                 |
| Leftovers flagged                                          | Yes   | Tue, Fri                                                             |
| Allergen line                                              | Yes   | Felt noisy to Maya; see below                                        |
| Add to list only after yes, skip duplicates, say how many  | Yes   | "Added 14 ... Eggs were already on"                                  |
| Shared list: never change partner's item; partial match kept | Yes | onions vs red onions; eggs left alone                               |
| Calendar only after yes, all-day, name only                | Yes   |                                                                      |
| Single add: one line with count, no question               | Yes   | dish soap                                                            |
| No shame, no "just", no tip lists                          | Yes   |                                                                      |

## Gaps this run found (for the reviewers)

1. **Shared duplicate with no quantity on the partner's item.** She needed 6 eggs; Jonah's
   item said only "eggs". The skill's "add the difference as its own item" assumes both sides
   have quantities. The run treated it as covered. Suggest one line: "If their item has no
   quantity, count it as enough."
2. **Siri tip timing when the list already exists.** "Mention once, after the list is made"
   never fires for someone whose list was there before the chat. Either drop "is made" or say
   "the first time items go on the list".
3. **Allergen line on every plan.** Strict reading of "say so if a meal could contain a common
   allergen" puts eggs/dairy/gluten on almost every plan. Maya, with no allergies, skimmed it.
   Consider: flag allergens strictly when someone named one; otherwise one short line or none.
4. **Partner notification question.** Came up naturally on a shared list. A one-line answer in
   the skill ("I can't see their notification settings; they'll see it next time they open the
   list") would keep replies consistent and stop a future run from over-promising.
5. **Leftovers counting as a dinner.** Tue's traybake "makes Wed dinner too" and Wed is listed
   as its own dinner. Fine here, but the template counts it as 5 dinners when only 4 are cooked.
   Not wrong; worth a reviewer's view on whether "5 dinners" should say "4 to cook".
