# FixHostel — Goals & Features

**Linked to:** `01_Problem_Context_Scope.md`, `02_Research_Notes.md`  
**Purpose:** spell out what users want, what the hostel side wants, and which features we will actually design

---

## 1. User goals

### Residents (students)

- Report a problem quickly without hunting for the right WhatsApp number
- Know that the request was received (not just “ok” in a chat)
- See progress — assigned / in progress / done — without nagging
- Give enough detail (photo, room, type) so the visit is not wasted
- For urgent things (leak, no power, safety), get it treated differently from small issues

### Warden / floor in-charge

- See all open requests in one place instead of scattered chats
- Sort or filter by urgency, block, and status
- Assign the right person and know who owns the ticket
- Reduce repeat “any update?” messages from residents

### Maintenance staff (technician / caretaker doing the work)

- Open today’s jobs with clear room / block / problem / photo
- Update status in a few taps (start work → mark resolved)
- Avoid long calls just to collect basic details

---

## 2. Business / institutional goals

(Here “business” = hostel administration / institution, not a startup pitch.)

- Cut lost or forgotten complaints
- Bring down average time from report → assign → resolve
- Make ownership clear (who is responsible for this ticket)
- Keep a simple history if someone asks “what happened to that complaint?”
- Improve resident trust that reporting is worth it
- Give wardens a calmer peak-day workflow (rain, power cuts, etc.)

If FixHostel works, the hostel doesn’t need a heavy ERP — just fewer missed requests and less coordination noise.

---

## 3. How goals connect (short)

| If this user goal is met… | …it also helps the hostel because… |
|---------------------------|-------------------------------------|
| Resident can track status | Fewer follow-up messages / escalations |
| Warden can triage urgency | Serious issues get attention first |
| Technician gets full job info | Fewer failed visits, faster closure |
| Feedback after resolve | Weak spots in service show up over time |

---

## 4. Feature list

We kept the list tight on purpose. Only things we can show in sketches / wireframes for Unit 4.

### Must have (design these)

| # | Feature | Who mainly uses it | Why (from research) |
|---|---------|--------------------|---------------------|
| 1 | Role-based home (Resident / Warden / Staff) | All | Different jobs need different first screens |
| 2 | Report issue (category, block/room, description, photo, urgency) | Resident | Incomplete reports waste visits; photo helps |
| 3 | My Requests + status timeline | Resident | Silence was the biggest pain |
| 4 | Notifications on status change | Resident (+ others) | Stops blind follow-ups |
| 5 | Warden queue (open tickets, filters) | Warden | “One list, not forty chats” |
| 6 | Assign technician to a ticket | Warden | Clear ownership |
| 7 | Technician job list + job detail | Staff | Know what to do today |
| 8 | Update status (Assigned → In progress → Resolved) | Staff | Closes the loop |
| 9 | Quick rating / feedback after resolve | Resident | Light quality signal |

### Should have (include if time; nice in hi-fi)

| # | Feature | Notes |
|---|---------|--------|
| 10 | Common-area reporting (corridor, washroom, cooler) | Same form, location = common area |
| 11 | Emergency / high-urgency flag in UI | Visual push on warden queue |
| 12 | Search + filter on history | “What did I raise last month?” |
| 13 | Simple warden summary (open vs closed this week) | One small stats strip, not a full analytics module |

### Could have / later (not in main wireflows)

- Auto-assign rules by category
- Multi-language UI
- Offline draft of a report
- Spare-parts / inventory
- Chat with technician inside the app

---

## 5. Feature priorities for design work

**First wireflow to design end-to-end:**  
Report → Warden assigns → Technician resolves → Resident sees update + rates  

That one path covers almost every Must-have feature. Secondary screens (history filters, summary strip) can stay simpler.

---

## 6. What we are not calling “features” yet

Out of scope stays out of scope (fees, mess, laundry, room allotment).  
Those may come up in brainstorming, but they are not part of FixHostel for this assignment.

---

## 7. Next document

`04_Personas_Stories_Scenarios.md` — 3 personas, user stories for major features, and 2–3 scenarios we will use for flows and the video.
