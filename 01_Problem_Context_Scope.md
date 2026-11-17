# FixHostel — Problem, Context & Scope

**Subject:** Interaction Design and UI/UX (Unit 4)  
**App idea:** Hostel & Property Maintenance  
**Working title:** FixHostel  
**Date:** Nov 2026

---

## 1. What we noticed (starting point)

In our hostel, when something breaks — fan, bathroom leak, lights in the corridor — people usually do one of these:

- message the warden on WhatsApp
- put it in the floor group chat
- tell the caretaker in person
- sometimes write it in a register near the office (if anyone remembers)

It kind of works for small things, but a lot of requests just… disappear. Someone says “ok noted”, then nothing for days. You don't know if it's assigned, if the electrician came and left, or if they forgot. So people keep following up, or they stop reporting small issues altogether.

We spoke informally with a few residents and one person from the hostel staff side (details in the research notes). The same complaints kept coming up: no tracking, no clear priority, and too much back-and-forth on chat.

---

## 2. Problem statement

Hostel residents and staff currently manage maintenance through scattered channels (WhatsApp, verbal complaints, paper registers). Because there is no single place to log, prioritise and track requests, issues get delayed or lost, urgent problems are not clearly separated from minor ones, and residents have no visibility on progress. This creates repeated follow-ups for students and extra coordination load for the warden and technicians.

**In one line:**  
Maintenance requests in hostels get lost between chats and verbal updates — FixHostel gives one place to report, assign and track them.

---

## 3. Target users

| Role | Who | Why they matter |
|------|-----|-----------------|
| Primary | Hostel residents (students) | They face the problem daily and will use the app most |
| Secondary | Warden / floor in-charge | They decide priority and assign work |
| Supporting | Maintenance staff (electrician, plumber, carpenter, housekeeping) | They close the loop by doing the actual work |

We are designing mainly around **college hostel** life first. The same idea can later stretch to PG / small property maintenance, but that is not the focus for this submission.

---

## 4. Context

- Shared rooms and common areas (washrooms, corridors, water coolers, etc.)
- Limited on-site staff; technicians are often shared across blocks
- Peak complaint times: mornings, evenings, right after rain / power cuts
- Most students are comfortable with mobile apps; staff prefer simple screens, not long forms
- Communication today is almost entirely WhatsApp + in-person

This is not a “facility management ERP”. It's a lightweight request + tracking tool that fits how hostels already operate.

---

## 5. Scope

### In scope (what FixHostel will cover)

- Report a maintenance issue (category, location/room-block, short description, optional photo, urgency)
- View “My Requests” and a basic status timeline
- Warden view: open queue, filter by urgency / block / status, assign to staff
- Technician view: today's jobs, open job detail, update status (assigned → in progress → resolved)
- Simple notifications when status changes
- After resolve: quick feedback / rating from the resident
- Basic request history

### Out of scope (intentionally not building this)

- Hostel fee / rent payments
- Mess menu, laundry booking, room allotment
- Full inventory / stock management for spare parts
- Multi-campus admin dashboards with heavy analytics
- Live chat with technicians inside the app

If something is out of scope, we still may mention it as a “future idea” in the presentation, but it won't be in personas, user stories or wireframes for Unit 4.

---

## 6. Success (how we'll know the design is useful)

For residents: “I reported it once and I can see what's happening.”  
For warden: “I have one list instead of 40 chat threads.”  
For technicians: “I know the room, the problem, and can mark it done without calling around.”

---

## 7. Next document

`02_Research_Notes.md` — how we looked into the problem (conversations + secondary notes) and what we took away for features.
