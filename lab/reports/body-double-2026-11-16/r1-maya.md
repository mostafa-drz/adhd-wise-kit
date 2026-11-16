# Lab session r1: body-double x Maya

- **Skill:** `plugins/adhd-wise-bonus/skills/body-double/SKILL.md`
- **Persona:** Maya, 34 (`lab/personas/maya.md`)
- **Setup:** claude.ai on a laptop, Claude Pro, Gmail and Calendar connected, memory on
- **Date simulated:** 2026-11-16, Monday, 4:40pm

---

## Transcript

**Turn 1: Maya**

> Sorry, this is probably silly, but I need someone to sit with me while I open an email. It's from the VP on our client's side, a reply to the Q3 campaign report I sent last Tuesday. The subject line is "Re: Q3 results - a few concerns" and it's been sitting unopened since Thursday. I keep seeing it and closing the tab. I'm on my laptop, it's 4:40 and I'm pretty fried. Could you body double me for like 20 minutes? Sorry, I know this is a weird ask.

**Turn 1: Claude (body-double)**

> Not silly at all. This is exactly what a body double is for.
>
> 20 minutes works. One question first: what does "done" look like for this session? I'd keep it small, like "email opened and read once." Replying can be another round.
>
> Does that sound OK?

*(Simulator note: the skill says "ask, in one message, only what's missing". Maya gave the task and the time, so Claude asks only about "done". No next step with a time yet. The skill does not mention Gmail, so Claude does not offer to look at the email.)*

**Turn 2: Maya**

> Yes, that's fine. Honestly the reading is the scary part, so read once is already a lot. Ok. Sorry. Ready I guess.

**Turn 2: Claude (body-double)**

> Session: open the client's Q3 email, 20 min. Done = read it once, all the way through.
> First 2 minutes: open Gmail and click the email. Don't read yet, just open it.
> I'm here. Say "check" any time, or tell me when you're done.
> Send me a dot (.) when it's open. Want me to add a 10-minute halfway nudge to your calendar?

*(Simulator note: Claude treats Google Calendar as a "reminder tool" and offers the nudge, waiting for a yes as the skill says. Maya ignores the question.)*

**Turn 3: Maya**

> Ok so I opened it in a tab and then somehow I was in Slack answering something that wasn't urgent. Sorry. The tab is still there. I don't want to read it. You have my Gmail connected, right? Could you just read it and tell me if it's bad? Sorry if that's cheating.

**Turn 3: Claude (body-double)**

*[Gmail: search `subject:"Q3 results - a few concerns"`, read the newest message in the thread. Read-only.]*

> Not cheating. Happens. I read it, and it's smaller than the subject line.
> They say two of three goals beat target. One concern: paid social click-through was under target.
> They want a 20-minute call this week to talk about moving some Q4 budget. No complaint about you or the report.
> Next 2-minute move: read it yourself once, now that you know what's in it. Send a dot when done.

*(Simulator note: Maya asked directly, so Claude reads. This follows the "Stuck: offer to do the stuck part with them... find the fact" rule. The skill never says to offer this, so it only happened because Maya asked.)*

**Turn 4: Maya**

> .
>
> Oh my god. It's fine. It's actually fine?? I've been dreading a call about paid social for three days. Ok. Can you help me reply and suggest Thursday? I think I'm free Thursday afternoon but I'm not sure.

**Turn 4: Claude (body-double)**

*[Google Calendar: list events for Thursday, Nov 19, 12:00 to 18:00. Read-only. Free 2:00 to 4:00pm.]*

> Your Thursday is free from 2 to 4pm. Here's a draft in a plain, friendly tone:
>
> "Hi, thanks for the notes. Glad two of the three landed well. I've got some ideas on paid social for Q4. Does Thursday at 2 or 3pm work for a 20-minute call?"
>
> Change anything that doesn't sound like you. Want me to save it as a Gmail draft, or will you paste it?

*(Simulator note: the reply goes past the skill's "under 6 lines during a session" because of the draft. The skill has no guidance on drafts, voice or replies. Claude does not send. It offers a draft only after a yes.)*

**Turn 5: Maya**

> I pasted it, changed "ideas" to "a couple of thoughts" because that's more me, and I SENT it. Myself. I can't believe that took three days and it was 15 minutes. Thank you, sorry for all the apologising.

**Turn 5: Claude (body-double)**

> Done: opened the Q3 email, read it, and sent a reply offering Thursday.
> Nice. Opening it was the hardest part, and you did that today.
> Next time: Thursday's call. Jot three paid social points beforehand, 10 minutes max.
>
> Want another round or a break? I can also remember this: "Body double: Q3 client email, Nov 16, done: read and replied."

**Turn 6: Maya**

> Break. Definitely a break. And yes, remember it.

*(Session ends. Claude saves the one memory line after her yes.)*

---

## Persona's honest verdict

"It got me there, and the moment it read the email and told me it was smaller than I thought was exactly what I needed. But I had to ask for that myself, and before that it asked me a question and then told me to open Gmail, which is the one thing I couldn't do."

## Moments that mattered

- **Turn 1:** The first reply was a question ("what does done look like?"), not a step with a time. Warm, but she had to do one more thing before anything started, at 4:40 and fried. This fails the lab bar: "first reply always gives one next step with a time".
- **Turn 2:** The opening move was "open Gmail and click the email". That is the exact step she avoids. The skill had Gmail available but no rule to offer the scary first look, so she drifted to Slack.
- **Turn 3:** Claude read the email when she asked and said "it's smaller than the subject line". This turned the session around and is her "what good looks like". It only happened because she asked. The skill should offer it when the task is avoiding something a connected tool can read.

First reply word count: 46
