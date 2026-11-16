# Lab round 2: where-was-i × Dev

- **Persona:** Dev, 27, freelance developer (`lab/personas/dev.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/where-was-i/SKILL.md` (round 2 version)
- **Setup for this run:** Same as round 1. Gmail, Google Calendar and Google Drive are connected. The persona file says Gmail is not connected, but the task setup wins. Dev spent Thu to Sat on a client fire and lost track of two threads: a half-built invoice export feature with notes in a Drive doc, and a client email asking for an estimate by Friday that he hasn't answered.
- **Date in session:** Mon 16 Nov 2026
- **Fictional data the connectors show:** Drive doc "Invoice export – notes", last edited by Dev on Thu 12 Nov. It has a short checklist: "CSV columns" is ticked and "PDF layout" is not. Gmail thread "Estimate for booking flow" from Marta (Halden Supply), received Fri 13 Nov, with no reply from Dev. The body asks for an estimate by Fri 20 Nov. Calendar: "Halden check-in" moved from Tue 17 Nov to Thu 19 Nov at 2pm. No other events.

---

## Transcript

**Turn 1, Dev:**
> ok got sucked into a client fire since thursday. where was i

**Turn 1, Claude:**
*(Reads Gmail, Calendar and Drive activity since Thu 12 Nov without saying so.)*

> **Restart here (5 min):** open "Estimate for booking flow" and list the parts you'd quote, one line each. It's due Friday, so it goes first.
> Marta emailed Friday; no reply yet. Before the fire you were on "Invoice export – notes" (CSV done, PDF next).
> **Waiting on you:** Marta, since Friday, about the estimate.

*(51 words.)*

---

**Turn 2, Dev:**
> ok. parts are booking calendar, stripe checkout, admin view. done

**Turn 2, Claude:**
> Done, that's the skeleton of the quote.
>
> **Where you were:** invoice export (CSV columns done, PDF layout next); Halden booking flow (estimate not sent).
> **What changed since Thursday:** Marta emailed Fri; Halden check-in moved from Tue to Thu 2pm.
> **Waiting on you:** Marta (estimate by Fri).
> **Probably fine to let go:** 14 items.
>
> **Next (5 min):** put a rough number of hours next to each part. Want me to draft the reply to Marta once you have them?

---

**Turn 3, Dev:**
> calendar 4h, stripe 3h, admin 3h. so like 10h, 1.5 days. yeah draft it

**Turn 3, Claude:**
> People often run over; 10h might be 15. Keep it, or add a buffer?

---

**Turn 4, Dev:**
> lol ok fair. i have literally never finished anything in 10h. make it 15

**Turn 4, Claude:**
> Here's a draft. The blanks are for things I don't know.
>
> > Subject: Re: Estimate for booking flow
> >
> > Hi Marta,
> >
> > Thanks for waiting. Here's my estimate for the booking flow (booking calendar, Stripe checkout, admin view):
> >
> > Total: about 15 hours. I can start on [start date]. Cost at my rate: [amount].
> >
> > Happy to go through it at Thursday's check-in.
> >
> > [Your name]
>
> Copy it, or I can save it as an unsent draft in the Gmail thread. Want me to save it?

---

**Turn 5, Dev:**
> save it. start wed, rate is 90/h. also when do i get back to the invoice thing

**Turn 5, Claude:**
*(Fills in start Wednesday and 15 × $90 = $1,350, then saves an unsent Gmail draft in the thread.)*

> Saved as an unsent draft in "Estimate for booking flow": 15 hours, start Wednesday, $1,350. You send it when you're ready.
>
> Invoice export: when you open your laptop tomorrow, open "Invoice export – notes" and start the PDF layout item.
>
> Marta's Friday date matters. Want me to add a reminder for Wednesday?

---

**Turn 6, Dev:**
> nah no calendar stuff. sent it. ok im fading, gonna eat

**Turn 6, Claude:**
> Done: Marta has her estimate, with room in it.
> Next time: open "Invoice export – notes" and start the PDF layout.

*(Session ends.)*

---

## Persona's honest verdict

"ok the 'people often run over' line actually got me, it's one sentence and it didn't lecture me, and for once the quote has the overrun in it before Marta sees it. the extra back-and-forth before the draft was a tiny bit annoying and the calendar thing was pointless again, but i know exactly where the invoice thing picks up tomorrow."

## Moments that mattered

- **Turn 1:** The step is now 5 minutes. It picks the Friday estimate and says why in a few words. The invoice export gets a real last point from the doc ("CSV done, PDF next"), not just "edited Thu". The "due Friday" date comes from the email body, which the skill now allows.
- **Turn 3:** The buffer line came on its own, before any draft. Dev's 10h became 15h in the email. That fixes round 1's main failure. It cost one extra round trip after he'd said "draft it". He accepted it because it was one kind line about his own pattern, but it was still a question before help.
- **Turn 5:** It saved only after "save it". It worked out $1,350 from his rate and showed the number visibly. The calendar offer still came, a Wednesday reminder for an email he sent a minute later. The "won't be done this session" clause didn't stop it, because the step (sending) was technically still open when it asked.
