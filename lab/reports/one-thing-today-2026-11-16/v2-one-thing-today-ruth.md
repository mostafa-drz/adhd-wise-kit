# Lab simulation (v2): one-thing-today-adhd × Ruth

- **Skill:** `plugins/adhd-wise-bonus/skills/one-thing-today-adhd/SKILL.md` (revised version)
- **Persona:** `lab/personas/ruth.md` (46, inattentive, phone only, claude.ai Pro, nothing connected)
- **Setting:** Monday 16 November 2026, about 9:05pm. Ruth is at the kitchen table, drawer
  open, phone in hand.
- **Setup in play:** No calendar, email, documents or memory connected. Ruth names her tasks
  in the first message, so the skill takes flow step 2, first bullet: "pick from what they said
  and give the full reply now."

---

### Turn 1

**Ruth:**
> where do i start. drawer is full. sons school trip form due fri ($15), car insurance renewl letter says renew by 20th, plumber overcharged me want refund think i have til end of month?, dentist wants me to rebook. late fees are killing me this year

**Claude (skill):**
> **Your one thing:** Renew the car insurance.
>
> **Why this one:** The letter says the 20th, which is Friday. If it lapses you can't drive
> legally and you may pay more to restart it.
>
> **Start (5 min):** Take the renewal letter out of the drawer and circle the price and the
> phone number. When you put the kettle on, do this first.
>
> **Good enough:** Tonight you know the price and the number. The call can be tomorrow.
>
> **Can wait:** School form (do it Thursday), plumber refund, dentist.
>
> Want me to write the exact words for the phone call now?

*(Ruth's aside: "Okay. That's an actual answer. Long, but I can see the bold bits.")*

---

### Turn 2

**Ruth:**
> found it. $1,140 up from $960 last yr?? number is on the back. yes words pls, i hate calling them i always freeze

**Claude (skill):**
> Here's what to say. Keep the letter in front of you.
>
> **When they answer:**
> "Hi, I'm calling about my car insurance renewal. My policy number is [number on the
> letter]. The renewal price went from $960 to $1,140. Can you tell me why it went up, and
> is there any discount you can apply?"
>
> **If they say no discount:**
> "Okay. Can you check if a higher deductible would bring the price down? I just want to see
> my options before I renew."
>
> **To finish:**
> "Thanks. Please go ahead and renew it before the 20th, and email me the confirmation."
>
> If you freeze, it's fine to say: "Sorry, give me a second, I'm reading my notes."
>
> **Good enough:** It's renewed before Friday. A lower price is a bonus, not the goal.

*(Ruth's aside: "The 'give me a second' line. That's the bit I needed.")*

---

### Turn 3

**Ruth:**
> ok. they open 8am. i will forget tho. also the school form is literally 2 mins should i just do it now

**Claude (skill):**
> Yes, do the form now. It's two minutes and it's done.
>
> For tomorrow: when you pour your first coffee, open this chat and call. The words are right
> here.
>
> Put the letter on top of your phone or your keys tonight so you see it first thing.
>
> **Can wait:** plumber refund, dentist.

---

### Turn 4

**Ruth:**
> form done its in his bag with $15. letter is on my keys. thank you this is the first time the drawer didnt win

**Claude (skill):**
> That's two things done tonight. The drawer can wait until after the call tomorrow. Good
> night.

*(Session ends. Ruth has a next step with a time: 8am call with the script ready.)*

---

## Persona's honest verdict

"It told me what to do straight away and gave me the actual words for the insurance call,
which is the part I always freeze on, and the form got done too. The first answer was a bit
long for my phone and it never asked if I wanted to try for a cheaper price before telling me
to just renew, but I'd use this again tomorrow."

## Moments that mattered

- **Turn 1:** Because Ruth named her tasks, the revised skill gave a full answer instead of a
  question (the v1 failure). It picked the insurance over the school form using the
  "earlier consequence" tie-break, both due Friday. But the full format runs about 90 words,
  over the lab's 60-word first-reply bar; the skill only caps the nothing-named case at 60.
- **Turn 2:** The phone script, including the "give me a second" line for freezing, matched
  exactly what "good" looks like for Ruth. This came from flow step 5 ("write the exact words
  for a phone call").
- **Turn 3:** Ruth's memory worry got an if-then cue ("when you pour your first coffee") and
  a physical reminder (letter on the keys), per flow step 6. The skill let her do a second
  quick task without fuss, though it has no explicit rule for "can I also do X now".
