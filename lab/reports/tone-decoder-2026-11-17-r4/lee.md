# Tone Decoder, round 4: Lee (Check mode, nothing connected, privacy question)

- **Persona:** `lab/personas/lee.md`. Claude desktop app, nothing connected, Claude Max.
- **Skill under test:** `adhd-wise-skills/plugins/adhd-wise-free/skills/tone-decoder/SKILL.md` (round 4 version: the come-back line comes only after they accept a draft or cleaned-up version or say it's sent, and never goes on an answer to a question).
- **Opening and later turns:** same as round 3b, word for word. Turn 2 changes because the privacy answer no longer carries the come-back line. Turn 4 now gets a skill reply, because "Sent the Rui one" is where SKILL.md puts the line. Turn 5 is new.
- **Word counts** cover the skill's own words. Cleaned-up versions are counted separately, because SKILL.md leaves them out of the 60-word limit. Numbers and quoted words count as words; arrows and markdown don't. Counts were redone for this round, so a few differ from round 3 for the same text.

---

**Turn 1, Lee**

> Convince me this isn't another tool I'll stop using in a week. Here's a Slack message to a peer. Does it read as rude?
>
> "Rui, I need the vendor access list by Thursday. I've already asked twice and the audit is blocked on it. Can you send it or tell me who has it?"

**Turn 1, Skill**

> Lands as firm and clear; "I need" plus "already asked twice" might read as a bit sharp.
>
> > Hi Rui, I need the vendor access list by Thursday. I've asked twice now and the audit is blocked on it. Could you send it, or tell me who has it?
>
> Changed: "Rui," → "Hi Rui,", "I've already asked twice" → "I've asked twice now", "Can you" → "Could you".
>
> **Next (1 min):** copy it and send it, or tell me what's off.

*Word count: 44 (plus the 29-word cleaned-up version)*

*(Same content as round 3. The landing line is now one sentence, as Check step 1 says. "Convince me" still has no rule in SKILL.md, so the skill just runs Check mode. The deadline and "asked twice" stay in. There's no come-back line: nothing has been accepted yet.)*

---

**Turn 2, Lee**

> Fine. It's barely different, which is honestly what I wanted. Thursday's still there. Before I paste anything real in: what are you keeping? Names, my coworker's messages, any of it?

**Turn 2, Skill**

> This skill saves nothing itself. Whether Claude remembers chats depends on your memory setting in Claude, which you control. You can swap names for "X" and it works the same.

*Word count: 29*

*(Lee's "Fine… what I wanted" reads as accepting the cleaned-up version, but in the same message they ask a question. SKILL.md says "Never put it on an answer to a question", so there's no come-back line. Round 3b's "Paste the next one whenever it's bugging you" is gone too. The reply ends on the answer.)*

---

**Turn 3, Lee**

> Where's that setting? And "works the same": even if I strip the names, you still see the content.

**Turn 3, Skill**

> In Claude's settings; look for the memory option. I can't see or change it from here. And yes: I still read the message itself. Swap anything else you'd rather not share for "X" too; the tone read works on the wording.

*Word count: 41*

*(Same as round 3b. It answers a question, so no come-back line. SKILL.md still says nothing about where the setting is, so the answer stays general.)*

---

**Turn 4, Lee**

> Okay. Straight answer, at least. Sent the Rui one. We'll see if I remember this exists next week.

**Turn 4, Skill**

> Sent. Next time a message makes your stomach drop, paste it here before you answer.

*Word count: 15*

*(The come-back line goes here, once: Lee said it's sent, and nothing new needed answering. It happens to land right after "We'll see if I remember this exists". The wording is SKILL.md's example, which is written for received messages ("before you answer"). Lee's use was checking their own outgoing draft.)*

---

**Turn 5, Lee**

> My stomach doesn't drop over Slack. I just don't want to sound like a jerk to Rui. But fine, one line, no "see you tomorrow", no streak. I'll take it.

*(Session ends. Lee sent the message themselves.)*

---

## Persona's honest verdict

"It fixed the message in one pass, kept my deadline and my 'asked twice', answered the privacy questions straight, and didn't tack a pitch onto them this time. The come-back line came at the right moment, after I'd sent it, but 'stomach drop' is someone else's problem. Mine is not sounding like a jerk, so it reminded me of the tool without really describing why I'd use it."

## Moments that mattered

- **Turn 1:** The cleaned-up version kept "by Thursday" and "asked twice", with one "Changed:" line and a timed Next step, in 44 words. For Lee, the work was the answer to "convince me".
- **Turn 2:** The privacy answer came with nothing attached. In round 3b the come-back line went here a turn early. The "never on an answer to a question" rule fixed that, even though Lee's message also half-accepted the draft.
- **Turn 4–5:** The line showed up once, after "sent", and Lee called it acceptable because it wasn't a streak. The fixed wording ("stomach drop", "before you answer") fits Decode, not a Check-mode session about one's own draft, and Lee pointed out the mismatch.
