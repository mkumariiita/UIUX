# FixHostel — Persona Development (Design Thinking)

**Subject:** Interaction Design and UI/UX (Unit 4)  
**App:** FixHostel — Hostel & Property Maintenance  
**Based on process structure from:** class Personas IDU method  
**Date:** Nov 2026

---

# Overview & Process

## Objective

To understand different hostel maintenance users through their behaviours, goals, motivations, needs, frustrations, skills, activities, and environmental context before designing the FixHostel experience.

## Design Thinking Process Flow

1. Research / Observation
2. Group Users
3. Behavioral Variables
4. Behavior Mapping
5. Behavior Patterns
6. Goals & Characteristics
7. Persona Type
8. Persona Narrative
9. Final Persona

## Deliverable

Five developed personas grounded in observed hostel behaviours, mapped to significant patterns and typed by role (**Primary**, **Secondary**, **Supplemental**).

---

# Step 1: Group Users by Role

## A. Hostel Residents

*People living in the hostel who raise or live with maintenance issues.*

- Frequent reporter (raises issues often, expects status)
- First-year / process-confused resident
- Urgent-only reporter (only reports serious problems)
- Common-area reporter (corridor, washroom, cooler)
- Privacy-conscious resident (avoids big WhatsApp groups)

## B. Hostel Workforce

*People coordinating and fixing maintenance.*

- Warden / floor in-charge
- Technician (electrician / plumber / carpenter)
- Caretaker (middleman between residents and technicians)

## Observation

These users differ not only by year or job title, but mainly in **responsibility**, **urgency**, **need for status**, **detail-giving**, **digital comfort**, **privacy comfort**, and **decision load**.

---

# Step 2: Behavioral Variables

## Ten scales to characterise user behaviour

1. **Digital dependence:** Low → High
2. **Independence:** Low → High
3. **Need for human assistance:** Low → High
4. **Urgency of needs:** Low → High
5. **On-site mobility / access:** Restricted → Unrestricted
6. **Information preference:** Human / chat → In-app digital
7. **Decision-making:** Needs guidance → Independent
8. **Frequency of maintenance interaction:** Low → High
9. **Responsibility:** Self / room → Many people / block
10. **Stress / cognitive load:** Low → High

## How to use these scales

Each user type is placed on every scale based on observed behaviour (hostel chats + staff conversation). Users who cluster on multiple scales reveal significant behaviour patterns (Step 4).

---

# Step 3: Behavior Mapping

Users mapped against the 10 behavioural variables.

| User type | Digital dep. | Independence | Human assist. | Urgency | Mobility | Info pref. | Decision | Frequency | Responsibility | Stress |
|-----------|--------------|--------------|---------------|---------|----------|------------|----------|-----------|----------------|--------|
| Frequent reporter | High | High | Low | Med–High | Unrestricted | Digital | Independent | High | Self/room | Med |
| First-year confused | High | Med | High | Med | Unrestricted | Mixed | Needs guidance | Low | Self | High |
| Urgent-only reporter | High | High | Low | High (when reports) | Unrestricted | Digital | Independent | Low | Self | Med |
| Common-area reporter | High | Med | Med | Med | Unrestricted | Digital | Independent | Med | Floor/shared | Med |
| Privacy-conscious | High | High | Low | Med | Unrestricted | Digital (private) | Independent | Med | Self | Med |
| Warden | High | High | Low | High | Unrestricted | Digital | Independent | High | Many | High |
| Technician | Med–High | High | Low | High on job | Unrestricted | Mixed→Digital | Independent | High | Many jobs | Med–High |
| Caretaker | Med | Med | Med | High | Unrestricted | Human/chat | Mixed | High | Many | High |

---

# Step 4: Significant Behavior Patterns

## Five clusters that reveal how users actually behave

### Pattern 1: Status-seeking self-serve residents

**Users:** Frequent reporter, Privacy-conscious, Urgent-only (when they do report)  
**Characteristics:**

- Want to report once and move on  
- Hate silence after “ok noted”  
- Prefer private app over public groups  
- Will add photo if the form is short

### Pattern 2: Process-confused newcomers

**Users:** First-year confused  
**Characteristics:**

- Don’t know who to contact  
- Hesitate to post in big groups  
- Need guided, obvious next steps  
- High stress from not knowing the “unwritten process”

### Pattern 3: Shared-space reporters

**Users:** Common-area reporter  
**Characteristics:**

- Problem is not only “my room”  
- Ownership of the issue feels unclear  
- Want someone officially responsible  
- Location needs a label, not only room number

### Pattern 4: High operational responsibility (warden / caretaker)

**Users:** Warden, Caretaker  
**Characteristics:**

- Coordinate many people  
- Peak-day overload (rain, power cut)  
- Need one queue, filters, clear assign  
- Stressed by scattered WhatsApp threads

### Pattern 5: Field execution under incomplete info

**Users:** Technician  
**Characteristics:**

- Needs room + problem + photo  
- Prefers large simple actions  
- Wastes time on vague tickets  
- Marks done fast if UI is easy

---

# Step 5: Behavior → Attitude → Goal

Synthesise characteristics and define goals.

| Pattern | Behavior | Attitude | Goal |
|---------|----------|----------|------|
| 1 Status-seeking | Reports in app, checks timeline/notifications | Impatient with silence, practical | Know it’s owned and progressing |
| 2 Process-confused | Avoids groups, looks for a clear path | Uncertain, careful, doesn’t want to look lost | Raise issue without asking seniors |
| 3 Shared-space | Reports corridor/washroom/cooler | Slightly detached but responsible | Get shared problems officially logged |
| 4 Operational | Triages queue, assigns staff | Efficient, overloaded, decisive | Keep one list and clear ownership |
| 5 Field execution | Opens job card, updates status on site | Task-focused, low patience for fluff | Fix prepared, mark done, move next |

---

# Step 6: Completeness Check

## Coverage checklist

- [x] Fast private reporting for residents  
- [x] Status visibility / notifications  
- [x] Urgency triage for serious issues  
- [x] Photo + location detail for fewer wasted visits  
- [x] Common-area reporting  
- [x] First-year / process-confused support  
- [x] Warden queue + assign workflow  
- [x] Technician job clarity + status update  
- [x] Peak-load / rainy-day coordination  
- [x] Feedback after resolve  

## Redundancy review

Each persona was reviewed against the others. No two personas share the same combination of **behaviour pattern + role**, so no duplication remains.

---

# Step 7: Persona Type Analysis

Classifying each persona by design importance.

| Persona | Type | Reason |
|---------|------|--------|
| Aarav Mehta (Frequent resident reporter) | **Primary** | Represents the majority resident use case; drives report + track core experience |
| Sneha Iyer (Warden) | **Primary** | Operational decision-maker; queue/assign must work for her or the system fails |
| Ramesh Kumar (Technician) | **Secondary** | Closes the loop; shapes job-card simplicity without redesigning resident core |
| Priya Nair (First-year resident) | **Supplemental** | Ensures newcomers can report without unwritten hostel knowledge |
| Kabir Shah (Urgent-only / sceptical resident) | **Supplemental** | Reminds us urgency + trust/status matter or people stop reporting small issues |

**Note on selection:** Primary personas drive the core experience; secondary personas must be satisfied without compromising primaries; supplemental personas ensure inclusion and edge coverage. No negative persona was required for this scope.

---

# Final Personas

---

## Persona 1: Aarav Mehta

**Frequent hostel resident reporter — Primary**

### Overview

| | |
|--|--|
| **Name** | Aarav Mehta |
| **Age** | 20 |
| **Role** | 2nd-year student, Block C Room 214 |
| **Persona type** | Primary |
| **Background** | Aarav shares a hostel room and lives mostly on his phone. He has already wasted a week waiting on a ceiling fan repair after messaging the floor group. He doesn’t want to “manage” maintenance — he wants to raise a problem once and know someone owns it. |

### Profile

**Activities**

- Notices room issues (fan, leak, lights)
- Reports via app (used to use WhatsApp groups)
- Checks request status between classes
- Uploads a photo when the form is short

**Attitudes**

- Practical, slightly impatient with silence
- Expects app-like speed
- Doesn’t want to nag people

**Aptitudes**

- High digital comfort
- Fast form filling
- Good at describing problems in short text

**Motivations**

- Get issues fixed without follow-up drama
- Keep room liveable for study/sleep
- Feel heard by the system

**Skills**

- Smartphone native
- Comfortable with notifications
- Can take a clear photo of the issue

**Goals**

- Report in under a minute
- See Assigned / In progress / Resolved
- Get urgent problems treated seriously

**Needs**

- Short report form
- Visible status timeline
- Notifications on change

**Pain points**

- “Ok noted” with no follow-through
- Repeating details on calls
- Not knowing who is coming

**Environment / context**

- Shared room, odd study hours
- Peak annoyance during heat / leaks
- Phone always nearby

**Relevant interactions**

- FixHostel Report / My Requests
- Warden (indirect via assign)
- Technician visit to room

### Persona type justification

Aarav represents the largest group of FixHostel users — regular residents who just want tracking. Designing for him covers the core report → track → rate loop, making him a **Primary** persona.

### Quote

> “Just tell me it’s assigned and when someone is coming.”

### Narrative

Aarav noticed water spreading under the washbasin in Room 214 one morning. Last time something broke, the floor group ate the message and nothing moved for days. This time he opened FixHostel, chose Plumbing, added Block C / 214, a short description, High urgency, and a photo. He saw **Submitted** immediately. Between lectures he got **Assigned**, then later **Resolved**. He checked the dry floor, left a quick rating, and for once didn’t send a single “any update?” text.

---

## Persona 2: Sneha Iyer

**Hostel warden / floor in-charge — Primary**

### Overview

| | |
|--|--|
| **Name** | Sneha Iyer |
| **Age** | 34 |
| **Role** | Hostel warden managing complaints across a few hundred residents |
| **Persona type** | Primary |
| **Background** | Sneha spends a large part of the day sorting requests that arrive as personal messages, group pings, and people stopping her in the corridor. On rainy days or after a power cut, everything feels urgent and she has no clean list of what’s still open. |

### Profile

**Activities**

- Reviews open maintenance queue
- Filters by urgency / block / status
- Assigns technicians
- Answers resident follow-ups (wants fewer of these)

**Attitudes**

- Efficient, decisive under pressure
- Low patience for messy chat threads
- Fair — wants serious issues first

**Aptitudes**

- Comfortable with phone apps
- Good at quick triage
- Can read a dense list if filters exist

**Motivations**

- Clear ownership of every ticket
- Reduce personal WhatsApp noise
- Keep hostel functioning on peak days

**Skills**

- Coordination across staff
- Prioritisation
- Knowing which technician fits which job

**Goals**

- One trusted open queue
- Assign the right person fast
- See what’s done vs still open

**Needs**

- Filters and badges
- Ticket detail with photo/location
- Assign confirm in few taps

**Pain points**

- Same issue reported three times
- No idea if electrician already went
- Residents asking for updates she doesn’t have

**Environment / context**

- Checks phone in short bursts
- Interrupted often while walking blocks
- Peak chaos after rain / power cuts

**Relevant interactions**

- FixHostel Warden Queue / Assign
- Technicians
- Residents (less direct if status works)

### Persona type justification

Sneha is **Primary** because she is the operational decision-maker. If triage and assign fail for her, resident reporting has nowhere to go.

### Quote

> “I need one list, not forty chat threads.”

### Narrative

After heavy rain, more than a dozen tickets hit the queue before noon. Sneha didn’t scroll aimlessly. She filtered **High** first — leaks, a loose wire, seepage near stairs — assigned those, then moved to **Medium**. When a student almost messaged her personally, she pointed them to the app status. By evening the High list was empty. Same rain chaos as always, but with order and ownership instead of a flooded WhatsApp.

---

## Persona 3: Ramesh Kumar

**Maintenance technician — Secondary**

### Overview

| | |
|--|--|
| **Name** | Ramesh Kumar |
| **Age** | 41 |
| **Role** | Campus electrician / plumbing contractor shared across blocks |
| **Persona type** | Secondary |
| **Background** | Ramesh gets pulled into jobs with incomplete information — wrong room, no photo, vague “AC problem.” He wastes time calling back for basics. He doesn’t need analytics; he needs today’s list and a way to mark done. |

### Profile

**Activities**

- Opens today’s job list
- Checks photo + location before going
- Fixes on site
- Updates status (Start / Resolved)

**Attitudes**

- Task-focused
- Low patience for fluff UI
- Practical and direct

**Aptitudes**

- Smartphone capable if screens are simple
- Strong hands-on repair skills
- Reads job cards faster than long chats

**Motivations**

- Finish jobs without repeat visits
- Avoid blame for missing info he never got
- Clear day plan

**Skills**

- Electrical / plumbing work
- Quick diagnosis from photo + description
- On-site problem solving

**Goals**

- Clear job card every time
- Update status in a few taps
- Move to the next job cleanly

**Needs**

- Room / block / problem / photo / urgency
- Large action buttons
- Less phone-calling for basics

**Pain points**

- Incomplete tickets
- Verbal stacks of instructions that get forgotten
- Residents expecting him to remember history

**Environment / context**

- Moving between blocks all day
- Tools in hand, phone in pocket
- Interrupted, standing, sometimes poor signal

**Relevant interactions**

- FixHostel Today’s Jobs / Job Detail
- Warden assign
- Resident at the door

### Persona type justification

Ramesh is **Secondary**. His need for simple job cards shapes staff UI, but designing only for him must not compromise the resident/warden primary flows.

### Quote

> “Give me the room, the problem, and a photo. That’s enough.”

### Narrative

After lunch Ramesh opened Today’s Jobs and saw a High plumbing card for Block C 214 with a photo of a wet pipe joint. No guessing. He tapped **Start work**, fixed the leak, marked **Resolved**, and moved on. Nobody called him three times for the room number. The ticket already had what he needed.

---

## Persona 4: Priya Nair

**First-year / process-confused resident — Supplemental**

### Overview

| | |
|--|--|
| **Name** | Priya Nair |
| **Age** | 18 |
| **Role** | 1st-year student, Block A |
| **Persona type** | Supplemental |
| **Background** | Priya has been in hostel only a few weeks. She doesn’t know the caretaker’s number or the “usual” WhatsApp process. She hesitates to post in big groups because she doesn’t want to look lost. |

### Profile

**Activities**

- Notices common-area or room issues
- Asks roommate what to do
- Avoids noisy groups when unsure
- Uses guided report form when available

**Attitudes**

- Careful, slightly anxious
- Doesn’t want to bother seniors
- Willing to use an official app

**Aptitudes**

- Digitally comfortable
- Needs clearer labels than seniors
- Learns process fast once shown once

**Motivations**

- Stay safe (e.g. dark corridor)
- Fit into hostel without embarrassment
- Get help without social risk

**Skills**

- Smartphone use
- Following simple forms
- Describing location in plain words

**Goals**

- Report without knowing unwritten rules
- See that someone received it
- Avoid public group exposure

**Needs**

- Obvious Report CTA
- Common-area option
- Status so she doesn’t keep asking people

**Pain points**

- Not knowing who to contact
- Fear of posting dumb questions
- Silence after verbal complaints

**Environment / context**

- New to blocks and staff names
- Evenings in corridors / stairs
- Relies on roommate for “how things work”

**Relevant interactions**

- FixHostel Report (common area)
- Indirect warden/technician
- Roommate advice

### Persona type justification

Priya is **Supplemental**. She ensures FixHostel works for newcomers who lack hostel process knowledge — inclusion without changing the primary resident flow.

### Quote

> “I don’t even know who to message. I just want a proper place to report it.”

### Narrative

Priya walked back from mess and found the 2nd floor corridor light dead near the stairs. Her roommate said to post in the group; Priya opened it and closed it again. In FixHostel she picked Electrical, Common area, “Block A – 2nd floor corridor near stairs,” Medium urgency, and submitted. **Submitted** then **Assigned** arrived without her asking three seniors what to do. By evening the light was on. The app had carried the process she didn’t know yet.

---

## Persona 5: Kabir Shah

**Urgent-only / sceptical resident — Supplemental**

### Overview

| | |
|--|--|
| **Name** | Kabir Shah |
| **Age** | 22 |
| **Role** | Final-year student |
| **Persona type** | Supplemental |
| **Background** | Kabir used to report small issues, then stopped after too many ignored chats. Now he only raises something when it is serious — leak, no power, safety. He will use FixHostel only if status proves someone actually saw the ticket. |

### Profile

**Activities**

- Ignores minor annoyances
- Reports only high-impact problems
- Checks status once, not obsessively
- Quits channels that waste time

**Attitudes**

- Sceptical from past experience
- Direct, low patience
- Will re-engage if system shows proof

**Aptitudes**

- Digitally fluent
- Good at judging urgency
- Minimal form tolerance

**Motivations**

- Don’t waste effort on black holes
- Fix only what blocks living/studying
- Trust actions over promises

**Skills**

- Clear urgent descriptions
- Photo when it matters
- Filtering noise

**Goals**

- Serious tickets jump the queue
- Visible proof of assign/progress
- Minimal steps

**Needs**

- Urgency marking that means something
- Fast High-path on warden side
- Honest status

**Pain points**

- Past ignored reports
- Fake “we’ll look into it”
- Long forms

**Environment / context**

- Busy final-year schedule
- Only opens maintenance tools when stuck
- Influences juniors (“don’t bother reporting”)

**Relevant interactions**

- FixHostel Report (High)
- Status notifications
- Rare direct staff contact

### Persona type justification

Kabir is **Supplemental**. He pressures the design to make urgency and status real — otherwise residents stop reporting and the whole system loses trust.

### Quote

> “If it doesn’t show assigned, I’m not wasting another message.”

### Narrative

When Kabir’s room lost power to half the sockets after a short circuit smell, he almost didn’t report — old habit. He tried FixHostel anyway, marked **High**, added a photo of the board area, and submitted. Seeing **Assigned** within an hour was the only reason he didn’t escalate angrily to the warden’s personal chat. Status, for him, is the product.

---

# Persona Comparison Summary

Five personas side by side.

| Persona | Main behavioural driver | Main goal | Main need | Main pain point | Type |
|---------|-------------------------|-----------|-----------|-----------------|------|
| Aarav Mehta | Status-seeking self-serve | Get issues tracked and fixed | Short report + timeline | Silence after “ok noted” | Primary |
| Sneha Iyer | Operational oversight | Triage and assign cleanly | One queue + filters | Forty chat threads | Primary |
| Ramesh Kumar | Field execution | Finish jobs prepared | Room + problem + photo | Incomplete tickets | Secondary |
| Priya Nair | Process confusion | Report without unwritten rules | Guided common-area report | Not knowing who to contact | Supplemental |
| Kabir Shah | Trust / urgency only | Serious issues actually move | Urgency that works + status proof | Ignored past reports | Supplemental |

---

# How to turn this into Personas.pdf (for submission)

1. Open this file in **Google Docs** / **Word** / **Notion**, or paste section-by-section into **Figma** frames (one step / persona per frame — closest to the class PDF look).
2. For final persona pages, add a **circular photo placeholder** beside the Overview box (stock or illustrated student/warden/technician).
3. Keep **purple** box = persona type justification, **yellow** box = quote (same as class PDF).
4. Export: **File → Export → PDF** (Docs/Word) or Figma **Export frames as PDF**.
5. Submit editable source (Figma/Doc) + **Personas.pdf** together with the other Unit 4 raw files.

**Suggested PDF page order (match class style):**  
Overview → Step 1 → Step 2 → Step 3 → Step 4 → Step 5 → Step 6 → Step 7 → Persona 1…5 → Comparison Summary
