# FixHostel — Information Architecture & Flows

**Linked to:** `03_Goals_and_Features.md`, `04_Personas_Stories_Scenarios.md`  
**Purpose:** decide screen structure and how people move through the main tasks before we sketch / wireframe

---

## 1. Information architecture (what sits where)

FixHostel is role-based. After login (or role select for the prototype), each person lands on a home that matches their job. We are not building one mega-app screen for everyone.

### High-level map

```text
FixHostel
│
├── Auth / Role entry (prototype: pick Resident | Warden | Staff)
│
├── RESIDENT
│   ├── Home
│   ├── Report Issue
│   ├── My Requests
│   │   └── Request Detail (timeline + status)
│   ├── Notifications
│   └── Profile
│
├── WARDEN
│   ├── Dashboard / Open Queue
│   ├── Ticket Detail
│   │   └── Assign Technician
│   ├── Filters (urgency / block / status)  ← on queue, not a separate app section
│   ├── Simple Summary (optional Should-have)
│   ├── Notifications
│   └── Profile
│
└── TECHNICIAN (Staff)
    ├── Today's Jobs
    ├── Job Detail
    │   └── Update Status
    ├── Notifications
    └── Profile
```

### Content types (what a “ticket” holds)

Every maintenance request stores roughly:

- Request ID  
- Category (Electrical / Plumbing / Carpentry / Housekeeping / Other)  
- Location (Block + Room **or** Common area label)  
- Description  
- Photo(s)  
- Urgency (Low / Medium / High)  
- Status (Submitted → Assigned → In progress → Resolved)  
- Reporter  
- Assignee (technician)  
- Timestamps + short timeline events  
- Optional rating after resolve  

That object is shared across roles; only the **views** change.

---

## 2. Navigation (per role)

Keeping nav shallow so sketches stay clean.

| Role | Bottom / main nav | Notes |
|------|-------------------|--------|
| Resident | Home · Report · My Requests · Profile | Notifications as bell on Home / top bar |
| Warden | Queue · Summary* · Profile | *Summary only if we include Should-have |
| Technician | Jobs · Profile | Job detail opened from list; notifications as bell |

No hamburger menu full of stuff for v1 — wardens and staff don’t need it.

---

## 3. Flow mapping (who uses which screens)

| Screen | Aarav | Sneha | Ramesh |
|--------|:-----:|:-----:|:------:|
| Report Issue | ● | | |
| My Requests / Request Detail | ● | | |
| Warden Queue | | ● | |
| Ticket Detail + Assign | | ● | |
| Today's Jobs | | | ● |
| Job Detail + Update Status | | | ● |
| Notifications | ● | ● | ● |
| Profile | ● | ● | ● |

● = primary use in our scenarios

---

## 4. User flows

### Flow A — Report → Assign → Resolve → Rate  
*(main flow = Scenario A from personas doc)*

```text
[Aarav] Home
   → Report Issue
      → fill category / location / description / photo / urgency
      → Submit
   → My Requests (status: Submitted)
      → Request Detail (timeline starts)

[Sneha] Queue (sees new High ticket)
   → Ticket Detail
      → Assign Technician (pick Ramesh)
      → Confirm
   → Ticket status: Assigned
   → (Aarav notified)

[Ramesh] Today's Jobs
   → Job Detail
      → Start → In progress
      → Mark Resolved
   → (Aarav + Sneha notified)

[Aarav] Request Detail (Resolved)
   → Rate / short feedback
   → Done
```

**Status path:**  
`Submitted → Assigned → In progress → Resolved`  
(+ optional `Closed` after rating, if we want to show it; not required)

---

### Flow B — Common area report (Scenario B)

```text
[Resident] Home
   → Report Issue
      → Category + location type: Common area
      → label e.g. "Block A – 2nd floor corridor"
      → urgency Medium → Submit
   → My Requests

[Warden] Queue → Assign → [Technician] resolve
   (same backend path as Flow A)
```

Difference is mostly on the **Report** form (location type), not a separate app.

---

### Flow C — Warden triage on a busy day (Scenario C)

```text
[Sneha] Queue
   → Filter: Urgency = High, Status = Open
   → Open ticket 1 → Assign
   → Open ticket 2 → Assign
   → Switch filter: Urgency = Medium
   → Continue assigning
   → (ignore Resolved / already Assigned unless needed)
```

This flow is why filters live **on the queue**, not buried in settings.

---

## 5. Flow diagram (main task — text form for drawing)

Use this when someone draws in FigJam / Figma / paper:

```text
                    ┌─────────────┐
                    │ Resident    │
                    │ reports     │
                    └──────┬──────┘
                           │
                           v
                    ┌─────────────┐
                    │ Submitted   │
                    └──────┬──────┘
                           │
                           v
                    ┌─────────────┐
              ┌─────│ Warden      │
              │     │ reviews     │
              │     └──────┬──────┘
              │            │ assign
              │            v
              │     ┌─────────────┐
              │     │ Assigned    │──────► notify resident
              │     └──────┬──────┘
              │            │
              │            v
              │     ┌─────────────┐
              │     │ Technician  │
              │     │ starts job  │
              │     └──────┬──────┘
              │            │
              │            v
              │     ┌─────────────┐
              │     │ In progress │──────► notify (optional)
              │     └──────┬──────┘
              │            │
              │            v
              │     ┌─────────────┐
              └────►│ Resolved    │──────► notify resident
                    └──────┬──────┘
                           │
                           v
                    ┌─────────────┐
                    │ Rating      │
                    │ (resident)  │
                    └─────────────┘
```

---

## 6. Screen inventory (what to sketch first)

Priority order for paper → wireframes:

1. Resident Home  
2. Report Issue  
3. My Requests  
4. Request Detail (timeline)  
5. Warden Queue  
6. Ticket Detail + Assign sheet/screen  
7. Technician Today's Jobs  
8. Job Detail + status actions  
9. Notification examples (can be simple overlays)  
10. Profile (minimal — name, role, logout)

Skip fancy empty states / settings until hi-fi if short on time.

---

## 7. IA decisions (so we don’t argue later)

- **One ticket model**, three role views — don’t invent separate “complaint” vs “job” objects in the UI copy; same request, different words if needed (“My request” vs “Job”).  
- **Report is a primary action** for residents (easy to reach from Home).  
- **No public feed** of everyone’s issues (privacy came up in research).  
- **Filters on queue**, not a separate “Search app”.  
- **Status is always visible** on list cards + detail timeline (visibility of system status).

---

## 8. Next steps for the team

1. Draw this IA as a simple sitemap on paper / FigJam.  
2. Sketch the 8–10 screens above (low-fi).  
3. Convert sketches → wireframes → wireflow for **Flow A**.  

Optional doc later: `06_Sketch_Wireframe_Notes.md` (screen-by-screen notes for whoever is in Figma). Say if you want that next.
