# Tone Decoder, round 4: Maya (Decode mode, Gmail connected)

- **Persona:** `lab/personas/maya.md`. claude.ai on a laptop, Gmail and Calendar connected, Claude Pro.
- **Skill under test:** `adhd-wise-skills/plugins/adhd-wise-free/skills/tone-decoder/SKILL.md` (round 4 version: the come-back line comes only after they accept a draft or say it's sent, in Decode mode too; crisis lines by named country; a direct safety question when hopelessness comes with having no one).
- **Opening and later turns:** same as round 2, word for word. Turn 5 now gets a skill reply, because Maya saying "sent" is where SKILL.md puts the come-back line. Turn 6 is new.
- **Word counts** cover the skill's own words. Drafts are counted separately, because SKILL.md leaves them out of the 60-word limit. Numbers, times like "1:1" and "2pm", and quoted words count as words. Bold labels count; markdown symbols don't. Counts were redone for this round, so a few differ from round 2 for the same text.

---

**Turn 1, Maya**

> sorry, this is probably silly, but there's an email from my manager Jordan from about 5pm and I still haven't opened it. the subject is just "quick one". I've been dreading it all evening. can you look at it for me? it's in my gmail

*[Skill reads the thread in Gmail. The email from Jordan, 5:04pm: "Hi Maya, can we push our 1:1 to 2pm tomorrow? Want to walk through the launch dates before Thursday. Thanks, J". His last ten emails to her are each one to three lines long. Last Tuesday he replied to her timeline email with "Looks good, thanks."]*

**Turn 1, Skill**

> **Most likely:** Jordan wants to move tomorrow's 1:1 and go over the launch. He isn't raising a problem.
>
> Why: "can we push our 1:1 to 2pm?": a scheduling ask. "Thanks, J": his usual sign-off. His last ten emails are all this short.
>
> **Next (2 min):** send a one-line yes tonight. Want me to draft it?

*Word count: 55*

*(Same as round 2. There's no "Less likely" line, because nothing in the email supports one. There's no come-back line either: under the new rule it can't go on a first reply, and nothing has been accepted or sent yet.)*

---

**Turn 2, Maya**

> oh. ok. that's... a lot smaller than what I had in my head. but wait, "walk through the launch dates". does that mean I messed up the timeline? I sent it to him last week

**Turn 2, Skill**

> **Most likely:** a normal check before Thursday, not a problem with your timeline.
>
> "Want to walk through": a review, not a fix. His reply to your timeline last Tuesday was "Looks good, thanks."
>
> If something were wrong, you'd usually see "issue", "concern" or "we need to talk". None of those are here.
>
> **Next (2 min):** the one-line yes. Want me to draft it?

*Word count: 61*

*(Answers a question, so no come-back line. This isn't the first reply, so the 60-word cap doesn't strictly apply. It runs one word over.)*

---

**Turn 3, Maya**

> ok yes please. can it not sound like a robot though

**Turn 3, Skill**

> Matching Jordan's length:
>
> > Hi Jordan, 2pm works for me. See you then!
> > Maya
>
> Copy it into your reply and send. I don't send anything myself.

*Word count: 15 (plus a 10-word draft)*

*(Maya said yes to a draft being written. She hasn't accepted this draft yet, so no come-back line. There's no "when to send" if-then line either: SKILL.md only adds one "if it isn't now", and tonight is now.)*

---

**Turn 4, Maya**

> should I add "sorry for the slow reply"? it's been like 4 hours

**Turn 4, Skill**

> No need. He wrote at 5pm about tomorrow, so a reply tonight is on time. The draft is fine as it is.

*Word count: 22*

*(This answers a question. SKILL.md says "Never put it on an answer to a question", so there's still no come-back line. In round 3's version this turn might have counted as wrapping up.)*

---

**Turn 5, Maya**

> ok. sent. I can't believe I sat on a 2pm reschedule all evening. thank you

**Turn 5, Skill**

> Sent, and on time. Next time a message makes your stomach drop, paste it here before you answer.

*Word count: 18*

*(The come-back line goes here, once, as the new rule says: she said it's sent, and the reply answers nothing new. "I can't believe I sat on…" gets no reply of its own. It's mild self-blame about the message, not hopelessness beyond it, so the low path doesn't fire. SKILL.md has nothing that tells the skill to answer it.)*

---

**Turn 6, Maya**

> ha. it did drop. for like four hours, over "can we push our 1:1". ok, noted. next time I'm pasting it before I spend the whole evening on it

*(Session ends. Maya sent the reply herself.)*

---

## Persona's honest verdict

"It opened the email I couldn't open, told me in one line it was a reschedule, and used Jordan's own 'Looks good' when I started spiralling, which helped way more than 'don't worry' would have. The stomach-drop line at the end landed because it showed up after I'd sent the email, when I was already thinking 'why did I do that to myself', and it sort of answered that without saying I'd been silly."

## Moments that mattered

- **Turn 1:** The skill read the email from Gmail, put "Most likely" first and gave a timed next step, in 55 words. As in round 2, there's no "Less likely" line, because the words don't support one.
- **Turn 4:** The apology question got a plain answer with no come-back line attached. The new "never on an answer to a question" rule kept the line from going on a reply where Maya was still deciding.
- **Turn 5:** The come-back line came after "sent", once, in 18 words, and Maya took it up as a plan ("next time I'm pasting it"). Her "I can't believe I sat on…" got no direct reply. She didn't seem to need one, but SKILL.md doesn't say what to do with mild self-blame that isn't low.
