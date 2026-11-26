# Lab round 1: meal-plan-grocery × Maya

- **Persona:** Maya, 34, marketing manager, late-diagnosed, anxious, apologetic writer
  (`lab/personas/maya.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md`
- **Setup for this run:** Claude Pro. Google Calendar connected on claude.ai (account-level, so
  it is also available in the iPhone app). The Claude iPhone app has Reminders allowed. A
  Reminders list called "Groceries" exists and is shared with her partner (fictional name: Sam).
  Sam has already put 4 items on it: milk, bin bags, onion, rice. Memory off. The whole session
  happens in the Claude iPhone app, so Reminders tools are available.
- **Scenario:** Thu 26 Nov 2026, 9:15pm, on the sofa, phone in hand, after a long day. She asks
  for next week's dinners (Mon 30 Nov to Sun 6 Dec), then wants the ingredients on the shared
  list. Same chat, Sat 5 Dec 11am: she is at the supermarket.
- **Calendar next week (what the skill reads):** Mon 5-7pm launch review call; Wed in office all
  day, team drinks 6-8pm; Fri 7:30pm dinner reservation; Tue, Thu, Sat, Sun clear evenings.
- **Skill route taken:** "The weekly plan" (steps 1-6), then "Where the list lives" step 1
  (Apple Reminders, list "Groceries" found), then "The running list" step 2 (at the store).

---

## Transcript

**Turn 1, Maya (Thu 9:15pm):**
> Hi, sorry, this is probably a silly thing to ask an AI but I genuinely never know what to
> make for dinner and we've ordered takeaway like four times this week and I feel kind of bad
> about it. Could you plan dinners for next week? It's just me and my partner, he doesn't eat
> mushrooms, otherwise we eat pretty much anything. Nothing complicated please, I'm usually
> wiped by the time I get home. Sorry for the essay!

**Turn 1, Claude:**
*(Memory off. Maya already answered both step 1 questions: 2 people, no mushrooms. Reads the
calendar for Mon 30 Nov to Sun 6 Dec: Mon and Wed are late, Fri has a dinner booking. Step 3:
asks once about the fridge.)*

> Not silly at all. I can see Monday and Wednesday are late for you, so those get 10-minute
> meals, and Friday you're out. Anything in the fridge that needs using up?

*(33 words. One question. No time on the next step, but the next step is "answer one
question".)*

**Maya, inner:**
> Oh, it looked at my calendar. That's slightly spooky but also... it's right, Wednesday is the
> drinks thing, I'd forgotten. "Not silly at all", okay, that's nice. It didn't make me fill in
> a form. Fridge. Let me go look. Actually I know: spinach that's about to go, feta, eggs.

---

**Turn 2, Maya (9:18pm):**
> Um, there's half a bag of spinach that needs using, some feta that's probably still fine, and
> eggs. Sorry, it's not much! We have the normal stuff, pasta, olive oil, garlic, spices.

**Turn 2, Claude:**
*(Builds the first meals around spinach, feta, eggs. Reuses spinach, feta, chickpeas and
tortillas across meals. Default 5 dinners; Friday is the dinner out, Sunday left for leftovers.
Removes what she already has: pasta, olive oil, garlic, spices, eggs, feta. No allergies given;
flags dairy and eggs per the safety rule.)*

> **This week** (5 dinners, 2 low-energy nights):
> - Mon (busy): Spinach and feta omelette with toast, 10 min. Wilt spinach, pour in eggs,
>   crumble feta, fold.
> - Tue: Chickpea and spinach curry with rice, 25 min. Fry onion and paste, add chickpeas,
>   tomatoes, coconut milk, spinach.
> - Wed (busy): Leftover curry in warm wraps with yogurt, 5 min.
> - Thu: Baked feta pasta with cherry tomatoes, 30 min. Roast feta and tomatoes, stir into
>   pasta with spinach.
> - Sat: Black bean quesadillas with salsa, 20 min. Beans and cheese in tortillas, pan-fry,
>   lime on top.
> - Emergency meal: Pasta with garlic, olive oil, frozen peas and cheese, 12 min.
>
> Contains dairy and eggs. Tell me if that's a problem.
>
> **To buy** (16 items)
> Produce: cherry tomatoes (2 punnets), onions (2), spinach (1 bag), lime (1), frozen peas (1 bag)
> Protein: chickpeas (2 tins), black beans (1 tin)
> Dairy: grated cheese (1 bag), Greek yogurt (1 small pot)
> Pantry: chopped tomatoes (1 tin), coconut milk (1 tin), curry paste (1 jar), rice (1 bag),
> tortillas (1 pack), salsa (1 jar), crusty bread (1 loaf)
>
> Add these 16 to your Groceries list?

*(About 170 words. Frozen peas listed under Produce instead of a Frozen group; bread under
Pantry. Each meal has a time and one line of steps, as the skill asks.)*

**Maya, inner:**
> Okay this is... actually good? Wednesday is just leftovers in a wrap, I can do that drunk.
> Monday omelette, yes. It used my sad spinach. I like that it said "(busy)", it's like someone
> noticed my week is hard without making a thing of it.
> Sixteen things is more than I expected though. I scrolled twice. I'm not going to read the
> whole list properly, I'm just going to say yes and trust it.
> Wait, Sam already put stuff on the list this morning. Will this double everything? Will he
> think I've lost it when 16 things show up on his phone?

---

**Turn 3, Maya (9:21pm):**
> Yes please! Oh wait, sorry, Sam already added some things to that list earlier, will this mess
> it up? I don't want to wipe his stuff

**Turn 3, Claude:**
*(Reads the Reminders list "Groceries": milk, bin bags, onion, rice. Skips onion and rice as
already on. Adds 14. Does not touch Sam's items.)*

> Added 14 to Groceries. Onions and rice were already on, so I left them, and Sam's items are
> untouched (18 on the list).

*(23 words.)*

**Maya, inner:**
> Phew. It didn't delete anything. Good.
> Hmm, Sam put "onion", one onion I think, and the plan needs two. It just skipped it. That's
> fine, I'll probably grab two anyway. Probably.
> Now his phone is going to buzz 14 times, or at least he'll open the list and see a wall of
> stuff and text me "???". I should tell him. Ugh, I hate writing those "don't worry, I'm not
> being weird" messages. And I'll forget what Tuesday is by Tuesday.

*(Note: the skill's duplicate rule is item-name only. Sam's "onion" (no quantity) hid the need
for 2. Minor here, but on a shared list a partner's single item can mask a quantity the plan
needs. The skill says nothing about telling the partner what changed on a shared list.)*

---

**Turn 4, Maya (9:24pm):**
> Thank you so much. Sorry, two more tiny things: could you put the dinners in my calendar so I
> actually remember what we're having? And could you write something short I can send Sam so he
> doesn't panic when he sees the list lol

**Turn 4, Claude:**
*(She asked, so this is the yes the skill requires before putting meals on the calendar. The
skill gives no time for meal events; Claude picks times after the busy blocks: Mon 7:15pm, Wed
8:15pm, Tue/Thu/Sat 6:30pm, 30 min each, title "Dinner: <meal>". The message to Sam is outside
the skill's steps; Claude drafts it in her voice and does not send it.)*

> Done: 5 dinners are on your calendar (Mon after your call, Wed after drinks, the rest at
> 6:30pm).
>
> For Sam:
> "Planned next week's dinners! That's why 14 things just showed up on the Groceries list. Your
> stuff's still there. Monday is omelettes, I'll send the rest."

*(50 words. Draft is not sent; she copies it.)*

**Maya, inner:**
> Oh, Mon "after your call" and Wed "after drinks". It got it. I'd have put Monday at 6:30 and
> then felt bad about it.
> The message sounds like me. Kind of. I'd say "babe" but I can add that. I'll copy it.
> I didn't have to explain three times. That's the first time this week something was actually
> easy.

---

**Turn 5, Maya (Sat 5 Dec, 11:02am, supermarket entrance, same chat):**
> ok I'm at the shop, what do I need

**Turn 5, Claude:**
*(Reads Groceries. Sam ticked off milk on Thursday and added "coffee" on Friday. 18 items now:
14 from the plan, onion, rice, bin bags, coffee. Groups into 5 groups, nothing above it. No
staples saved, so no staples line.)*

> **Produce:** cherry tomatoes (2), onion, spinach, lime
> **Fridge:** grated cheese, Greek yogurt
> **Pantry:** chickpeas (2 tins), black beans, chopped tomatoes, coconut milk, curry paste, rice,
> tortillas, salsa, coffee, crusty bread
> **Frozen:** frozen peas
> **Other:** bin bags

*(One onion shows, not two: the plan's "onions (2)" was skipped as a duplicate in turn 3.
Nothing above the list, as the skill says. No staples line, since none are saved.)*

**Maya, inner:**
> Yes. This is all I need. It's in the order of the shop, roughly. Coffee's on, Sam must have
> added it. Good.
> One onion. Didn't it say two? Whatever, I'll get two.
> I'm actually going to cook this week. Maybe. Monday at least.

*(Session ends. She shops from the list.)*

---

## Lab notes (simulator, not scores)

What worked for Maya:
- **Turn 1 asked one thing.** She had already given people and dislikes, so the skill skipped
  step 1's questions and asked only the fridge question. No form, no list of tips.
- **Calendar reading felt like care, not surveillance**, because it was named in plain words
  ("Monday and Wednesday are late for you"). "(busy)" labels and the 5-minute leftovers night
  on drinks night landed well with an exhausted, masking persona.
- **Shared-list safety.** Turn 3 answered her real fear (wiping Sam's items) in one line, with a
  count. No question asked before adding, as the skill says.
- **Calendar placement** after busy blocks (turn 4) was the moment she felt understood.
- **Store view (turn 5)** was clean, included the partner's items, and had no guessed staples
  line.

Where it was weaker:
1. **The plan reply is long** (about 170 words, 16 items). She scrolled twice and said yes
   without reading. The skill's template has no length cap. Suggest: cap "To buy" or show only
   the count plus the first group, with the full list going straight to Reminders on yes.
2. **Duplicate rule ignores quantity on a shared list.** Sam's "onion" masked the plan's 2. The
   store view showed 1. Suggest: when an item is already on, bump the quantity if the plan needs
   more ("onion was on; made it 2").
3. **No partner heads-up.** On a shared list, 14 new items appear on someone else's phone. Maya
   had to ask for a message to Sam. The skill's "Shared with a partner" line covers setup only.
   Suggest: after adding to a shared list, offer one line: "Want a short note for whoever shares
   the list?" (draft only, never sent).
4. **Meals on calendar: no default time.** Claude chose times after busy blocks, which worked,
   but the skill gives no rule. Another run could put Monday's dinner during her call.
5. **Grouping drift between sections.** The weekly plan groups (produce, protein, dairy, pantry,
   frozen) differ from the store groups (Produce, Fridge, Pantry, Frozen, Other), and in turn 2
   peas went under Produce. Minor, but two group sets for one list is extra load.
6. **First reply has no time on the next step.** The lab bar asks for one next step with a time.
   Here the step is "answer a question", so a time feels forced, but reviewers may flag it.
7. **Out-of-skill request (draft for Sam)** was handled sensibly but the skill doesn't cover it.
   Fine to leave out of scope; noted for reviewers.
