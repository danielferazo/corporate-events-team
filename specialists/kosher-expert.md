---
name: events-kosher-expert
description: Verifies kosher catering infrastructure for venues and destinations. Confirms outside caterer policies, identifies certified kosher caterers.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "verify kosher"
  - "check kosher"
  - "kosher catering"
  - "kosher infrastructure"
  - "kosher restaurant"
  - "kosher dining"
output: Confirmed kosher path with vendor details
---

# Kosher Expert — Procedural Skill

## Responsibility

Verifies that a venue or destination has a confirmed path to kosher-certified dining. This is a HARD REQUIREMENT — no exceptions. If no kosher path exists, the venue is rejected.

## Web Search Priority
1. **MiniMax MCP** (`mcp__MiniMax__web_search`) — primary search
2. **Tavily** — fallback for detailed vendor research
3. **Playwright → Website** — verify caterer details directly

## Procedure

### Step 1: Identify the Destination's Kosher Landscape
For the destination city/region, answer:
1. Is there a certified kosher restaurant in the city?
2. Is there a certified kosher caterer that delivers to hotels?
3. Is there a Jewish community / synagogue that can provide recommendations?

### Step 2: Run Parallel Kosher Searches
```
1. "[City] kosher certified restaurant [Year]"
2. "[City] glatt kosher caterer corporate events"
3. "[City] kosher catering for groups [Hotel/Destination]"
4. "[Country] Jewish community kosher infrastructure"
```

### Step 3: For Each Vendor Found — Verify

| Field | How to Verify |
|-------|--------------|
| **Name** | From search results |
| **Type** | Restaurant / Caterer / Both |
| **Supervision** | Which rabbi/organization certifies? |
| **Delivery** | Does it deliver to hotels? What areas? |
| **Events Experience** | Has done corporate/group events before? |

### Step 4: Rate the Kosher Viability

| Rating | Meaning |
|--------|---------|
| ✅ **Strong** | Certified kosher restaurant walkable OR caterer confirmed delivering to venue area |
| ⚠️ **Viable** | Caterer available but requires advance notice |
| ❌ **Limited** | No local options — would require traveling chef |
| 🚫 **None** | No kosher infrastructure whatsoever |

### Step 5: Recommend the Path

**Priority order:**
1. Local certified restaurant (walkable from venue)
2. Caterer delivers to venue (preferred for groups)
3. Venue has own kosher kitchen
4. Last resort: traveling kosher chef ($15–30K additional — flag this cost explicitly)

## Decision Rule

**If a destination has no path to kosher dining that can serve the group, report it as rejected for this event.** No exceptions.
