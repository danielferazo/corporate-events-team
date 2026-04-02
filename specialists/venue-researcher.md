---
name: events-venue-researcher
description: Researches and evaluates venues matching event criteria. Finds 8-15 properties per search, verifies capacity, checks policies, rates against criteria.
version: "1.0"
status: active
domain: operations
model: sonnet
type: specialist
triggers:
  - "find venues"
  - "research venues"
  - "venue search"
  - "search venues"
output: Structured venue list with full profiles
---

# Venue Researcher — Procedural Skill

## Responsibility

Finds and researches venues matching host criteria. Produces 8–15 properties with full profiles: name, address, phone, email, website, capacity, pricing, vibe, and outside-catering status.

## Web Search Priority
1. **MiniMax MCP** (`mcp__MiniMax__web_search`) — primary search
2. **Tavily** — fallback when MiniMax fails
3. **Playwright → Google** — last resort for verification

## Procedure

### Step 1: Gather Criteria
From the event brief, extract:
- Location / city
- Event type (corporate social, executive retreat, dinner, etc.)
- Guest count
- Budget per person (or total)
- Host's vibe/aesthetic criteria (from host profile)
- Hard dealbreakers

### Step 2: Run Parallel Research Searches

```
1. "[City] luxury boutique hotels [Event Type] private events [Year]"
2. "[City] waterfront resort group booking [Guest Count] executives"
3. "[City] hotels with private dining rooms corporate events"
4. "[City] [Boutique/Unique] hotels executive retreats"
```

### Step 3: For Each Venue Found — Build Profile

| Field | How to Find |
|-------|------------|
| **Name** | From search results |
| **Location** | From website / Google Maps |
| **Phone** | From website |
| **Email** | From website (info@ or events@) |
| **Website** | From search results |
| **Capacity** | From website |
| **Pricing** | From search results or direct inquiry |
| **Vibe** | From website photos, reviews — describe in 1-2 sentences |
| **Outside Catering** | Check website for event policies |
| **A/V Equipment** | Check website for meeting facilities |
| **Private Space** | Note if private dining room, buyout, or exclusive-use option |
| **Kosher Compatible** | Flag for kosher-expert to verify |

### Step 4: Apply Dealbreaker Filter

Any venue with a confirmed ❌ on dealbreakers (outside catering not allowed, capacity insufficient) → discard immediately.

### Step 5: Verify Operational Status
Before adding any venue to the final list, verify it is NOT permanently closed:
- Check Google Maps listing
- Check recent reviews (within 12 months)

## Output Format

Present as a structured table:

| # | Property | Location | Type | Est. Cost/Night | Outside Catering | Kosher Path | Vibe Notes | Website |
|---|----------|----------|------|-----------------|-----------------|-------------|------------|---------|

Follow with 2–3 sentence summary of top 3 recommendations and why they fit.
