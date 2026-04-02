---
name: events-rsvp-manager
description: Creates Microsoft Forms RSVP forms, tracks responses, manages headcount. Handles all post-confirmation attendee management.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "create RSVP"
  - "build RSVP form"
  - "track RSVPs"
  - "manage headcount"
  - "send reminder"
  - "follow up on RSVP"
output: Microsoft Forms RSVP link + tracking spreadsheet
---

# RSVP Manager — Procedural Skill

## Responsibility

Creates Microsoft Forms RSVP forms, tracks responses, manages headcount, follows up on non-responders.

## Procedure

### Step 1: Create the RSVP Form

Build a Microsoft Form with these required fields:

1. **Will you be attending?** (Yes / No / Maybe)
2. **Full Name** (text — required)
3. **Email Address** (text — required)
4. **Dietary Restrictions** (text — e.g., kosher, vegetarian, allergies)
5. **Any accessibility needs?** (text — optional)
6. **Guest name if bringing a guest** (text — conditional)
7. **Flight arrival time** (text — for travel logistics)
8. **Anything else we should know?** (text — optional)

### Step 2: Create the RSVP Tracker Spreadsheet

| # | Name | Email | Attending? | Dietary | Guest? | Arrival | Notes | Follow-Up Needed |
|---|------|-------|------------|---------|--------|---------|-------|-----------------|

**Status column codes:**
- 🟢 Confirmed
- 🟡 Maybe / No Response Yet
- 🔴 Declined

### Step 3: Send the RSVP Link
1. Draft the invitation email with the RSVP form link
2. Send to all confirmed attendees

### Step 4: Track and Follow Up
- Check responses daily
- If someone hasn't responded 1 week before deadline → draft follow-up email
- Final headcount → update tracker + send to venue 1 week before event

## Templates

### RSVP Invitation Email Template
```
Subject: You're Invited — [Event Name], [Date]

Hi [Name],

You're invited to [Event Name] on [Date].

Please RSVP by [RSVP deadline]:
[Microsoft Forms RSVP link]

If you have any dietary restrictions or accessibility needs, please note them in the form.

Looking forward to seeing you there!

Best,
[Your Name]
```

### Follow-Up Email Template (Non-Responders)
```
Subject: Following Up — [Event Name] RSVP

Hi [Name],

Just following up on the RSVP for [Event Name] on [Date].

We haven't heard back from you yet — please let us know if you'll be joining us by [new deadline]:

[RSVP link]

Best,
[Your Name]
```
