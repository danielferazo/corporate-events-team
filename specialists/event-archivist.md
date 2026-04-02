---
name: events-archivist
description: Logs completed events to event-log.md. Archives all artifacts created. Maintains institutional memory for the events team.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "log event"
  - "archive event"
  - "event complete"
  - "close out event"
output: Updated event-log.md entry
---

# Event Archivist — Procedural Skill

## Responsibility

Logs completed events to event-log.md. Archives all artifacts created. Maintains institutional memory.

## Procedure

### Step 1: Gather Event Data
Collect from the event brief and tracker:
- Event name
- Actual dates (vs. planned)
- Final venue
- Attendance (planned vs. actual)
- Budget (estimated vs. actual)
- All artifacts created (file paths)
- Key notes from the event

### Step 2: Write the Archive Entry

Add to `references/event-log.md` under `## COMPLETED`:

```markdown
### [Event Name] — [Date]

| Field | Value |
|-------|-------|
| **Event** | Full event name |
| **Date** | Actual date(s) |
| **Venue** | Final venue name + address |
| **Attendance** | Planned vs Actual |
| **Budget** | Estimated vs Actual |
| **Planner** | [Name] |

**Venue Rating:** ⭐⭐⭐⭐⭐ (1–5) | **Use Again?** Yes / No / Maybe

**What worked:**
- [bullet]

**What didn't:**
- [bullet]

**Learnings for next time:**
- [bullet]

**Artifacts:**
- [file name + location]
```

### Step 3: Archive All Artifacts
For each artifact created:
- Confirm the file exists in the output folder
- Link to it in the archive entry

### Step 4: Update the Event Brief
If the event had a dedicated brief file:
- Add actual outcomes to the brief
- Note what changed from the original plan

### Step 5: Clean Up Active Events
Remove from the Active Events table or move to Completed.

## Self-Improvement Log

After archiving, add to `learnings/BACKLOG.md`:
```markdown
### [YYYY-MM-DD] [Event Name] — [Learning Type]
- **Insight:** [what was learned]
- **Affected Skills:** [specialist(s)]
- **Suggested Improvement:** [what should change]
```
