# Tone Decoder, round 2: Maya (Decode mode, Gmail connected)

- **Persona:** `lab/personas/maya.md`. claude.ai on a laptop, Gmail and Calendar connected, Claude Pro.
- **Skill under test:** `adhd-wise-skills/plugins/adhd-wise-free/skills/tone-decoder/SKILL.md` (with TD-1 to TD-4 applied).
- **Opening:** same situation as round 1. It's a weekday, about 9pm. An email from her manager came in around 5pm and she still hasn't opened it.
- **Word counts** cover the skill's own words. Drafts and cleaned-up versions are counted separately, because SKILL.md leaves them out of the 60-word limit.

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

*Word count: 52* (no "Less likely" line, since nothing in the email supports one)

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

*Word count: 63*

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

---

**Turn 4, Maya**

> should I add "sorry for the slow reply"? it's been like 4 hours

**Turn 4, Skill**

> No need. He wrote at 5pm about tomorrow, so a reply tonight is on time. The draft is fine as it is.

*Word count: 22*

---

**Turn 5, Maya**

> ok. sent. I can't believe I sat on a 2pm reschedule all evening. thank you

*(Session ends. Maya sent the reply herself.)*

---

## Persona's honest verdict

"It opened the thing I couldn't open and told me in one line it was a reschedule, and then it gave me something to do with that instead of leaving me staring at it. When I tried to spiral about the launch dates it used Jordan's own 'Looks good' from last week, which landed much better than being told not to worry."

## Moments that mattered

- **Turn 1:** The skill read the email from Gmail and put "Most likely" first, with a timed next step, in 52 words. This is round 1's "I read it" moment, now with somewhere to go.
- **Turn 2:** It used Jordan's earlier reply from the connected thread as evidence against the new worry. It added no "Less likely" line, because the words didn't support one.
- **Turn 4:** It talked her out of an apology the email didn't call for. SKILL.md's anti-apology rule is only written for Check mode, but here it came out of the Decode reasoning ("on time").
