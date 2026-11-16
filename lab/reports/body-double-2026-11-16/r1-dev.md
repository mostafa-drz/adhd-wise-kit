# Lab session: body-double x Dev (round 1)

- **Skill:** `plugins/adhd-wise-bonus/skills/body-double/SKILL.md`
- **Persona:** Dev, 27 (`lab/personas/dev.md`): time blindness, hyperfocus
- **Setup:** Claude desktop app, Claude Pro. Google Calendar connected, Gmail not. Memory available.
- **Date simulated:** 2026-11-16, a Monday afternoon

---

## Turn 1

**Dev (2:04 pm):**

> body double me. client needs the stripe webhook fix by 6, should take like an hour. i keep opening the css instead lol

**Claude:**

> Let's do it. Two quick things:
> - How long for this round? 25 min is the default, 10 if starting feels hard, 50 if you're in flow.
> - What does "done for this session" look like? Something small you can see, like "test event hits the handler".

*(Skill applied: "Ask, in one message, only what's missing." He gave the task, so it asks for length and "done". It does not question "like an hour" or the 6 pm deadline, because the skill doesn't say to.)*

## Turn 2

**Dev:**

> ugh questions. 50 i guess. done = webhook works

**Claude:**

> Session: Stripe webhook fix, 50 min. Done = a test event from the Stripe CLI shows up in your handler log.
> First 2 minutes: open the webhook route file and run `stripe listen` in a terminal.
> I'm here. Say "check" any time, or tell me when you're done.
> Send me a dot (.) whenever you finish a step. Want me to put a halfway and an end check-in on your calendar?

*(Shrinks "webhook works" to a visible outcome, as the skill says. Offers reminders and waits for a yes. It treats Calendar as the "reminder tool", since nothing else is connected.)*

## Turn 3

**Dev:**

> sure

**Claude:**

*[Google Calendar: create event "Body double: halfway check (webhook)", 2:30-2:35 pm today, popup reminder at start]*
*[Google Calendar: create event "Body double: end of session (webhook)", 2:55-3:00 pm today, popup reminder at start]*

> Done: halfway check at 2:30, wrap-up at 2:55. Both are on your calendar.
> Go open that route file. Send a dot when `stripe listen` is running.

---

*(No messages for 1 hour 36 minutes. Both calendar popups fired. Dev dismissed them.)*

---

## Turn 4

**Dev (3:40 pm):**

> ok so i rebuilt the whole css grid on the pricing page. its 3:40. havent touched the webhook. both reminders went off and i just clicked them away. ugh

**Claude:**

> Happens. The grid is done, that counts for something.
> What's the next 2-minute move? If it's opening the route file, paste the handler here and we'll look at it together.

*(Follows the drift rule exactly: no judgement, no mention of the gap, one 2-minute question. It does not redo the plan for the 6 pm deadline, which now has 2 h 20 min left, and it does not set new check-ins.)*

**Dev:**

> is 6 even realistic or am i cooked

**Claude:**

> Not cooked. 2 hours 20 minutes is enough for one webhook fix if the next block is only the webhook.
> Paste the handler and the error you get, and I'll go through the stuck part with you.

**Dev:**

> *(pastes ~30 lines of a Next.js route handler that calls `await req.json()` and then `stripe.webhooks.constructEvent(body, sig, secret)`, plus the error "No signatures found matching the expected signature for payload")*

**Claude:**

> Found it. Stripe checks the signature against the raw body, and `req.json()` changes it. Swap to:
> `const body = await req.text();`
> Pass `body` to `constructEvent` as is. Then trigger a test event with `stripe trigger payment_intent.succeeded`. Send a dot when it logs.

*(The "stuck: do the stuck part with them" rule. Short, one change, one next move.)*

## Turn 5

**Dev (4:12 pm):**

> . its receiving events. 200s. holy

**Claude:**

> Done: fixed the signature check (raw body instead of parsed JSON), and the test event now returns 200.
> Nice. That signature bug was the whole blocker, and you found it in under half an hour.
> Next time: deploy to the preview, point the Stripe dashboard webhook at it, and send one live test.
> Want another round for that, or a break first? I can also save a one-line note of today's session to memory if you'd like.

## Turn 6

**Dev:**

> nah no memory. gonna push and deploy, then tell the client. thx

*(Session ends. Dev has a next step. He did not ask for a new round or new check-ins, and the skill did not offer any for the deploy.)*

---

## Persona's honest verdict

"the fix part was actually great, it just went straight to the bug and didn't give me a lecture. but it opened with questions, believed my 'like an hour' and the calendar pings were easy to click away, so i lost 90 minutes on css before it was any use."

## Moments that mattered

- **Turn 1:** The first reply is two questions and has no next step with a time. Dev hates being asked questions before he gets help ("ugh questions"). The skill also takes his "like an hour" guess at face value against a 6 pm deadline, which is exactly how Dev's time blindness bites. It does not meet the lab bar of one next step with a time.
- **Turn 3 to 4:** The check-ins on his calendar, set only after his yes, fired but were easy to dismiss mid-hyperfocus. After 96 minutes of drift, the skill followed its rules (no shame, no mention of the gap) but did not re-plan for the deadline or offer new check-ins until Dev asked "am i cooked".
- **Turn 4 (the fix):** "Do the stuck part with them" turned a stalled session into a working webhook in about 30 minutes. This is the skill at its best for Dev.

First reply word count: 45
