# Lab round 1: where-was-i × Dev

- **Persona:** Dev, 27, freelance developer (`lab/personas/dev.md`)
- **Skill:** `plugins/adhd-wise-kit/skills/where-was-i/SKILL.md`
- **Setup for this run:** Gmail, Google Calendar and Google Drive connected. (This differs from the persona file, which says Gmail is not connected. The task setup wins.) Dev spent Thu to Sat on a client fire and lost track of two threads: a half-built invoice export feature with notes in a Drive doc, and a client email asking for an estimate by Friday that he hasn't answered.
- **Date in session:** Mon 16 Nov 2026
- **Fictional data the connectors show:** Drive doc "Invoice export – notes", last edited by Dev on Thu 12 Nov. Gmail thread "Estimate for booking flow" from Marta (Halden Supply), received Fri 13 Nov, no reply from Dev. The email asks for an estimate by Fri 20 Nov. Calendar: the "Halden check-in" moved from Tue 17 Nov to Thu 19 Nov at 2pm. No other events.

---

## Transcript

**Turn 1, Dev:**
> ok got sucked into a client fire since thursday. where was i

**Turn 1, Claude:**
*(Reads Gmail, Calendar and Drive activity since Thu 12 Nov without saying so.)*

> **Restart here (10 min):** open Marta's email "Estimate for booking flow" and list the parts you'd need to quote, one line each.
> It arrived Friday and the estimate is due this Friday, so it goes first. Your last work was "Invoice export – notes" (edited Thu).
> **Waiting on you:** Marta, since Friday, about the estimate.

*(54 words.)*

---

**Turn 2, Dev:**
> ok. parts are booking calendar, stripe checkout, admin view. done

**Turn 2, Claude:**
> Done, that's the skeleton of the quote.
>
> **Where you were:** invoice export (notes doc, last edited Thu); Halden booking flow (estimate not sent).
> **What changed since Thursday:** Marta emailed Fri; Halden check-in moved from Tue to Thu 2pm.
> **Waiting on you:** Marta (estimate by Fri).
> **Probably fine to let go:** 14 items.
>
> **Next (10 min):** put a rough number of hours next to each of the three parts. Want me to draft the reply to Marta once you have them?

---

**Turn 3, Dev:**
> calendar 4h, stripe 3h, admin 3h. so like 10h, 1.5 days. yeah draft it

**Turn 3, Claude:**
> Here's a draft. The blanks are for things I don't know.
>
> > Subject: Re: Estimate for booking flow
> >
> > Hi Marta,
> >
> > Thanks for waiting. Here's my estimate for the booking flow:
> >
> > - Booking calendar: 4 hours
> > - Stripe checkout: 3 hours
> > - Admin view: 3 hours
> >
> > Total: about 10 hours (1.5 days). I can start on [start date]. Cost at my rate: [amount].
> >
> > Happy to go through it at Thursday's check-in.
> >
> > [Your name]
>
> Copy it, or I can save it as an unsent draft in Gmail. Do you want me to save it?

---

**Turn 4, Dev:**
> save it. start date wed, rate is 90/h so 900. also when do i get back to the invoice thing

**Turn 4, Claude:**
*(Fills in the blanks and saves an unsent Gmail draft in the thread.)*

> Saved as an unsent draft in the "Estimate for booking flow" thread: start Wednesday, $900. You send it when you're ready.
>
> Invoice export: when you open your laptop tomorrow, open "Invoice export – notes" first and write the next line.
>
> Marta's Friday date matters. Want me to add a reminder for Wednesday?

---

**Turn 5, Dev:**
> nah no calendar stuff. sent it. ok im fading, gonna eat

**Turn 5, Claude:**
> Done: Marta has her estimate.
> Next time: open "Invoice export – notes" and write the next line.

*(Session ends.)*

---

## Persona's honest verdict

"honestly it got me moving on the right thing in like ten seconds and i sent the estimate, which normally sits for days. but it just put my 10 hours straight into the email and i've never once finished anything in 10 hours, so i'll probably be pulling an all-nighter on thursday."

## Moments that mattered

- **Turn 1:** It picked the Friday estimate over the half-built feature and said why in a few words. That was the right call for someone who misses deadlines. But "due this Friday" comes from the email body, which bends the "quote subject lines, not contents" rule. And "edited Thu" isn't a real last concrete point for the feature, so that thread never really got rebuilt.
- **Turn 3:** The draft used Dev's own guess of 10h with no buffer. The skill says to use only facts he gave, and it has no rule for time blindness, so the likely underestimate went straight to the client. This is the opposite of Dev's "a plan that already accounts for him being late."
- **Turn 4:** It saved the Gmail draft only after he said yes, and it offered the calendar reminder once. Dev said no, and it didn't ask again. The "a few days early" rule turned into a Wednesday reminder for a task he was about to finish anyway, so the offer felt pointless.
