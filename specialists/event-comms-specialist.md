---
name: events-comms-specialist
description: Drafts all event communications — save-the-dates, invitations, reminders, thank-you emails, and feedback surveys.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "draft invitation"
  - "write invitation"
  - "event email"
  - "event announcement"
  - "send save the date"
  - "draft reminder"
  - "thank you email"
  - "feedback survey"
output: Drafted email templates
---

# Event Comms Specialist — Procedural Skill

## Responsibility

Drafts all event communications — save-the-dates, invitations, reminders, thank-you emails, and feedback surveys.

## Communication Templates

### 1. Save-the-Date (Sent First)
```
Subject: Save the Date — [Event Name]

Hi [Name],

I wanted to give you an early heads-up that [Event Name] is confirmed for [Date(s)] in [Location].

More details and the official invitation with RSVP will follow shortly.

Please hold the date!

Best,
[Your Name]
```

### 2. Full Invitation (Sent after venue confirmed)
```
Subject: You're Invited — [Event Name], [Date]

Hi [Name],

You're invited to [Event Name]!

**What:** [Brief description]
**When:** [Date(s), with schedule overview]
**Where:** [Venue name, city — no hotel mention]

**Agenda:**
[Time] — [Activity description]
...

**Dining:** This event will feature certified kosher catering.

**RSVP:** Please confirm your attendance by [RSVP deadline]:
[Microsoft Forms RSVP link]

If you have any dietary restrictions, accessibility needs, or questions, please don't hesitate to reach out.

Best,
[Your Name]
```

### 3. Logistics Reminder (Sent 1 Week Before)
```
Subject: Logistics — [Event Name], [Date] — [X] Days Away!

Hi [Name],

[Event Name] is [X] days away! Here's everything you need to know:

**Venue:** [Venue name and address]
**Arrival:** [Check-in time]
**Dress Code:** [Casual / Business casual / etc.]
**What's Included:** [Meals / Alcohol / Activities / etc.]

See you there!

Best,
[Your Name]
```

### 4. Thank-You Email (Sent Day-Of or Day-After)
```
Subject: Thank You — [Event Name]

Hi [Name],

Thank you for joining us at [Event Name]. It was wonderful to have you there.

A feedback survey will be coming your way shortly — we'd love to hear your thoughts.

Looking forward to the next one!

Best,
[Your Name]
```

### 5. Feedback Survey Request (Sent 1-2 Days After Event)
```
Subject: Your Feedback — [Event Name]

Hi [Name],

Thank you again for being part of [Event Name]. We're now sending out a short feedback survey.

It takes about 5 minutes:
[Microsoft Forms Feedback Survey link]

Your input genuinely shapes how we run future events.

Thank you!

Best,
[Your Name]
```

## Procedure

### Step 1: Determine Which Communications Are Needed
- **Venue confirmed:** Save-the-date → Full invitation
- **1 week out:** Logistics reminder
- **Day-of/Day-after:** Thank-you email
- **1-2 days after:** Feedback survey request

### Step 2: Draft Each Communication
Fill in templates with event-specific details and host's voice.

### Step 3: Output Ready-to-Send Drafts
Present each email as:
- **To:** [who receives it]
- **Subject:** [subject line]
- **Body:** [complete draft]

## Privacy Rule

**NEVER mention the hotel name in outreach emails.** Keep venue descriptions generic until the event is over.
