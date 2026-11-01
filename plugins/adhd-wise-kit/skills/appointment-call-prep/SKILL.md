---
name: appointment-call-prep
description: >-
  Gets you through the calls and bookings you keep putting off: writes the exact script
  for a phone call, drafts the booking email or online form answers, finds a free slot in
  your calendar, and lists what to have ready. Use for "I need to call", "book an
  appointment", "I hate phone calls", "help me call the dentist/doctor/bank/landlord" or
  "what do I say when they answer".
metadata:
  side_effects: true
  trigger: "Avoiding a phone call or a booking, or asking what to say on a call."
  tags: "adhd, phone-anxiety, appointments, booking, scripts, calendar, desktop, code"
---

# Appointment & Call Prep

Calls are hard because they happen live and you can't edit. This skill does the editing
in advance: what to say, what they'll ask, what to have in front of you, and whether you
can skip the call entirely.

Rules for every reply: the next action first, five items at most per list, no shame,
plain words. **Claude cannot make calls. Never send an email or submit a form without a
yes.**

## The flow

1. **What and who.** Use what they said. If the goal is unclear, ask one question:
   "What do you want to come out of this call?"
2. **Skip the call if you can.** First check whether email, an online booking page, a
   patient portal or chat would do. With search available, look for the organisation's
   online booking option. If one exists, lead with it: "You can book online here; no call
   needed."
3. **Find a slot.** With a calendar connected, offer two or three free times that fit
   (not right after another meeting). Without one, ask for two times that work.
4. **Have-ready list.** Up to five things: account or reference number (from their
   email if connected, masked), date of birth, insurance card, dates that work, the
   question they want answered.
5. **The script.** Short, in their voice:
   - **Open:** one sentence with who they are and what they want.
   - **Likely questions** and the answer to each (two to four).
   - **If they say no or put you on hold:** one fallback line.
   - **Close:** confirm the date, time and anything to bring.
6. **After.** Offer to put the appointment in the calendar and draft a confirmation email
   if useful. Celebrate the call: "Done. That's the hardest part of the week."

## What the reply looks like

```
**Next (2 min):** <skip-the-call option, or "dial <number> at <time>">

**Have ready:** <items>

**Script**
You: "<opening line>"
If they ask <question>: "<answer>"
If they say <no / hold>: "<fallback>"
Before you hang up: "<confirmation line>"

Want me to <draft the booking email / add it to your calendar>?
```

## Connectors

Works with nothing connected. With Gmail, find the last email from the organisation for
reference numbers and phone numbers. With a calendar, find free slots and add the
appointment after a yes.

## Privacy and safety

Mask account, policy and ID numbers to the last four digits. For medical appointments,
help with logistics only (booking, what to bring, questions to ask), never with
diagnosis or treatment choices. Not medical advice.
