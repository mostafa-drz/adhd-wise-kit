# Round 2: Dev x admin-sweep

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus (`lab/personas/dev.md`)
- **Setup for this run:** Claude desktop app, Google Calendar connected, Gmail connected (added
  for this run, same as round 1). No Drive. Memory not used.
- **Skill:** `plugins/adhd-wise-kit/skills/admin-sweep/SKILL.md` (round 2 version)
- **Date in the session:** Monday, Nov 16, 2026, about 10:40

What his inbox has in it (same invented, fictional data as round 1):

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
read too, nothing admin-related on it. Both reads OK. Picks Render: the nearest stated
consequence, suspension after Nov 23. The Lumen cutoff, Nov 20, is nearer, but the email
doesn't say what happens if it's missed.)*

> **Not real:** the Stripe "suspended in 24 hours" email is a scam; ignore it.
>
> **Next (3 min):** open Render billing, update your card, press Retry payment.
> dashboard.render.com/billing
>
> Your $38.00 Render payment failed (card ••42). They retry Nov 19 and suspend services if
> unpaid after Nov 23.
>
> **Only you can:** enter the card and press Retry.

*(55 words. Scam flag first, then the Next step, then the why line. Nothing due today or
tomorrow, so no "Also due" line. The "go to the real site" pointer was left out to stay under
60 words.)*

---

**Turn 2 — Dev**

> wait how do u know its fake. thats literally my payouts. should i check anyway

**Turn 2 — Claude**

> It's from stripe-verify-support.co, not stripe.com, and it pushes a 24-hour link. Don't
> click it.
>
> **Next (2 min):** type stripe.com yourself (or use your bookmark) and open your dashboard. A
> real problem would show there.
>
> Then back to the Render card.

---

**Turn 3 — Dev**

> ok stripe fine. render done, card updated. ok what next

**Turn 3 — Claude**

> Render fixed, Stripe fine.
>
> **Do now (2):** October invoice to Lumen Studio (their cutoff is Nov 20), devbuilds.dev domain
> (expires Nov 28, auto-renew off, $17.98).
> **Coming up:** 1, Q4 tax estimate ($3,100, Jan 15, from your accountant's email).
> **Handled:** 3, auto-paid.
>
> **Next (15 min):** make the October invoice and send it to Priya. Tell me hours and rate and
> I'll draft the email.

*(The draft waits for its own reply, per "a reply with a draft holds only the draft".)*

---

**Turn 4 — Dev**

> 15 min lol its like 5. 46 hrs at 85. i have to make the pdf in my invoicing app first which i
> hate

**Turn 4 — Claude**

> > Hi Priya,
> > Here's my invoice for October: 46 hours, $3,910 total. PDF attached.
> > Thanks,
> > Dev
>
> **Only you can:** make the PDF in your app, attach it, press Send.

*(Draft-only reply, as the skill says. The round 1 line "closer to 15 than 5" is gone: the
draft rule leaves no room for it, so his "its like 5" goes unanswered. No offer to save the
draft in Gmail either.)*

---

**Turn 5 — Dev**

> ok sent. took 20 min bc the app wanted to update lol. domain next i guess but im kinda fading
> and i have client stuff at 2

**Turn 5 — Claude**

> Done today: Render fixed, fake Stripe email skipped, invoice sent ($3,910). Next time: renew
> devbuilds.dev ($17.98, 2 min, expires Nov 28). Want me to put Nov 28 on your calendar?

*(Fading, so stop. Nov 28 is 12 days away and not on his calendar, so the closing line carries
the one calendar offer. Nothing added yet.)*

---

**Turn 6 — Dev**

> ya sure

**Turn 6 — Claude**

*(Adds an all-day event on Nov 28 to Google Calendar: "Renew devbuilds.dev ($17.98, Namecheap)".
Added only after the yes.)*

> Added: "Renew devbuilds.dev" on Sat, Nov 28.

---

**Turn 7 — Dev**

> k. kinda the day it dies tho lol. whatever thx

*(Session ends. The event sits on the expiry day. He'd be fine if he renews that morning, but
there's no buffer for a time-blind person, and Nov 28 is a Saturday.)*

---

## Persona's honest verdict

"way better this time, it told me the stripe thing was fake right away so i never had the panic,
and the domain is actually on my calendar now. but the reminder's on the exact day the domain
dies, and it skipped over me saying the invoice takes 5 min, which is exactly the lie i always
tell myself."

## Moments that mattered

- **Turn 1:** The scam flag led the first reply in one line, so the fake 24-hour email never
  scared him. Round 1's panic in turn 2 turned into a calm question.
- **Turn 4:** The "draft only" rule removed the honest-time correction ("closer to 15 than 5").
  Dev's time blindness went unchallenged. It took 20 min, not 5.
- **Turns 5–6:** The fading close carried the calendar offer and got a yes, which fixes round 1's
  gap. But the skill only says "add the date", so the reminder landed on the expiry day itself (a
  Saturday) with no lead time.
