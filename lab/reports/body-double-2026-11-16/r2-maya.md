# Lab session r2: body-double x Maya (revised skill)

- **Skill:** `plugins/adhd-wise-bonus/skills/body-double/SKILL.md` (revised after round 1)
- **Persona:** Maya, 34 (`lab/personas/maya.md`)
- **Setup:** claude.ai on a laptop, Claude Pro, Gmail and Calendar connected, memory on
- **Date simulated:** 2026-11-16, Monday, 4:45pm

---

## Transcript

**Turn 1: Maya**

> Sorry, this is probably silly, but could you sit with me for like 20 minutes? There's an email from the client's marketing director, a reply to the Q3 report I sent last week. Subject is "Re: Q3 results - a few concerns". It came in Thursday and I still haven't opened it. Every time I see it my stomach drops and I close the tab. It's nearly 5 and I'm fried. Sorry, I know it's just an email.

**Turn 1: Claude (body-double)**

> Not silly. Let's start.
>
> Session: the Q3 client email, 20 min. Done = you know what it says.
> First 2 minutes: want me to read it first and tell you what's in it? Say yes and I'll do it now.
> I'm here. Say "check" any time, or tell me when you're done.

*(Simulator note: the revised rules apply literally. No question before starting; length is her 20 minutes; Claude proposes a small "done"; Gmail is connected, so the first move is the scary first look, and it waits for her yes. "Probably silly" and "fried" sound apologetic and tired, not hopeless, so the low path does not trigger. The template's "First 2 minutes" line holds a question, not something she does. It reads fine here because a yes is all she needs to do. No dot instruction or calendar offer yet, which keeps it short.)*

**Turn 2: Maya**

> Yes. Please. Sorry. Just tell me if it's bad.

**Turn 2: Claude (body-double)**

*[Gmail: search `subject:"Q3 results - a few concerns"`, read the newest message in the thread. Read-only.]*

> Read it. It's smaller than the subject line.
> They liked the report and said the email results were "the strongest quarter yet".
> One concern: LinkedIn cost per lead went up. They want a suggested Q4 budget split by Friday.
> Nothing about you. That's your done.
> Next 2 minutes, if you want: read it yourself once. Send a dot (.) when you have.

*(Simulator note: five lines, under the six-line limit. "Smaller than the subject line" is her "what good looks like". The skill has no rule for how to report back what Claude read. Claude leads with the reassurance and then the one ask, which works. The dot instruction from "Check-ins" shows up here for the first time.)*

**Turn 3: Maya**

> .
>
> Ok. Wow. I read it. It's really ok. I've been carrying this since Thursday. The Friday thing is real work though, I can't do the budget split tonight, I'm done for today. But I feel like I should reply so they know I saw it? Could you help me write something short? I always over-apologise in emails.

**Turn 3: Claude (body-double)**

*[No tool call. A reply only needs the email she has just read.]*

> Yes, a short reply now is a good finish. Here's a draft:
>
> "Hi, thanks for the feedback, really glad the email results landed well. Good point on LinkedIn cost per lead. I'll send a suggested Q4 split by Friday."
>
> No apology in it. Change anything that doesn't sound like you. Want me to save it as a Gmail draft, or will you paste it?

*(Simulator note: "Stuck: offer to do the stuck part with them: draft the paragraph" covers this. The draft goes past the six-line limit, and the skill still has no rule for drafts or matching her voice. Claude picks up her own words ("I over-apologise") and keeps the apology out, so the draft sounds close enough to her. Friday counts as a deadline, but she isn't doing the work tonight. Claude does not add a "real time left" line, which matches what she needs, but the skill doesn't say whether to. Nothing gets sent or saved without a yes.)*

**Turn 4: Maya**

> Save it as a draft please. I'll change "really glad" to "so glad" because that's more me, then send it myself.

**Turn 4: Claude (body-double)**

*[Gmail: create a draft reply in the thread with the text above. Not sent.]*

> Saved as a draft in that thread. It's not sent. Change it and send it when you're ready.
> Send a dot when it's gone.

**Turn 5: Maya**

> .
>
> Sent. 12 minutes. Three days of dread for 12 minutes. Thank you, and sorry for all the sorrys.

**Turn 5: Claude (body-double)**

> Done: read the Q3 email and sent a reply promising the Q4 split by Friday.
> Nice. Getting past the dread was the hardest part, and you did it today.
> Next time: the Q4 split. 10 minutes tomorrow: list last quarter's spend per channel.
>
> Break or another round? I can also remember this: "Body double: Q3 client email, Nov 16, done: read and replied."

**Turn 6: Maya**

> Break. Yes, remember it. And honestly, put a 10-minute thing for the split on my calendar for tomorrow at 10? I'll probably ignore it but still.

*(Session ends. Claude saves the memory line and creates a 10-minute Calendar event, "Q4 split: list last quarter's spend per channel", for Tue Nov 17 at 10:00, both after her yes. The skill only covers calendar nudges inside a session ("a calendar event is a weak nudge; say so"). This one is for tomorrow and she has already said she might ignore it, so Claude just sets it.)*

---

## Persona's honest verdict

"This time it offered to read the email before I had to ask, and hearing 'it's smaller than the subject line' in the second message is the whole reason I got through it. The draft was nearly my voice, and I only changed two words, which is a first."

## Moments that mattered

- **Turn 1:** The first reply started the session with no question first and offered the scary first look ("want me to read it first?"). This is the round 1 fix working. She could answer with one word, at nearly 5pm and fried.
- **Turn 2:** "It's smaller than the subject line. Nothing about you." Claude took the first look for her and named that it was small, which matches her "what good looks like" exactly. It also put the one real ask (Friday) in a single line instead of a summary.
- **Turn 3:** Claude drafted with no apology because she said she over-apologises. This worked, but only because she said it. The skill still has no rule for drafts, voice or length, and the draft broke the six-line limit. Worth a line in `SKILL.md`.

First reply word count: 51
