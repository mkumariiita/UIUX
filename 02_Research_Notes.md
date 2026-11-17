# FixHostel — Research Notes

**Linked to:** `01_Problem_Context_Scope.md`  
**Method mix:** short conversations with people around us + looking at how similar apps handle requests  
**When:** early–mid Nov 2026 (around campus / hostel)

---

## 1. What we actually did

We didn’t run a huge formal study. For this unit we kept it practical:

1. **Talked to 6 hostel residents** (different blocks / years) — mostly 8–12 min chats, some over tea, some in the corridor after dinner.
2. **One longer chat with hostel office side** — caretaker / person who usually gets pulled into repair complaints (not a full “expert interview”, but useful).
3. **Quick look at existing patterns** — apartment maintenance / complaint apps and how colleges usually handle tickets (WhatsApp groups, Google Forms, registers). We noted what felt relevant for hostel life, not for big societies.

Questions we kept repeating (roughly):

- How do you report something broken right now?
- What usually goes wrong after you report?
- How long before you hear back?
- Would you bother uploading a photo / marking urgency?
- What would make you trust that someone actually saw your request?

---

## 2. People we spoke to (anonymised)

| Code | Who | Notes |
|------|-----|--------|
| R1 | 2nd year, Block C | Fan not working for a week; messaged floor group twice |
| R2 | 3rd year, Block A | Bathroom leak; caretaker came once, issue returned |
| R3 | 1st year | Didn’t know who to contact; asked roommate |
| R4 | Girl’s hostel resident | Prefers not putting personal room details in big groups |
| R5 | Final year | Only reports “serious” things; ignores small issues now |
| R6 | PG-style accommodation nearby | Uses landlord WhatsApp; same “seen but no update” problem |
| S1 | Hostel staff / caretaker side | Gets flooded with messages; hard to remember what was already told to electrician |

Names aren’t listed on purpose — for class submission this is enough, and people were more honest that way.

---

## 3. What kept coming up

### From residents

- **Chat is easy to start, bad to track.** “Ok” in WhatsApp doesn’t mean assigned or fixed.
- **No status = anxiety / nagging.** People follow up because silence feels like being ignored.
- **Urgency is fuzzy.** A leak and a loose shelf land in the same group chat with the same energy.
- **Details get lost.** Room number wrong, no photo, “AC not cooling” with zero extra info → technician shows up unprepared.
- **First-years are confused.** They don’t know the “unwritten” process (who to ping, what to expect).
- **Privacy / noise.** Not everyone wants to post room problems in a 80-person group.

### From staff side (S1)

- Messages come from everywhere — personal chat, group, in person while walking.
- Hard to know what’s still open vs already fixed.
- Technicians ask for photos/location; staff ends up being the middleman on calls.
- Peak days (rain, power cut) are chaos; priority is mental, not written down.

### From looking at other apps / patterns

- Status timeline (Submitted → Assigned → In progress → Done) is the thing users understand fastest.
- Photo + category + location is a common “minimum useful” report form — long forms get abandoned.
- Role-based views matter: resident doesn’t need the full admin queue; technician doesn’t need analytics.

---

## 4. Quotes we wrote down (paraphrased close to what was said)

> “I messaged three times. Still don’t know if anyone saw it.” — R1

> “If it shows assigned, I’ll wait. If it shows nothing, I’ll keep asking.” — R2

> “Don’t make me fill 15 fields. Room, problem, photo is enough.” — R5

> “Groups are noisy. I only put something if it’s really bad.” — R4

> “I need one list, not forty chats.” — S1 (roughly how they put it)

---

## 5. Insights → what this means for FixHostel

| Insight | Design direction |
|---------|------------------|
| Requests get lost across channels | One place to log + own a request ID |
| Silence causes follow-ups | Visible status + notifications on change |
| Urgent vs minor looks the same today | Urgency + simple priority on warden queue |
| Incomplete reports waste visits | Photo + category + block/room on report form |
| Different people need different screens | Resident / Warden / Technician roles |
| Staff overloaded on peak days | Filters (urgency, block, open only) |
| Not everyone likes public groups | Private reporting, not a public feed |

---

## 6. Research limits (being honest)

- Sample is small and mostly our own campus circle — not a city-wide study.
- We didn’t interview a full-time electrician end-to-end; technician needs are partly inferred from S1 + resident stories.
- Secondary research was light (pattern scan, not a formal competitor matrix).

That’s fine for Unit 4 if we stay clear about it and still ground personas / features in what we heard.

---

## 7. Next document

`03_Goals_and_Features.md` — user goals, business/hostel goals, and the feature list we’ll design for.
