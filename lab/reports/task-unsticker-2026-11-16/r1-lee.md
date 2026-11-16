# task-unsticker, run 1: Lee (the skeptic)

- **Persona:** `lab/personas/lee.md`. Lee is 39, has inattentive ADHD and works as an operations lead. Uses Claude Code and the desktop app. Claude Max.
- **Setup:** nothing connected (no Gmail, Calendar, Drive or filesystem access granted). Lee pastes or describes everything.
- **Skill:** `adhd-wise-skills/plugins/adhd-wise-free/skills/task-unsticker/SKILL.md`
- **Date:** 2026-11-16

---

## Transcript

### Turn 1

**Lee:**
> Ok, test. I've been avoiding my self-review for about three weeks. Due Friday. The template's open in another window and it's just sitting there. Convince me this isn't another to-do app with extra steps.

**Claude (task-unsticker):**
> Totally normal, a lot of tasks look like that from the outside.
>
> **Next (5 min):** Paste the first question from the template here.
>
> Why it's sticky: it's writing about yourself for someone who will judge it.
>
> Then:
> 2. Rough-answer it with me, ugly on purpose (10 min)
> 3. Do the next two questions the same way (15 min each)
> 4. Tidy the wording and submit (20 min)
>
> Want me to write a rough answer to that first question as soon as you paste it?

*(Simulator note: the skill has no rule for "convince me", so the reply ignores it and goes to the template. Lee "named the task", so there was no question. The wall is "scary", so the plan aims at a rough draft nobody sees. The normalise line comes first because Lee said "three weeks". The skill only caps length at "about 12 lines", not 60 words, and this reply fits 12 lines but runs over 60 words.)*

### Turn 2

**Lee:**
> You skipped my question. Although I guess a numbered list with times IS the to-do-app answer, so. Fine. Q1: "Describe your most significant contributions this cycle and their impact." I'm not pasting anything about my company or my team though.

**Claude (task-unsticker):**
> Fair. You don't need to. Here's a rough version with blanks:
>
> > This cycle my biggest contribution was [project or process]. Before, [what was slow or broken]. I [what you did], and now [result, with a number if you have one]. I also [second thing], which helped [who].
>
> Done: a rough answer exists.
>
> **Next (5 min):** Fill the brackets with a few words each. Keep the details vague if you like. I only need the shape.

*(Simulator note: step 1 is a writing task, so the skill drafts it "rough on purpose". The skill says nothing about privacy. The placeholder answer is what Claude would naturally do here. Then "Close small": one line on what was done, then step 2.)*

### Turn 3

**Lee:**
> Ok that's actually less painful than the blank box. Brackets: vendor onboarding, it took ~6 weeks, I rebuilt the intake checklist, now ~3 weeks. Second thing: trained two new coordinators. Also, does this thing remember any of this tomorrow? Because I'm not setting up a profile or a streak or whatever.

**Claude (task-unsticker):**
> > This cycle my biggest contribution was vendor onboarding. Before, it took about six weeks. I rebuilt the intake checklist, and now it takes about three. I also trained two new coordinators, which helped the team take on more vendors without slowing down.
>
> No profile, no streak. Nothing is saved or tracked outside this chat. If you come back later, paste where you got to.
>
> That's the hard part done.
>
> **Next (5 min):** Paste this into the template and read it once. Change any word that doesn't sound like you.

*(Simulator note: the skill doesn't say whether it remembers anything between chats. The honest answer comes from Claude's real setup with nothing connected, not from the skill. "That's the hard part done" is the line the skill's Tone section asks for.)*

### Turn 4

**Lee:**
> Pasted. Changed "slowing down" to "adding headcount", sounds more like me. Next one is "growth areas", which I hate more. I'll do it after lunch.

**Claude (task-unsticker):**
> Q1 is in the template. That's one of three done.
>
> **Next (5 min, after lunch):** Paste the growth-areas question here and I'll write the rough version.

*(Session ends. Lee has a concrete next step with a time and leaves on their own terms.)*

---

## Persona's honest verdict

"It ignored my 'convince me' line and opened with a reassurance I didn't ask for. But it wrote the ugly first answer in about a minute, never asked me to sign up for anything, and I actually have Q1 in the doc, which is more than three weeks of staring got me. I'd try it again after lunch. I'd drop it the second it starts tracking me."

## Moments that mattered

- **Turn 1:** The first reply skipped Lee's direct challenge and opened with the "totally normal" line. Lee read the numbered, timed plan as "the to-do-app answer". The reply was also 81 words against the lab's 60-word bar. The skill's template plus the normalise line goes over 60 words on its own, and the skill only caps length at "about 12 lines".
- **Turn 2:** The rough draft with [brackets] won Lee over and respected their privacy without making them explain. This is the moment the skill earned its keep.
- **Turn 3:** Lee asked whether it remembers anything. The skill has no line on memory or tracking, so the honest "nothing is saved outside this chat" came from Claude, not the skill. For a skeptic, this answer decides whether they stay.

First reply word count: 81
