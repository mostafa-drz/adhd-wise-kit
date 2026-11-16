# Round 1: Dev x admin-sweep

- **Persona:** Dev, 27, freelance developer, time blindness and hyperfocus (`lab/personas/dev.md`)
- **Setup for this run:** Claude desktop app, Google Calendar connected, Gmail connected (added
  for this run). No Drive. Memory not used.
- **Skill:** `plugins/adhd-wise-kit/skills/admin-sweep/SKILL.md`
- **Date in the session:** Monday, Nov 16, 2026, about 10:40

What his inbox has in it (invented, fictional companies and names):

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
read too, nothing admin-related on it. Both reads OK.)*

> Your card payment to Render failed ($38.00, card ending ••42). The email says they retry
> Nov 19 and suspend your services if it's still unpaid after Nov 23.
>
> **Next (3 min):** open Render billing, update the card, press Retry payment.
> dashboard.render.com/billing
>
> **Only you can:** enter the new card and press Retry.

*(51 words. Nothing is due today or tomorrow, so no "Also due" line. The phishing email was seen
in the sweep but not mentioned: one item at a time.)*

---

**Turn 2 — Dev**

> wait theres an email from stripe saying my account is suspended and payouts frozen in 24h??
> thats literally my income. isnt that way worse than 38 bucks

**Turn 2 — Claude**

> That one looks like phishing. It's from stripe-verify-support.co, not stripe.com, and it
> pushes a 24-hour link. Don't click it.
>
> **Next (2 min):** type stripe.com yourself (or use your bookmark) and open your dashboard. A
> real problem would show there.
>
> Then back to the Render card.

---

**Turn 3 — Dev**

> ok stripe is fine lol. my heart rate tho. render done too, card updated

**Turn 3 — Claude**

> Render paid, Stripe fine.
>
> **Do now (2):** October invoice to Lumen Studio (their cutoff is Nov 20), devbuilds.dev domain
> (expires Nov 28, auto-renew off, $17.98).
> **Coming up:** 1, Q4 tax estimate ($3,100, Jan 15, from your accountant's email).
> **Handled:** 3, auto-paid.
>
> **Next (15 min):** make the October invoice and send it. Draft email below; the blanks are
> yours.
>
> > Hi Priya,
> > Here's my invoice for October: [hours] hours, [amount] total. PDF attached.
> > Thanks,
> > Dev
>
> **Only you can:** fill the blanks, attach the PDF, press Send.

---

**Turn 4 — Dev**

> 15 min lol its like 5. 46 hours at 85. also i have to make the pdf in my invoicing app first
> which i hate

**Turn 4 — Claude**

> 46 x 85 = $3,910. Draft updated:
>
> > Hi Priya,
> > Here's my invoice for October: 46 hours, $3,910 total. PDF attached.
> > Thanks,
> > Dev
>
> Making the PDF plus sending is closer to 15 than 5. Still small.
>
> **Next (10 min):** make the PDF in your invoicing app, then attach and send.
>
> Want me to save this as a draft in your Gmail so it's ready?

---

**Turn 5 — Dev**

> yeah save it

**Turn 5 — Claude**

*(Creates a Gmail draft to the Lumen Studio thread. Does not send.)*

> Saved as a draft in the Lumen Studio thread.
>
> **Only you can:** attach the PDF and press Send.

---

**Turn 6 — Dev**

> ok sent. took 20 min bc the app wanted me to update lol. domain next i guess but im kinda
> fading and i have client stuff at 2

**Turn 6 — Claude**

> Done today: Render card fixed, fake Stripe email skipped, invoice sent ($3,910). Next time:
> renew devbuilds.dev before Nov 28 ($17.98, 2 min). When you open your laptop tomorrow
> morning, do the domain first.

**Turn 7 — Dev**

> k thx

*(Session ends. Domain not on his calendar; the calendar offer never happened because the
"fading, stop" rule came first and the offer must be in its own reply.)*

---

## Persona's honest verdict

"honestly the render thing first was right and it caught the fake stripe email before i did
anything dumb, and the replies were short enough that i actually did stuff. but it kinda sat on
that stripe email till i panicked about it, and the domain is gonna slip because nothing put it
anywhere i'll see it."

## Moments that mattered

- **Turn 1–2:** The sweep saw the phishing email but the one-item rule kept it hidden. Dev found
  it himself and panicked. The flag was right when it came (sender domain, no link, real site
  first), but a fake 24-hour threat should get one line up front.
- **Turn 4:** Honest time ("closer to 15 than 5") was right for Dev's time blindness, and it
  came true (20 min). The amount came only from his own numbers, not guessed.
- **Turn 6:** "Fading, stop" and "calendar offer in its own reply" clash. The skill stopped
  correctly, but the Nov 28 domain date never got onto his calendar. The only cue was an if-then
  line that a time-blind person may lose.
