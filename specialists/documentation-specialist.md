---
name: events-documentation-specialist
description: Creates and maintains Excel venue trackers, PowerPoint proposal decks, and event documentation.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "build tracker"
  - "create excel"
  - "update tracker"
  - "build deck"
  - "create proposal"
  - "update deck"
output: Excel workbook, PowerPoint deck, event documentation
---

# Documentation Specialist — Procedural Skill

## Responsibility

Creates and maintains the Excel venue tracker and PowerPoint proposal deck for every event.

## Output Convention

**Naming pattern:**
- Excel: `[EventName]_Venue_Tracker.xlsx`
- PowerPoint: `[EventName]_Proposals.pptx`

## Part 1: Build the Excel Venue Tracker

Create an Excel workbook with 3 sheets:

**Sheet 1: Master Venue Log**
| Column | Content |
|--------|---------|
| # | Row number |
| Property | Full venue name |
| Location | City, Country/State |
| Type | Hotel / Restaurant / Resort / Estate |
| Phone | Main contact number |
| Email | Main contact email |
| Website | URL |
| Est. Cost/Night | Per person or per night estimate |
| Outside Catering | ✅ Yes / ❌ No / ❓ Ask |
| Kosher Path | Confirmed caterer or restaurant name |
| Capacity | Room count AND event space capacity |
| Vibe | 1-2 sentence description |
| A/V Available | ✅ / ❌ |
| Private Space | ✅ / ❌ |
| Status | Active 🟢 / Rejected 🔴 / Closed 🟣 |

**Sheet 2: Outreach Tracker**
| Column | Content |
|--------|---------|
| Property | Full venue name |
| Email Sent | Date sent |
| Response | Yes / No / Pending |
| Response Date | Date received |
| Follow-Up Needed | Yes / No |
| Notes | **BLANK — personal space** |

**Sheet 3: Rejected / Do Not Pursue**
| Column | Content |
|--------|---------|
| Property | Full venue name |
| Reason Rejected | Why it was eliminated |
| Date | When it was rejected |

**Formatting rules:**
- Status color codes: Active 🟢 green / Rejected 🔴 red / Closed 🟣 purple
- Freeze the header row
- Bold all headers
- Auto-fit column widths
- Notes column = ALWAYS BLANK

## Part 2: Build the PowerPoint Proposal Deck

**Slide 1: Title Slide**
- Event name, Date range
- Hero photo of top venue
- "Prepared for [Client Name] — [Date]"

**Slide 2: The Brief**
- Host criteria summary (3-4 bullets)
- Dealbreakers listed
- Budget parameters
- Attendee count

**Slides 3–11: Top 3 Proposals (3 slides each)**
For each venue:
- Property name + location
- Hero photo
- "Why this property fits" (2-3 bullets)
- Estimated cost breakdown
- Kosher dining solution

**Slide 12: Side-by-Side Comparison Table**

**Slide 13: Next Steps**
- Recommended option bolded
- Decision needed by date
- Deposit timeline
