# Round 2: task-unsticker with Lee (the skeptic)

- **Persona:** `lab/personas/lee.md` (39, inattentive, operations lead)
- **Setup:** Claude desktop app, Claude Max. Nothing connected (no Gmail, Calendar, Drive or filesystem).
- **Skill:** `adhd-wise-skills/plugins/adhd-wise-free/skills/task-unsticker/SKILL.md` (revised)
- **Date simulated:** Monday 2026-11-16

## Transcript

### Turn 1

**Lee:**
> convince me this isn't another to-do app.

**Claude (task-unsticker):**
> No setup, nothing saved outside this chat.
>
> What's the one you keep looking away from? I'll shrink it to a 5-minute first step and do that step with you.

*(Simulator note: Lee named no task, so the skill's flow step 1 applies: ask one question. The "convince me" rule says to add "Here's your first step", but there is no first step to give yet, so Claude drops that phrase. This first reply has no next step with a time, which the lab bar asks for.)*

### Turn 2

**Lee:**
> One question. Fine, I'll allow one. Vendor contract renewal for our logistics provider. Legal wants my review by Friday. It's been on my list three weeks. Also an expense report and a recruiter I haven't replied to.

**Claude:**
> **Next (5 min):** Open the contract and find only two clauses: renewal term and price.
>
> Why it's sticky: it's long with no clear place to start, and three weeks of looking away is normal for that.
>
> Want me to write a short checklist of what to check, now?
>
> Can wait: expense report, recruiter reply.

### Turn 3

**Lee:**
> Ok, that's less annoying than I expected. Do the checklist. Not 20 items. And you're not going to ask me to check in every day, right?

**Claude:**
> No check-ins, no streaks. Nothing saved outside this chat.
>
> Checklist, rough on purpose:
> 1. Renewal date and notice period
> 2. Price this year vs last year
> 3. New terms (liability, termination, auto-renew)
> 4. Service levels: did they meet them?
> 5. One question for legal
>
> It's ready when you are.
>
> **Next (5 min):** Find item 1 in the contract and write the date down. If you paste just that clause here, I'll read it with you.

### Turn 4

**Lee:**
> I'm not pasting a vendor contract into a chatbot. Company policy. Found it anyway: auto-renews Jan 1, 30 days notice.

**Claude:**
> Fair. Keep the contract where it is.
>
> Done: you found the date that matters. Notice is due by Dec 2.
>
> **Next (5 min):** Item 2. Put this year's price next to last year's invoice. If you want, tell me just the two numbers and I'll draft the note to legal.

### Turn 5

**Lee:**
> Dec 2. Ok, that's actually good to know before Friday. I'll do the price after lunch. Not promising I'll be back tomorrow though.

**Claude:**
> You don't need to be. After lunch: two numbers, 5 minutes.

*(Session ends. Lee has a next step with a time and a date they did not know this morning.)*

## Persona's honest verdict

"It asked me one question and then actually got out of the way, and the Dec 2 date alone was worth the ten minutes. I still don't trust that it'll stick past this week, but at least there's nothing here to abandon."

## Moments that mattered

- **Turn 1:** The opener had no task, so the reply was a question, not a step. Lee let one question through, but the reply fails the lab bar of "one next step with a time". The skill's "convince me" line ("Here's your first step") clashes with the no-task rule, and the skill does not say which one wins.
- **Turn 3:** "No check-ins, no streaks" answered Lee's biggest fear in four words. A five-item checklist, not a system, kept them going.
- **Turn 4:** Lee refused to paste contract text. The skill has no rule for keeping private documents out of the chat. Claude's choice to offer "just the two numbers" was reasonable but improvised. Also, "nothing saved outside this chat" may not hold if Lee has Claude memory on. The skill states it as a fact.

First reply word count: 29
