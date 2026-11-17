# FixHostel — Personas, User Stories & Scenarios

**Linked to:** `01_Problem_Context_Scope.md`, `02_Research_Notes.md`, `03_Goals_and_Features.md`  
**How we built these:** grouped users by role → noted behaviour differences from our chats → wrote three personas that cover the main paths (report, triage, fix)

---

## 1. Grouping users (quick)

Before writing personas we split people into:

**A. People living in the hostel**  
- Regular resident who reports often  
- First-year who doesn’t know the process  
- Someone who only reports when it’s serious  

**B. People running / fixing things**  
- Warden / floor in-charge  
- Technician or caretaker who does the work  

For Unit 4 we turned the strongest patterns into **3 personas** (enough for stories + wireflows without flooding the submission).

---

## 2. Behaviour notes (what differed)

From the research chats, people didn’t only differ by age/year — they differed in:

- how urgently they need a fix  
- whether they trust chat or want a proper status  
- how much detail they give when reporting  
- how much responsibility they carry (self vs whole floor / block)  
- how comfortable they are with an app vs a phone call  

Residents clustered around “I just want it tracked.”  
Warden side clustered around “I need one queue.”  
Staff clustered around “give me location + photo, let me mark done.”

---

## 3. Personas

### Persona 1 — Aarav Mehta (Primary)

| | |
|--|--|
| **Role** | Hostel resident |
| **Age / year** | 20, 2nd year |
| **Block** | Block C, Room 214 |
| **Tech** | Uses phone for everything; fine with apps |
| **Type** | Primary |

**About him**  
Aarav shares a room, keeps odd study hours, and has already wasted a week waiting on a ceiling fan repair. He usually drops a message in the floor group and then forgets until the heat gets annoying again. He doesn’t want to “manage” maintenance — he just wants to raise it once and know someone owns it.

**Goals**
- Report in under a minute  
- See if it’s assigned or stuck  
- Get urgent stuff (leak / power) treated seriously  

**Frustrations**
- “Ok noted” with no follow-through  
- Repeating the same details on call  
- Not knowing who is supposed to come  

**Behaviours**
- Will upload a photo if the form is short  
- Checks notifications more than email  
- Follows up only when status is silent for too long  

**Quote**  
> “Just tell me it’s assigned and when someone is coming.”

---

### Persona 2 — Sneha Iyer (Secondary)

| | |
|--|--|
| **Role** | Hostel warden / floor in-charge |
| **Age** | 34 |
| **Context** | Handles complaints across ~few hundred residents |
| **Tech** | Comfortable with phone; hates messy groups |
| **Type** | Secondary |

**About her**  
Sneha spends a big part of the day sorting requests that arrive as personal messages, group pings, and people stopping her in the corridor. On rainy days or after a power cut, everything feels urgent and she has no clean list of what’s still open. She needs to prioritise and hand work to the right technician without becoming a full-time call centre.

**Goals**
- One open queue she can trust  
- Filter by urgency / block / status  
- Assign ownership clearly  

**Frustrations**
- Same issue reported three times by three people  
- No idea if the electrician already went  
- Residents asking for updates she doesn’t have  

**Behaviours**
- Checks phone in short bursts between other duties  
- Prefers filters and badges over long dashboards  
- Will use the app daily if it reduces chat noise  

**Quote**  
> “I need one list, not forty chat threads.”

---

### Persona 3 — Ramesh Kumar (Supporting)

| | |
|--|--|
| **Role** | Campus maintenance (electrician / plumbing jobs) |
| **Age** | 41 |
| **Context** | Shared across blocks; gets jobs via caretaker / warden |
| **Tech** | Uses smartphone; prefers simple screens, large actions |
| **Type** | Supporting / supplemental |

**About him**  
Ramesh gets pulled into jobs with incomplete information — wrong room, no photo, vague “AC problem”. He wastes time calling back to ask basics. He doesn’t need analytics. He needs today’s list, the location, what to fix, and a way to mark it done so people stop calling him.

**Goals**
- Clear job card (room, problem, photo, urgency)  
- Update status quickly on site  
- Avoid repeat visits for missing info  

**Frustrations**
- Half details, then blame for delay  
- Stacked verbal instructions that get forgotten  
- Residents expecting him to know the ticket history from memory  

**Behaviours**
- Opens jobs in order of urgency when told  
- Takes a quick look at the photo before going upstairs  
- Marks resolved as soon as the work is done (if the UI is easy)  

**Quote**  
> “Give me the room, the problem, and a photo. That’s enough.”

---

## 4. User stories (major features)

Format: *As a … I want … so that …*

### Reporting & tracking (Aarav)

1. As a **resident**, I want to **report an issue with category, room/block, description and photo**, so that **staff understand the problem without calling me**.  
2. As a **resident**, I want to **mark urgency when I report**, so that **serious problems don’t sit behind small ones**.  
3. As a **resident**, I want to **see my request status on a timeline**, so that **I don’t have to keep asking for updates**.  
4. As a **resident**, I want to **get a notification when status changes**, so that **I know when someone is assigned or the work is done**.  
5. As a **resident**, I want to **rate the resolution after it’s closed**, so that **bad fixes don’t stay invisible**.

### Triage & assign (Sneha)

6. As a **warden**, I want to **see all open tickets in one queue**, so that **nothing depends on remembering chat threads**.  
7. As a **warden**, I want to **filter by urgency, block and status**, so that **I can triage on busy days**.  
8. As a **warden**, I want to **assign a technician to a ticket**, so that **ownership is clear**.  

### Execute & close (Ramesh)

9. As a **technician**, I want to **see today’s assigned jobs with location and photo**, so that **I can go prepared**.  
10. As a **technician**, I want to **update status to in progress / resolved**, so that **the resident and warden stay informed without calling me**.

### Common area (stretch story if we show it)

11. As a **resident**, I want to **report a common-area issue (corridor / washroom)**, so that **shared problems also get logged and owned**.

---

## 5. Scenarios

These are the stories we will use for flow diagrams, wireflows and (later) the video. Written as short narratives so the journey feels real, not just a checklist.

---

### Scenario A — Happy path: water leakage (main scenario)

**Personas:** Aarav Mehta → Sneha Iyer → Ramesh Kumar  
**Why this scenario:** covers almost every Must-have feature in one run.

It was a little after 9 on a weekday morning when Aarav noticed a dark patch spreading under the washbasin in Room 214. At first he thought it was just water from brushing, but when he touched the pipe joint it was wet again within a minute. His roommate groaned — last time something like this happened, they had messaged the floor group, got three “ok” replies, and then waited four days.

This time Aarav opened **FixHostel**. On Home he tapped **Report an issue**. He chose **Plumbing**, typed Block C and Room 214, wrote a short line — “Leak near washbasin joint, water pooling on floor” — set urgency to **High**, and clicked a quick photo of the wet pipe. Submit. No hunting for the caretaker’s number. No posting in a noisy group.

Almost immediately, **My Requests** showed the ticket as **Submitted**, with a small timeline starting at the top. Aarav felt that quiet relief of “at least it’s logged.” He put his phone down and went to class.

Across campus, Sneha was already in her mid-morning sweep of the **Open Queue**. A new High-urgency card sat near the top: washbasin leak, Block C 214, photo attached. She opened it, skimmed the description, and tapped **Assign technician**. Ramesh’s name was in the list for plumbing/electrical jobs. She confirmed. The ticket moved to **Assigned**.

Aarav’s phone buzzed between lectures: *Your request was assigned to Ramesh.* He didn’t need to ping anyone. That alone was different from WhatsApp.

Ramesh checked **Today’s Jobs** after lunch. The leak card showed room, urgency, and the photo — enough to know he’d need basic plumbing tools, not a blind visit. He walked to Block C, opened **Job Detail**, tapped **Start work** (**In progress**), tightened and resealed the joint, wiped the floor, then marked **Resolved**.

By evening Aarav was back in the room. The floor was dry. FixHostel showed **Resolved** on the timeline. He left a quick 4-star rating and a one-line note: “Came same day, fixed properly.” For once, the whole loop — report, assign, fix, feedback — had happened without a single “any update?” message.

**Status path in this story:** Submitted → Assigned → In progress → Resolved → Rated

---

### Scenario B — First-year confusion: dark corridor (common area)

**Persona:** Priya Nair (first-year resident; same goals as Aarav, less hostel knowledge)  
**Supporting:** Sneha (warden), technician/electrician  
**Why this scenario:** shows the app replacing “unwritten process” knowledge that seniors usually gatekeep.

Priya had only been in hostel for three weeks. Block A still felt like a maze. Around 8:30 pm she walked back from the mess and noticed the tube light outside the 2nd floor corridor was dead. The stretch near the stairs was properly dark. She hesitated at her door. Who do you even tell? In the induction they had mentioned “contact the caretaker,” but she didn’t have the number saved. Her roommate, already half asleep, mumbled, “Just put it in the floor group,” and turned over.

Priya opened the group, stared at it, and closed it again. She didn’t want to look stupid asking basic questions in front of fifty people. She also didn’t want her room number floating in a public chat for a corridor light.

She remembered seniors talking about **FixHostel** during a floor meeting. She opened the app, chose **Report an issue**, set category to **Electrical**, switched location to **Common area**, and typed “Block A – 2nd floor corridor, tube light near stairs.” Urgency **Medium** — not a flood, but unsafe at night. She skipped overthinking the form, attached no photo (too dark to capture well), and submitted.

**My Requests** showed **Submitted**. That was enough for her to sleep without asking three different people what the “proper” process was.

Next morning Sneha saw the common-area ticket in the queue, assigned an electrician from the staff list, and moved on. Priya got the **Assigned** notification while sitting in class. By evening the corridor light was on again; the ticket showed **Resolved**. She never had to learn which WhatsApp number mattered, or who “usually handles lights.” The app carried the process she didn’t know yet.

**What this story highlights:** common-area reporting, low-confidence first-year user, private reporting instead of public groups, status without senior gatekeeping.

---

### Scenario C — Busy day triage: after the rain (warden stress)

**Persona:** Sneha Iyer (focus), with residents and technicians in the background  
**Why this scenario:** justifies filters, urgency marking, and a single queue — strong for viva / video UX explanation.

The rain started before dawn and didn’t seriously stop until mid-morning. By 11 am Sneha’s personal WhatsApp would normally be unusable — leaks, “water cooler dead,” “socket sparking,” people stopping her in the corridor with wet shoes and half-stories. Today those same problems were landing in **FixHostel** instead of twenty parallel chats.

When she opened the **Open Queue**, the count badge already said more than a dozen open tickets. She didn’t try to read them top to bottom. She set the filter to **Urgency = High** and **Status = Open**.

What remained was the dangerous stuff first: two room leaks, one report of a loose bathroom wire, a water seepage complaint near the Block B stairs. One by one she opened each card, checked the photo if there was one, and **assigned** the right technician. High tickets left her list as **Assigned**. She could feel the difference — she wasn’t holding the whole backlog in her head.

Then she switched the filter to **Medium**. Cooler not cooling, stuck window latch, flickering balcony light. Important, but not “drop everything.” She assigned what she could, left two for after lunch when another staff member would be free.

A few residents still almost messaged her personally out of habit. She replied once with “Check FixHostel status — it’s assigned.” After that, most stopped. On their side they could already see **Assigned** or **In progress**. The queue stayed usable because she wasn’t staring at Resolved tickets mixed into the same pile; those were filtered out.

By late afternoon the High list was empty. Medium was thinner. The rain had created the same chaos as always — but the work had an order, ownership, and a place to look. Sneha closed the app for a tea break without that usual feeling of “I’m forgetting someone.”

**What this story highlights:** peak load, urgency filters, assign-as-triage, status reducing follow-up spam, queue designed for ops not for scrolling chats.

---

## 6. What we’ll draw next

From Scenario A we need:

- Resident: Home, Report, My Requests, Request detail  
- Warden: Queue, Ticket detail + Assign  
- Technician: Job list, Job detail + status actions  

IA + flow diagrams come in the next file.

---

## 7. Next document

`05_IA_and_Flows.md` — information architecture (screen map) + flow diagrams / flow mapping for the main scenarios.
