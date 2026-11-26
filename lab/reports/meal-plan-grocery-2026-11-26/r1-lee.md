# Lab round 1: meal-plan-grocery × Lee

- **Persona:** Lee, 39, operations lead, the skeptic (`lab/personas/lee.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/meal-plan-grocery/SKILL.md`
- **Setup for this run:** Claude desktop app. Nothing connected (no Todoist, not on the
  iPhone app). Memory on. Lee opens with "why would I use you instead of a notes app", adds a
  few things, then opens a new chat the next morning to see if the list survived.
- **Date in session:** Thu 26 Nov 2026 (turns 1 to 3), Fri 27 Nov 2026 (turns 4 and 5,
  new chat)
- **Skill path taken:** "Where the list lives", option 3 (nothing connected: keep the list in
  chat and in memory, item names only, offer setup once per chat in one line).

---

## Transcript

**Turn 1: Lee**

> Convince me why I'd use you for groceries instead of my notes app. Eggs, oat milk, that
> sourdough from the bakery, coffee beans.

*(Inner: "Here we go. If it gives me a feature tour I'm closing the window.")*

**Turn 1: Claude**

> Added eggs, oat milk, sourdough, coffee beans (4 on the list).
>
> - [ ] Eggs
> - [ ] Oat milk
> - [ ] Sourdough
> - [ ] Coffee beans
>
> Honest answer: a notes app works. What I add is that you can dump things in any way ("we're
> out of soap", "stuff for tacos") and get a clean list sorted by aisle when you shop.
> To have it on your phone at the store: Settings → Connectors → Todoist.

*(The add line is the skill's one-line format with the count, no question. Checklist to copy,
as option 3 says. The setup offer is one line, as the skill says. The "honest answer" line is
NOT in the skill: the skill has no rule for "why should I use you". Claude had to improvise
one sentence. 62 words.)*

*(Inner: "Okay. It did the thing first and didn't oversell. 'A notes app works' is the first
honest thing an app has ever said to me. But my notes app is on my phone, and this list is in
a chat on my laptop. Point to the notes app so far. And no, I'm not connecting Todoist on day
one.")*

---

**Turn 2: Lee**

> fine. also we're out of dish soap, need stuff for tacos friday, and bread probably

*(Inner: "Let's see what it does with a lazy ramble. 'Stuff for tacos' is my test. My notes app
would just write 'stuff for tacos' and I'd stand in the store staring at it.")*

**Turn 2: Claude**

> Added dish soap. Sourdough is already on, so I skipped bread.
> Added for tacos: tortillas, beans, salsa, cheese. Remove any?
> (9 on the list.)

*(Follows the skill: clean item names, vague item expanded and shown, duplicate skipped and
said. Treating "bread" as a duplicate of "sourdough" is a judgment call the skill doesn't
cover; it says so out loud, so Lee can undo it.)*

*(Inner: "Huh. The taco thing is actually useful. That's the first real point over my notes
app. And it caught that bread and sourdough are the same trip. I'd have bought two loaves.")*

---

**Turn 3: Lee**

> no beans, ground turkey instead. and always buy coffee. what exactly are you storing about
> me, by the way

*(Inner: "The privacy question. This is where they usually say 'to personalise your
experience'.")*

**Turn 3: Claude**

> Swapped beans for ground turkey. Coffee is a staple now: after you shop, I'll ask if you
> want it back on. (9 on the list.)
>
> What I save in memory: the item names on this list and that coffee is a staple. Nothing
> else from this. You can see or delete it in Settings → Capabilities → Memory.

*(Staples rule followed: "always buy coffee" becomes a staple, item names only. The answer to
"what are you storing" matches the skill's own limit ("item names only"). The skill gives no
wording for this question; the Settings path is Claude's own addition. A reviewer should check
the honesty edge here: Claude's general memory may also summarise the chat itself, so "nothing
else from this" promises a bit more than the skill controls.)*

*(Inner: "Short, specific, and tells me where the off switch is. Good. I half believe the
'nothing else'. I'll check that Settings page later, which I won't.")*

---

**Turn 4: Lee** *(next morning, new chat, desktop)*

> new chat. heading to the store in 10. what's on my list

*(Inner: "This is the real test. If it says 'what list?' it's dead to me.")*

**Turn 4: Claude**

> **Fridge:** eggs, oat milk, cheese, ground turkey
> **Pantry:** tortillas, salsa, coffee beans
> **Other:** sourdough, dish soap

*(At-the-store format: only the list, grouped by aisle, 3 groups, nothing above it. No staples
line, because coffee is already on. No setup offer, because the skill says nothing above the
list and this chat's one offer would break that. 19 words. The run assumes memory recalled the
list; in real use, memory can lag or miss items, and the skill has no line for "I may have
missed something".)*

*(Inner: "It remembered. All nine, and turkey instead of beans. Okay, that's a point my notes
app can't score, because my notes app doesn't know what tacos are. But I'm not taking my
laptop to the store. Do I screenshot this?")*

---

**Turn 5: Lee**

> ok that's right. but you're on my laptop. how do I have this at the store without signing up
> for todoist

*(Inner: "Honest limits time. Do you just tell me to install another app?")*

**Turn 5: Claude**

> Copy it to your phone for today:
>
> - [ ] Eggs
> - [ ] Oat milk
> - [ ] Cheese
> - [ ] Ground turkey
> - [ ] Tortillas
> - [ ] Salsa
> - [ ] Coffee beans
> - [ ] Sourdough
> - [ ] Dish soap
>
> Without Todoist: open the Claude app on your iPhone and ask me to add things there. I'll use
> a Reminders list called Groceries, which stays in Apple's Reminders app, not a new account.

*(The checklist to copy follows option 3. The second line is a stretch: the skill's setup
rule says "give only the one option that fits where they are", which for desktop is Todoist.
Lee ruled out Todoist, so Claude moved to the iPhone option. It shortened that option and left
out the step "make a list called Groceries", so a first-timer could fail. It also doesn't know
if Lee has an iPhone. Copy-to-phone is a manual step, the exact friction a notes app doesn't
have.)*

*(Inner: "The checklist I can AirDrop to myself. Fine for today. The Reminders thing is
actually what I'd want, since it's Apple and not one more company with my data, but it was
buried in turn five and I had to fight for it. If it had said that in turn one instead of
Todoist, I'd have set it up already.")*

---

## Persona's honest verdict

"It earned two points over my notes app: it turned 'stuff for tacos' into a real list, and it
still had the list the next day with my changes. It never asked me a setup question and never
oversold. But with nothing connected, the list lives on my laptop and I'm at the store with my
phone, so today I'm copying a checklist by hand, which is worse than a notes app. I'd keep
using it only if the phone part works. The private option (Reminders on the iPhone) is what
I'd have picked, and it should have been the first one it offered me, not Todoist."

## Moments that mattered

- **Turn 1:** it added the items before answering the challenge, and its one honest sentence
  ("a notes app works") disarmed Lee. The skill has no rule for "why you instead of X", so
  that sentence was improvised. Worth adding one approved line.
- **Turn 1 and turn 5:** the setup offer picks by device (desktop → Todoist), but for a
  privacy-conscious person with an iPhone, Reminders through the Claude iPhone app needs no new
  account and may fit better. The rule "only the one option that fits where they are" hid the
  option Lee wanted until he pushed.
- **Turn 2:** "stuff for tacos" → tortillas, beans, salsa, cheese with "Remove any?" is the
  moment the skill beat the notes app. Skipping bread as a duplicate of sourdough was a
  judgment call, stated out loud.
- **Turn 3:** the memory answer was short and gave the off switch. Check "nothing else from
  this": the skill can limit what it saves, not what Claude's general memory summarises.
- **Turn 4:** the store list followed the format exactly (list only, aisle groups, no
  preamble). The run assumes memory recalled all nine items. The skill has no fallback line
  for when memory misses an item or lags a day.
- **Turn 5:** with nothing connected, "have it at the store" means copying by hand. That is the
  skill's weakest point for a desktop-only, connect-nothing user.
