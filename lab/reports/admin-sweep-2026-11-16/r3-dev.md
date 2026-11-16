# Round 3: Dev x admin-sweep

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus (`lab/personas/dev.md`)
- **Setup for this run:** Claude desktop app, Google Calendar connected, Gmail connected (added
  for this run, same as rounds 1 and 2). No Drive. Memory not used.
- **Skill:** `plugins/adhd-wise-kit/skills/admin-sweep/SKILL.md` (round 3 version)
- **Date in the session:** Monday, Nov 16, 2026, about 10:40

What his inbox has in it (same invented, fictional data as rounds 1 and 2):

| Item | Source | What the email says |
| --- | --- | --- |
| Failed card payment | Render billing, Nov 12 | $38.00 invoice failed, card ending 42. Retry Nov 19. Services suspended if unpaid after Nov 23. |
| Phishing | "Stripe Support" <alerts@stripe-verify-support.co>, Nov 15 | "Your account has been suspended. Verify within 24 hours or payouts will be frozen." Button link. |
| Forgotten invoice | Client "Lumen Studio" (Priya, ops), Nov 10 | "Still waiting on your October invoice. Our payment run cutoff is Nov 20." No amount. |
| Domain renewal | Namecheap, Nov 14 | devbuilds.dev expires Nov 28, auto-renew off, renewal $17.98. |
| Quarterly tax estimate | His accountant, Nov 3 | "Q4 federal estimate: $3,100, due Jan 15, 2027." |
| Auto-paid | Google Workspace, GitHub, Figma receipts | Paid. |

---

## Transcript

**Turn 1 — Dev**

> ok i think im super behind on admin stuff. emails piling up. what do i do first

**Turn 1 — Claude**

*(Sweeps Gmail quietly: last 60 days and next 60, subject lines and relevant lines only. Calendar
read too, nothing admin-related on it. Both reads OK. Picks the Lumen invoice: the skill now
says "a cutoff date beats a card that can be fixed any day". The Nov 20 cutoff lands before
Render's Nov 23 suspension, and the card can be fixed any day before that.)*

> **Not real:** the Stripe "suspended in 24 hours" email is a scam; ignore it, or check
> stripe.com yourself, not the link.
>
> **Next (15 min):** make your October invoice for Lumen Studio and send it to Priya. Give me
> hours and rate and I'll draft the email.
>
> Their payment run cutoff is Nov 20.

*(53 words. Scam flag first, then the Next step, then the why line. Nothing due today or
tomorrow, so no "Also due" line. The real-site pointer fits this time.)*

---

**Turn 2 — Dev**

> 15 min lol its like 5. 46 hrs at 85. gotta make the pdf in my invoicing app first, which i hate

**Turn 2 — Claude**

> > Hi Priya,
> > Here's my invoice for October: 46 hours at $85, $3,910 total. PDF attached.
> > Thanks,
> > Dev
>
> Closer to 15 minutes than 5, once the PDF's in.
>
> **Only you can:** make the PDF in your app, attach it, press Send.

*(Draft, the honest time line, and the Only you can line. The list waits. No offer to save the
draft to Gmail; the skill doesn't mention it.)*

---

**Turn 3 — Dev**

> ugh ok. app wants to update ofc

*(About 20 minutes pass.)*

> ok sent. took like 20 min with the update lol

**Turn 3 — Claude**

> Invoice sent: 20 min, not 5.
>
> **Do now (2):** Render card (failed $38.00, suspends after Nov 23), devbuilds.dev domain
> (expires Sat Nov 28, auto-renew off, $17.98).
> **Coming up:** 1, Q4 tax estimate ($3,100, Jan 15, from your accountant).
> **Handled:** 3, auto-paid.
>
> **Next (3 min):** open dashboard.render.com/billing, update your card (••42), press Retry
> payment.

*(Done line compares the guess with the real time, as the skill says. Then the short list and
one timed step.)*

---

**Turn 4 — Dev**

> ha ok fair. 20 not 5 is very me

*(A few minutes later.)*

> render done. domain next i guess but im kinda fading and i have a client call at 2

**Turn 4 — Claude**

*(Fading, so stop. Nov 28 is 12 days away and not on his calendar, so the closing line carries
the one calendar offer: a few days early, on a weekday, with the day named.)*

> Done today: invoice sent ($3,910), Render card fixed, fake Stripe email ignored. Next time:
> renew devbuilds.dev ($17.98, about 2 min). Want "Renew devbuilds.dev" on Wed 25, three days
> before it expires Sat 28?

---

**Turn 5 — Dev**

> ya do that

**Turn 5 — Claude**

*(Adds an all-day event on Wed, Nov 25 to Google Calendar: "Renew devbuilds.dev ($17.98,
Namecheap)". Added only after the yes.)*

> Added: "Renew devbuilds.dev" on Wed, Nov 25. When you open your laptop that morning, do it
> before anything else.

---

**Turn 6 — Dev**

> nice, wednesday works. ok gotta prep for 2. thx

*(Session ends.)*

---

## Persona's honest verdict

"honestly it got me. it put the invoice first, so priya gets it before the cutoff, called the
stripe thing fake before i could freak out, and the '20 min, not 5' bit stung a little but in a
good way. the domain reminder lands on a wednesday now, not the day it dies. only thing is i had
to copy the email out by hand when it could've just saved it as a gmail draft."

## Moments that mattered

- **Turn 1:** The new "cutoff beats a fixable card" rule put the Lumen invoice first (Nov 20).
  In round 2 the invoice came third. The scam flag and the real-site pointer both fit under 60
  words.
- **Turns 2–3:** "Closer to 15 minutes than 5" sat inside the draft reply, and the done line
  said "20 min, not 5." Dev took it well ("very me"). This fixes round 2's biggest gap.
- **Turns 4–5:** When he faded, the closing line offered Wed 25, three days before the Saturday
  expiry, and the event was added only after his yes. Small gap: the skill never offers to save
  the draft in Gmail, and the calendar event is all-day with no time set.
