# Part 6: Agile, Scrum, Kanban, and Backlogs

**Source note:** As publicly described, Google's *Agile Project Management* course covers Agile values and principles, Scrum (roles, events, artifacts), Kanban and other Agile approaches, and backlogs, user stories, and sprints. I haven't re-checked Coursera live, so confirm the current contents there. **[Supplemental]** marks my additions (INVEST, WSJF, flow metrics, burnup charts). For Scrum rules I follow the **Scrum Guide (2020 edition)**, and I label what is *required by Scrum* versus *common practice*, because many courses blur the two. Templates, numbers, and questions are my original material, not official Google content.

This part covers **Skills 16 (Backlogs)** and **17 (Agile Project Management)**, plus the velocity and burndown calculations promised in Part 3.

**Terminology note:** Google's course materials (as I recall) use "development team." The 2020 Scrum Guide says there is one **Scrum Team** made up of a Scrum Master, a Product Owner, and **Developers** (anyone doing the work: designers, testers, and programmers, not only coders). Exams may use either wording.

---

## 1. Learning Objectives

By the end of Part 6 you should be able to:
- Explain Agile values and principles, and when Agile or predictive suits a project
- Describe Scrum's roles, events, and artifacts, and separate required rules from common practice
- Build and prioritize a product backlog, and write user stories with acceptance criteria
- Plan, run, and review a sprint, including handling scope change and impediments
- Use Kanban boards and work-in-progress (WIP) limits
- Calculate velocity, forecast with it, and read a burndown chart

**Running example:** an **Agile re-telling** of BrightCuts. Twelve weeks become six two-week sprints. The numbers differ from the predictive plan in Part 3 on purpose, so you can compare the two approaches. Maria Lopez acts as **Product Owner**. You act as project manager and coordinate with a Scrum Master (an experienced team member could fill this role). The team is Dev, Priya (designer), and Sam (tester).

---

## 2. How the Pieces Connect

```
Product Goal → Product Backlog (ordered) → Sprint Planning → Sprint Backlog
      ↑                                                            ↓
 Backlog updated ← Sprint Review ← Increment ← Daily work (Daily Scrum)
      ↑                                  ↓
      └────────── Sprint Retrospective (improve the process)
```

Predictive projects plan most of the work up front. Agile projects plan the *next slice* in detail, deliver it, learn from it, and adjust. The backlog is the living scope. The sprint is the delivery rhythm. Reviews and retrospectives are the feedback loops.

---

## 3. Predictive vs. Adaptive (Agile) Project Management

| | Predictive (waterfall) | Adaptive (Agile) | Hybrid |
|---|---|---|---|
| Requirements | Fixed early | Expected to evolve | Core fixed, details evolve |
| Planning | Detailed up front | Rolling: plan the next sprint in detail | Phase plan plus sprints inside |
| Delivery | One main delivery near the end | Working increments every sprint | Mixed |
| Change | Formal change control | Welcomed through backlog ordering | Both |
| Customer involvement | At milestones | Continuous | Frequent |
| Best when | Requirements are stable; regulated or physical work | Requirements uncertain; fast feedback valuable | Fixed deadline or contract with uncertain features |
| Typical metrics | CPI, SPI, critical path | Velocity, burndown, cycle time | Both |

**Practical guidance:** choose by uncertainty and cost of change, not by fashion. A hospital building suits predictive. A new consumer app with unknown demand suits Agile. A fixed-price contract with some unclear features often suits hybrid.

### Agile values (Agile Manifesto, 2001), paraphrased
1. People and their interactions matter more than processes and tools.
2. Working software matters more than exhaustive documentation.
3. Collaborating with customers matters more than negotiating contracts.
4. Responding to change matters more than following a plan.

The manifesto says the items on the right still have value, but the items on the left are valued *more*. Agile does not mean "no documentation" or "no planning."

**Principles in plain English:** satisfy the customer through early, continuous delivery; welcome changing requirements; deliver working results frequently; business people and developers work together daily; trust motivated people; talk face to face when possible; working product is the main measure of progress; keep a sustainable pace; pursue technical excellence; keep things simple; let teams self-organize; reflect regularly and adjust.

**Other approaches [Supplemental]:** *Lean* focuses on eliminating waste and improving flow. *Extreme Programming (XP)* adds engineering practices such as pair programming, test-driven development, and continuous integration. Kanban and Scrum are the two you must know best for this course.

---

## 4. Skill 17: Agile Project Management

**Definition:** Managing work in short iterative cycles with frequent delivery, close customer collaboration, and regular reflection, adapting plans as you learn.

**Why it matters:** When requirements are uncertain, delivering small increments reduces the risk of building the wrong thing for months.

**When to use:** Projects with uncertain or evolving requirements, where customers can give frequent feedback and work can be delivered in slices. Be cautious where late change is extremely costly or regulation demands full upfront specification.

### Scrum: the framework

**Scrum (per the Scrum Guide) is built on three pillars:** transparency (work is visible), inspection (check progress and results often), and adaptation (adjust when needed).

**Roles (called "accountabilities" in the 2020 guide)**

| Role | Accountable for | BrightCuts |
|---|---|---|
| **Product Owner (PO)** | Maximizing product value; ordering the Product Backlog; one person, not a committee | Maria |
| **Scrum Master** | Scrum being understood and effective; coaching; removing impediments; facilitating events as needed | Team member or coach |
| **Developers** | Creating a usable Increment each Sprint; planning the Sprint Backlog; holding each other accountable to the Definition of Done | Dev, Priya, Sam |

**Events**

| Event | Purpose | Max length for a 1-month Sprint* |
|---|---|---|
| **Sprint** | Container for all other events; a fixed-length cycle of one month or less | 1 month |
| **Sprint Planning** | Decide *why* (Sprint Goal), *what* (items), and *how* (plan) | 8 hours |
| **Daily Scrum** | Developers inspect progress toward the Sprint Goal and adapt the plan | 15 minutes |
| **Sprint Review** | Inspect the Increment with stakeholders and adapt the Product Backlog | 4 hours |
| **Sprint Retrospective** | Plan improvements to quality and effectiveness | 3 hours |

*Shorter Sprints normally have shorter events. For a two-week Sprint, teams commonly plan for about 2 to 4 hours of planning, 1 to 2 hours for review, and 1 to 1.5 hours for the retrospective. Those numbers are common practice, not rules.*

**Artifacts and their commitments**

| Artifact | Commitment | Meaning |
|---|---|---|
| **Product Backlog** | **Product Goal** | Ordered list of what the product might need; the goal is the long-term objective |
| **Sprint Backlog** | **Sprint Goal** | Items selected for the Sprint plus the plan to deliver them; the goal is the single purpose of the Sprint |
| **Increment** | **Definition of Done** | A usable, integrated step toward the Product Goal that meets the Definition of Done |

### What Scrum requires vs. common practice

**Avoid exam traps: many popular practices are *not* in the Scrum Guide.**

| Required by Scrum | Common practice, **not required** |
|---|---|
| Scrum Team: PO, Scrum Master, Developers | User story format ("As a... I want... so that...") |
| Sprints of one month or less, fixed length | Story points and planning poker |
| The five events | Velocity and burndown charts |
| Three artifacts with their commitments | The "three daily questions" format |
| Sprint Goal stays fixed during the Sprint | Definition of Ready |
| Definition of Done shared by the team | MoSCoW prioritization |
| Only the PO can cancel a Sprint | Two-week Sprint length; "Sprint Zero" |
| Developers own the Sprint Backlog and how they do the work | A separate "backlog refinement meeting" (the guide treats refinement as ongoing activity, not an event) |

### The Sprint step by step (BrightCuts, two weeks)

1. **Sprint Planning (day 1):** PO proposes the value; Developers forecast what they can complete; together they write a **Sprint Goal**; Developers plan the work.
2. **Daily Scrum (each day, 15 min):** Developers coordinate toward the Sprint Goal and surface impediments.
3. **Work:** build, test, and integrate. Items are "done" only when they meet the Definition of Done.
4. **Refinement (ongoing):** PO and Developers clarify, split, and estimate upcoming backlog items.
5. **Sprint Review (last days):** show the Increment to stakeholders, collect feedback, discuss what to build next. It is a working session, not a one-way status presentation.
6. **Sprint Retrospective (last):** the team inspects how it worked and agrees improvements.
7. **Next Sprint starts immediately.**

### Handling scope changes during a sprint

| Situation | Guidance |
|---|---|
| New idea or request mid-Sprint | Add it to the Product Backlog. The PO orders it for a future Sprint |
| Real emergency (e.g., a critical production defect) | PO and Developers discuss. If it can't wait, they may swap items. The Sprint Goal still stands |
| Scope turns out larger or smaller than thought | Developers and PO **renegotiate the scope** while keeping the Sprint Goal intact |
| The Sprint Goal itself becomes obsolete | Only the **Product Owner** may cancel the Sprint (rare and disruptive) |
| Developers finish early | They talk with the PO about pulling more work that supports the goal |

**Key point:** the *Sprint Goal* is protected, and the *scope* underneath it is flexible by agreement. Nobody outside the team should push work into the Sprint.

### Managing dependencies and impediments

- **Impediment:** anything blocking progress (a vendor delay, a broken test server, an unresolved decision). Raise it at the Daily Scrum. The Scrum Master helps remove it or escalates.
- **Dependency:** work that relies on another item, team, or vendor. Ways to manage them: reorder the backlog, split stories to remove the link, build against a mock (as with the payment API), agree delivery dates with the other party, track them visibly, and avoid committing to work whose dependency isn't ready.
- **Scrum of Scrums [Supplemental]:** a common (not required) way for several teams to coordinate dependencies.

### The project manager in Agile

A PM's role varies. In pure Scrum there is no "project manager" accountability. The duties still exist and get shared:

| Duty | Who often covers it in Agile |
|---|---|
| Product vision, backlog order | Product Owner |
| Process, impediments, team effectiveness | Scrum Master |
| Task planning and how to build | Developers |
| Budget, vendor contracts, risks, stakeholders, cross-team coordination, reporting | PM, program manager, or PO, depending on the organization |

**If you are a developer moving into PM:** resist the urge to prescribe *how* things are built (Developers decide) or to reorder the backlog (the PO does). Your value lies in protecting the team from interruption, making risks and dependencies visible, and keeping stakeholders informed.

**Agile risk, budget, and scope in brief**
- **Risk:** handled continuously. Risky items are often scheduled early to learn sooner, and impediments are surfaced daily. A risk register still helps for external risks.
- **Budget:** commonly based on team capacity (people × time) rather than task-by-task estimates. Scope flexes to fit the budget.
- **Scope:** the Product Backlog changes. Success is measured by value delivered, not by matching an original plan.

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| "Agile" used to mean no planning | Keep a Product Goal, ordered backlog, and Sprint Goals |
| Stakeholders push work into sprints | Route all requests through the PO and backlog |
| Sprint Review becomes a status meeting | Demo working product and ask for feedback to shape the backlog |
| Retrospective actions never happen | Pick 1 to 2 actions, assign owners, review them next retro |
| Velocity used to compare teams or pressure people | Use it only for the team's own forecasting |
| Fixed deadline and fixed scope | Use hybrid, or negotiate scope by priority |
| Remote team loses cohesion | Short daily check-ins, shared board, recorded demos |

**Relationships:** Agile replaces much of the upfront WBS and schedule with a **backlog** and **sprints**, still needs **stakeholder analysis**, **communication**, and **risk** work, uses the **Definition of Done** as its **quality** gate, and handles **change** through backlog ordering instead of heavy change control (though contracts may still require formal change control).

---

## 5. Skill 16: Backlogs

**Definition:** An ordered list of the work needed to deliver value, kept visible and continuously updated. The **Product Backlog** lists everything that might be needed in the product. The **Sprint Backlog** is the subset chosen for the current Sprint plus the plan to deliver it.

| | Product Backlog | Sprint Backlog |
|---|---|---|
| Owner | Product Owner (accountable for ordering) | Developers |
| Content | Features, fixes, improvements, with varying detail | Chosen items plus a plan for the Sprint |
| Changes | Constantly | By the Developers as they learn, while protecting the Sprint Goal |
| Life span | Life of the product | One Sprint |
| Commitment | Product Goal | Sprint Goal |

**Why it matters:** It is the single, transparent source of what is to be done and in what order. Without it, priorities live in people's heads and arguments.

### Backlog management process
1. **Capture** ideas, needs, and bugs in one place.
2. **Write** items clearly (user stories are common).
3. **Refine:** add detail, split large items, clarify acceptance criteria, and estimate. Done continuously.
4. **Prioritize/order** by value, risk, dependency, and effort.
5. **Plan:** top items feed Sprint Planning.
6. **Inspect and adapt** after each Review.

### Epics, stories, tasks
- **Epic:** a large body of work ("Payments").
- **User story:** a small slice of value from a user's view.
- **Task:** a technical step to build the story ("create payment API client").

### User stories **[Supplemental: common practice, not required by Scrum]**

**Format:** *As a [type of user], I want [goal], so that [benefit].*

**INVEST checklist for a good story:**

| Letter | Meaning |
|---|---|
| **I**ndependent | Can be built without being tied to others |
| **N**egotiable | A conversation, not a contract |
| **V**aluable | Delivers value to a user or the business |
| **E**stimable | The team can size it |
| **S**mall | Fits within a Sprint |
| **T**estable | You can tell when it's done |

**Acceptance criteria:** specific conditions for that story to be accepted. A popular format is **Given / When / Then**.

### Template: User Story with Acceptance Criteria (completed)

| Field | Content |
|---|---|
| ID | PB-04 |
| Story | As a customer, I want to cancel or reschedule my appointment online up to 2 hours before it starts, so that I don't have to phone the salon. |
| Acceptance criteria | **Given** I have a booking more than 2 hours away, **when** I choose "Cancel," **then** the slot is released and I receive a confirmation email. **Given** my booking is less than 2 hours away, **when** I open it, **then** the cancel option is disabled and a phone number is shown. **Given** I reschedule, **when** I pick a new slot, **then** the old slot is released only after the new one is confirmed. |
| Estimate | 5 points |
| Notes | Depends on PB-03 (booking confirmation) |

### Definition of Ready vs. Definition of Done

| | Definition of Ready (DoR) | Definition of Done (DoD) |
|---|---|---|
| Status | Common practice, **optional** | **Required** (commitment for the Increment) |
| Applies to | Backlog items entering a Sprint | Every item in the Increment |
| Question | "Is this clear enough to start?" | "Is this finished to our quality standard?" |
| Example | Story written, criteria agreed, estimated, no blocking dependency | Code reviewed, tests pass, integrated, documented, accepted by PO |

**Acceptance criteria vs. DoD:** acceptance criteria are specific to *one* story. The DoD is a shared quality standard for *all* stories. Be careful with this on exams.

### Prioritization methods

**MoSCoW** **[Supplemental]:**

| Category | Meaning | BrightCuts |
|---|---|---|
| **Must have** | Without it, the release fails | Book, cancel, pay deposit |
| **Should have** | Important, but a workaround exists | Reminders, stylist time-off |
| **Could have** | Nice to have if capacity allows | Color-coded calendar |
| **Won't have (this time)** | Agreed out of scope for this release | Loyalty points |

"Won't" means *not now*, not *never*.

**Other methods:**
- **Value vs. effort grid:** do high-value, low-effort items first.
- **Weighted Shortest Job First (WSJF) [Supplemental]:** score = (business value + time criticality + risk reduction) ÷ job size. Highest score first.
- **Risk-first:** tackle the riskiest or most uncertain items early to learn sooner (useful for the payment integration).
- **Dependencies:** items that unblock many others move up.

### Estimating with story points **[Supplemental]**

- A **story point** is a relative size that combines effort, complexity, and uncertainty. It is *not* hours.
- Teams often use a Fibonacci-like scale (1, 2, 3, 5, 8, 13) and **planning poker**: each person picks a card privately, they reveal together, discuss differences, and re-vote.
- Compare to a **reference story** ("This is about twice the size of the 3-pointer").
- Anything 13 or larger is usually split.
- Points are **team-specific**: one team's 5 is not another team's 5.

### Template: Agile Product Backlog (completed, start of project)

| ID | Story (short) | MoSCoW | Points | Order | Status |
|---|---|---|---|---|---|
| PB-01 | Browse services and prices | Must | 3 | 1 | Ready |
| PB-02 | Select stylist and time slot | Must | 8 | 2 | Ready |
| PB-03 | Confirm booking, send confirmation email | Must | 5 | 3 | Ready |
| PB-04 | Cancel or reschedule up to 2 hours before | Must | 5 | 4 | Ready |
| PB-06 | Receptionist daily calendar view | Must | 8 | 5 | Ready |
| PB-09 | Admin: manage services and prices | Must | 5 | 6 | Ready |
| PB-05 | Pay deposit at booking | Must | 13 | 7 | Needs splitting |
| PB-07 | Stylist blocks out time off | Should | 5 | 8 | Ready |
| PB-08 | Email reminder 24 hours before | Should | 5 | 9 | Needs criteria |
| PB-10 | Color-coded calendar by stylist | Could | 3 | 10 | Idea |
| PB-12 | Basic bookings report | Could | 5 | 11 | Idea |
| PB-11 | SMS reminders | Could | 8 | 12 | Idea |
| PB-13 | Loyalty points | Won't (this release) | 13 | n/a | Parked for release 2 |

**Totals:** Must = 47, Should = 10, Could = 16 (Must + Should + Could = **73**). Won't = 13.

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Backlog becomes a dumping ground | Review regularly; delete or archive stale items |
| Everything is "high priority" | Force-rank (one ordered list) and use MoSCoW with a cap on Musts |
| Too many people order the backlog | One accountable PO; others advise |
| Stories too big | Split by workflow step, rule, or data variation |
| Vague stories | Add acceptance criteria; clarify in refinement |
| Estimates treated as promises | Remind everyone they are forecasts |
| Technical work ignored | Make technical work visible in the backlog and weigh it against value |

**Relationships:** The backlog replaces the WBS and much of the scope statement in Agile. Its acceptance criteria connect to **quality**, its dependencies to **risk**, and its ordering to **stakeholder** expectations and the **Product Goal**.

---

## 6. Sprint Planning, Review, and Retrospective Templates

### Template: Sprint Planning (completed, Sprint 2)

| Field | Content |
|---|---|
| Sprint | 2 (two weeks) |
| Product Goal | 60% of bookings made online within 3 months of launch |
| **Sprint Goal** | Customers can cancel or reschedule online, and the receptionist can see the day's bookings and manage services |
| Capacity | 3 Developers, 1 day of planned leave (Sam). Recent velocity: 16 |
| Forecast | PB-04 (5) + PB-06 (8) + PB-09 (5) = **18 points** |
| Plan (tasks) | PB-04: cancel API, email template, tests. PB-06: calendar view, filters, tests. PB-09: service CRUD screen, validation, tests |
| Dependencies | PB-04 needs PB-03 from Sprint 1 (complete) |
| Risks | Calendar view performance with many bookings |
| Definition of Done | Reviewed, tested, integrated, accepted by PO |

### Template: Sprint Review and Retrospective (completed, Sprint 2)

**Sprint Review**

| Item | Content |
|---|---|
| Attendees | Scrum Team, Maria (PO), Tom, two stylists |
| Sprint Goal met? | Yes. All 3 items Done (18 points) |
| Demo | Cancel and reschedule flow; receptionist calendar; service editing |
| Feedback | Tom wants to see walk-ins on the calendar. Stylists want colors per stylist |
| Backlog changes | Add PB-14 "walk-in bookings" (Should, 3 points). PB-10 (colors) moves up |
| Next | Sprint 3 will focus on deposit payment |

**Sprint Retrospective**

| What went well | What didn't | Improvement actions (owner, by when) |
|---|---|---|
| Stories were small enough to demo | PB-06 finished only on the last day | Split stories larger than 5 points (PO and Dev, Sprint 3) |
| Test data was ready early | Review requests waited 2 days | Review within 1 working day (all, starting tomorrow) |
| Tom's early feedback saved rework | Two items were started at once | Limit work in progress to 2 items per person (Scrum Master) |

### Template: Burndown Chart (completed, Sprint 2)

A **sprint burndown** plots remaining work (story points) against time. The ideal line falls steadily. The actual line shows what really got finished. 18 points over 10 working days gives an ideal slope of **1.8 points per day**.

| Day | Ideal remaining | Actual remaining | What happened |
|---|---|---|---|
| 0 | 18.0 | 18 | Sprint starts |
| 2 | 14.4 | 18 | Nothing finished yet |
| 3 | 12.6 | 13 | PB-04 done (5 points) |
| 4 | 10.8 | 13 | |
| 5 | 9.0 | 13 | Behind ideal by 4 points |
| 6 | 7.2 | 8 | PB-09 done (5 points) |
| 8 | 3.6 | 8 | PB-06 in testing |
| 10 | 0 | 0 | PB-06 done (8 points). Goal met |

```
Pts
18 |■ ■
13 |      ■ ■ ■
 8 |            ■ ■ ■ ■
 0 |                      ■
   +--------------------------
    0  2  3  4  5  6  8  10 Day
```

**How to read it**
- The line steps down because points count only when an item is **Done**, not when it is "half finished."
- Above the ideal line mid-sprint means you're behind pace. Below means you're ahead.
- A flat line followed by a sudden drop suggests items are too large or too many were started at once.
- A line that **rises** means scope was added or items were re-estimated upward.
- **Burnup chart [Supplemental]:** plots work completed *and* total scope on one chart. It shows scope changes more clearly than a burndown.

---

## 7. Kanban

**Definition:** A visual method for managing flow. Work items move across a board's columns, and limits on work in progress keep the team from starting more than it can finish. Kanban has no required sprints, roles, or events.

**Principles:** visualize the work, limit WIP, manage flow, make policies explicit, improve continuously.

**Pull system:** you start a new item only when capacity opens up in your column, instead of pushing work in.

### Example: BrightCuts post-launch support board

```
Backlog | Ready (limit 5) | In Progress (limit 3) | Review (limit 2) | Done
 ■ ■ ■ ■ |  ■ ■ ■          |  ■ ■ ■                |  ■ ■             |  ■ ■ ■ ■
```

*"In Progress" is full (3 of 3). Nobody starts a new item until one moves to Review. That forces the team to finish work and exposes bottlenecks, such as a growing Review column.*

### Flow metrics **[Supplemental]**

| Metric | Meaning | Example |
|---|---|---|
| **Lead time** | From request to delivery | Request on Monday, delivered next Friday: 11 calendar days |
| **Cycle time** | From work started to done | Started Tuesday, done Friday: 3 days |
| **Throughput** | Items finished per period | 6 items this week |
| **WIP** | Items in progress | 3 |

**Little's Law (approx.):** average cycle time ≈ WIP ÷ throughput. With WIP = 6 and throughput = 3 per week, the average cycle time is about 2 weeks. Reducing WIP shortens cycle time.

### Scrum vs. Kanban vs. Waterfall

| | Scrum | Kanban | Waterfall |
|---|---|---|---|
| Cadence | Fixed Sprints | Continuous flow | Sequential phases |
| Roles | PO, Scrum Master, Developers | None required | PM, functional roles |
| Change | Between Sprints via backlog (Sprint Goal fixed in a Sprint) | Anytime, within WIP limits | Formal change control |
| Key limit | Sprint timebox and capacity | WIP limits | Phase gates |
| Metrics | Velocity, burndown (common) | Cycle time, throughput | CPI, SPI |
| Best for | New product development in iterations | Support, maintenance, steady streams | Stable, well-defined scope |

**Scrumban [Supplemental]:** Scrum with Kanban-style boards and WIP limits.

---

## 8. Agile Numerical Problems (Velocity and Burndown)

**Predictive vs. Agile metrics:** CPI and SPI compare progress to a fixed baseline, so they fit predictive projects. Velocity measures a team's *own* delivered capacity, so it fits Agile work. Velocity is a **planning tool, not a performance score**, and it can't be compared across teams (points differ). Hybrid projects often use both.

### 8.1 Sprint Velocity
- **Formula:** Velocity = sum of story points of items that fully meet the Definition of Done in a sprint.
- **Variables:** story points (relative size); *Done* means finished to the DoD (partially done work counts as **zero**).
- **Useful when:** forecasting how much the team can take next sprint.
- **Worked example (BrightCuts):** Sprint 1 = 16, Sprint 2 = 18, Sprint 3 = 5. **Average velocity = (16 + 18 + 5) ÷ 3 = 13**.
- **Plain English:** The team has been completing about 13 points per sprint. Sprint 3 was low for reasons explained in Case 10, so use judgment about whether it is typical.

| Practice | Solution |
|---|---|
| 1. Sprints of 14, 18, 16 points. Average? | 48 ÷ 3 = **16** |
| 2. Committed 5 stories (3, 3, 5, 5, 8). Four finished, the 8-pointer is 90% done. Velocity? | 3+3+5+5 = **16**. Partial work doesn't count |
| 3. Velocities 20, 24, 22, 18. Average of the last 3? | (24+22+18) ÷ 3 = 21.3, about **21** |

### 8.2 Release Forecast
- **Formula:** Sprints needed = remaining backlog points ÷ average velocity (round **up**).
- **Useful when:** estimating how many sprints a set of backlog items will take.
- **Worked example (start of project):** Must + Should = 57 points. With velocity 18: 57 ÷ 18 = 3.17, so **4 sprints**. Everything (73 points): 73 ÷ 18 = 4.06, so **5 sprints**. With six sprints available, the team has a spare sprint for hardening, user acceptance testing, and launch.
- **Plain English:** The forecast is a range, not a promise. It is refreshed after every sprint.

| Practice | Solution |
|---|---|
| 1. 90 points remain, velocity 15 | 90 ÷ 15 = **6 sprints** |
| 2. 100 points remain, velocity 18 | 5.56, so **6 sprints** |
| 3. 6 sprints left, 2 reserved for hardening and launch, velocity 20. Can 80 points be delivered? | 4 build sprints × 20 = 80, so **yes, exactly**, with no buffer, which is risky |

### 8.3 Burndown Interpretation

| Practice | Solution |
|---|---|
| 1. The line stays flat for the first week, then drops sharply | Stories too large or too many started at once. Split stories and limit WIP |
| 2. The line **rises** on day 5 | Scope added or an item re-estimated upward. Check with the PO whether the Sprint Goal is still safe |
| 3. The line is well below ideal and hits zero on day 7 | The team may have over-estimated or under-committed. Discuss with the PO pulling in more goal-supporting work, and revisit estimates in the retrospective |

---

## 9. Common Mistakes

| Mistake | How to avoid |
|---|---|
| Treating Scrum practices (stories, points, DoR) as mandatory rules | Know the Scrum Guide's required parts |
| Changing the Sprint Goal mid-sprint | Protect the goal; renegotiate scope only |
| Letting managers assign work into the sprint | Developers pull work; the PO orders the backlog |
| Using velocity as a target or to compare teams | Use it only for the team's own forecasting |
| Counting partly done work | Only Done items count |
| Skipping retrospectives | Hold them every Sprint; follow up on actions |
| A Sprint Review that is only a slideshow | Show working product and gather feedback |
| No Product Goal | Link every sprint to a longer-term aim |
| PM acting as Product Owner without authority | Clarify who owns value decisions |

---

## 10. Module Summary and Revision Notes

- Agile is **iterative and adaptive**. Predictive is **plan-driven**. Hybrid mixes them.
- Scrum Team: **Product Owner, Scrum Master, Developers**. Events: **Sprint, Planning, Daily Scrum, Review, Retrospective**. Artifacts: **Product Backlog, Sprint Backlog, Increment**, each with a commitment (**Product Goal, Sprint Goal, Definition of Done**).
- The **Sprint Goal is fixed**. Scope under it can be renegotiated between the PO and Developers. Only the PO cancels a Sprint.
- User stories, story points, velocity, burndown, MoSCoW, and DoR are **common but not required**.
- **DoD** (all items, required) differs from **acceptance criteria** (per story).
- **MoSCoW:** Must, Should, Could, Won't (this time).
- **Velocity** = points of Done items per sprint. **Forecast** = remaining points ÷ average velocity, rounded up.
- **Kanban:** visualize, limit WIP, pull, improve. Metrics: cycle time, lead time, throughput.
- The Agile PM focuses on stakeholders, risks, dependencies, impediments, and protecting the team.

---

## 11. Skill-by-Skill Question Sets

*Brief explanations are included. The full 10-field format appears in the numbered bank in Part 8.*

### Skill 16: Backlogs

**Beginner**
1. **What is a product backlog?** An ordered list of everything that might be needed to improve the product.
2. **Who is accountable for ordering it in Scrum?** The Product Owner.
3. **What is a user story?** A short description of a feature from the user's view: As a..., I want..., so that...
4. **What does MoSCoW stand for?** Must, Should, Could, Won't (this time).
5. **True or false: the product backlog is fixed after the project starts.** False. It evolves continuously.

**Intermediate**
1. **Product backlog vs. sprint backlog?** The product backlog holds everything for the product. The sprint backlog holds the selected items and plan for one sprint.
2. **What does INVEST stand for?** Independent, Negotiable, Valuable, Estimable, Small, Testable.
3. **Acceptance criteria vs. Definition of Done?** Acceptance criteria are specific to one story. The DoD is a quality standard for all items.
4. **What are story points?** A relative measure of size that combines effort, complexity, and uncertainty. They are not hours.
5. **Is a Definition of Ready required by Scrum?** No. It is a common optional practice. *Why it matters:* exams often test required vs. optional.

**Scenario**
1. **Five stakeholders each say their item is top priority.** Gather criteria tied to the Product Goal, have the PO order the list, and explain the reasoning openly. *Reasoning:* one accountable decider, transparent criteria.
2. **A story is 13 points and the sprint is two weeks.** Split it into smaller stories that each deliver value (for example, pay with a mock first, then the live provider).
3. **The sponsor wants a new feature added to the sprint on day 4.** Add it to the product backlog. The PO may reorder it for the next sprint. *Reasoning:* protect the Sprint Goal.
4. **A story has no acceptance criteria and the team disagrees on what's needed.** Clarify with the PO in refinement, write criteria, then estimate.
5. **The backlog has 200 old items nobody reads.** Prune, merge, and archive. Keep the top items detailed and the tail light.

**Interview**
1. **How do you prioritize a backlog?** *Sample:* "I link every item to the product goal, then use value, risk, effort, and dependencies. MoSCoW helps with release scope. The Product Owner makes the final call."
2. **Tell me about a time priorities competed.** *Sample (STAR):* "Three stakeholders wanted different features first. I ran a short workshop to agree scoring criteria, the PO ordered the list, and we explained the reasoning. Complaints dropped and the first release shipped on time."
3. **How do you write a good user story?** "Short, from the user's view, with the benefit, testable acceptance criteria, and small enough to finish in a sprint."
4. **How do you estimate with story points?** "Relative sizing against a reference story, planning poker to surface differences, and splitting anything too large."
5. **What's the difference between a backlog and a requirements document?** "A backlog is a living, ordered list that changes as we learn. A traditional requirements document is usually fixed and approved up front."

### Skill 17: Agile Project Management

**Beginner**
1. **Name the three Scrum roles.** Product Owner, Scrum Master, Developers.
2. **Name the five Scrum events.** Sprint, Sprint Planning, Daily Scrum, Sprint Review, Sprint Retrospective.
3. **How long is the Daily Scrum?** 15 minutes at most.
4. **What is a sprint?** A fixed-length cycle (one month or less) in which a usable Increment is created.
5. **True or false: Agile means no planning.** False. It means planning continuously in smaller steps.

**Intermediate**
1. **What is the purpose of the Sprint Review?** To inspect the Increment with stakeholders and adapt the Product Backlog.
2. **What is the purpose of the Retrospective?** To plan improvements to how the team works.
3. **Who can cancel a Sprint?** Only the Product Owner.
4. **Predictive vs. adaptive?** Predictive fixes scope early and plans in detail. Adaptive expects change and plans iteratively.
5. **What does a WIP limit do?** It caps work in progress to improve flow and expose bottlenecks.

**Scenario**
1. **The team can't finish the Sprint Goal.** Developers talk to the PO about renegotiating scope while protecting the goal. If the goal is obsolete, the PO may cancel. Review and retro explain what happened.
2. **A senior manager tells a developer to do an urgent side task.** Redirect to the PO and add it to the backlog. Swap only by agreement. *Reasoning:* protect the team's focus.
3. **Retro actions are never completed.** Choose one or two, assign owners, and review them at the start of the next retro.
4. **Velocity drops three sprints in a row.** Investigate: team changes, tech debt, unclear stories, interruptions. Share findings, don't push people to "go faster."
5. **A stakeholder asks for a fixed scope and date upfront.** Explain the trade-offs, define a minimum viable scope, fix the date, and flex lower-priority scope. Consider a hybrid.

**Interview**
1. **When would you use Agile instead of waterfall?** *Sample:* "When requirements are uncertain and customer feedback is valuable. I'd use waterfall when scope is stable and change is costly, and hybrid when a contract is fixed but details evolve."
2. **What is your role as PM in a Scrum team?** "I don't replace the Scrum roles. I support by managing stakeholders, risks, dependencies, and budget, and removing obstacles."
3. **Tell me about a sprint that missed its goal.** *Sample (STAR):* "A vendor dependency delayed us. We showed honest results at the review, found root causes in the retro, split the oversized story, and used actual velocity to reset the forecast."
4. **How do you handle scope change in a sprint?** "New requests go to the backlog. Scope under the Sprint Goal can be renegotiated between the PO and Developers. The goal stays stable."
5. **With a development background, how do you avoid micromanaging?** "I trust the Developers to decide how, focus on clarity of goals, risks, and impediments, and ask questions rather than prescribe solutions."

### Revision Checklist
- [ ] I can list Scrum roles, events, artifacts, and commitments
- [ ] I can say which practices are required and which are common
- [ ] I can write a user story with Given/When/Then criteria
- [ ] I can prioritize with MoSCoW and split large stories
- [ ] I can calculate velocity and forecast sprints
- [ ] I can read a burndown chart
- [ ] I can explain Kanban WIP limits and flow metrics
- [ ] I can say how an Agile PM differs from a Scrum Master and Product Owner

---

## 12. Case Studies (2 more of the 15)

### Case 9: A product backlog with competing priorities

| Element | Detail |
|---|---|
| Situation | Before Sprint 4: Maria wants loyalty points. Stylists want color-coded calendars. Tom wants a bookings report. Dev wants a week to clean up payment code. All say theirs is urgent. |
| Main problem | Too many "top priorities," and the team doesn't know what to build next |
| Root cause | No agreed prioritization criteria, and several people lobbying the team directly |
| Options | (a) Build whatever the loudest person asks, (b) split the sprint among everyone, (c) the PO orders the backlog using transparent criteria tied to the Product Goal |
| Recommended | (c) |
| Resolution steps | 1) Restate the Product Goal (60% online bookings). 2) Agree criteria: contribution to the goal, risk reduction, effort, dependencies. 3) Score each request. 4) Maria, as PO, orders the list. Loyalty points stay in Won't (this release). 5) Dev's cleanup is added as a small, visible backlog item because it reduces payment-bug risk. 6) Explain the order to all requesters. 7) Revisit after each Review. |
| Documentation | Updated product backlog (with MoSCoW and order), decision log |
| Communication | Message below. Share the ordered backlog on the board. |
| Expected outcome | Fewer side requests, shared understanding, team focus |
| Lessons | One accountable owner and visible criteria defuse competing priorities |
| Possible exam question | "Several stakeholders say their items are highest priority. What should happen?" Answer: the Product Owner orders the backlog using agreed criteria tied to the product goal |

> **Message to requesters:** "Thanks for your requests. We ordered the backlog by how much each item helps us reach 60% online bookings and reduces launch risk. Order for next sprint: payment deposit, payment cleanup, stylist time-off. Calendar colors and the bookings report are next in line, and loyalty points are planned for release 2. If something changes, we'll re-order at the next review."

### Case 10: A sprint that fails to achieve its goal

| Element | Detail |
|---|---|
| Situation | Sprint 3. **Goal:** customers can pay a deposit when booking. Committed: PB-05 (13) + PB-07 (5) = 18 points. At the end: PB-07 done (5), PB-05 not done. **Velocity: 5** (Sprints 1 and 2: 16 and 18). |
| Main problem | The Sprint Goal was missed |
| Root cause | 1) The payment sandbox arrived late (a dependency). 2) PB-05 was a 13-point story that should have been split. 3) The team committed to a full 18 despite the known vendor risk. |
| Options | (a) Extend the sprint, (b) cancel the sprint, (c) end it on time, show what's real, and learn |
| Recommended | (c). Sprints are fixed length, so extending breaks the rhythm. Cancelling is for a Sprint Goal that has become obsolete, and here the goal still matters. |
| Resolution steps | 1) Hold the Review honestly. Show PB-07 and the mock-payment progress. 2) Do **not** count PB-05 as done. 3) In the Retrospective, find the causes (5 Whys) and agree actions: split PB-05 into 05a "pay deposit using the mock provider" (5) and 05b "connect the live provider" (8); start dependency-heavy items only when the dependency is ready; consider smaller commitments when a vendor risk is open. 4) The PO re-orders the backlog. 5) Re-forecast with actual velocity. |
| Re-forecast | Done so far: 16 + 18 + 5 = 39 points. Average velocity = 13. Remaining Must + Should = PB-05 (13) + PB-08 (5) = **18 points**, which is 18 ÷ 13 = 1.4, so **2 sprints**. Remaining Could items = 16, so all remaining work = 34 points, which is 34 ÷ 13 = 2.6, so **3 sprints**. With Sprints 4 to 6 left and Sprint 6 reserved for hardening, UAT, and launch, only Sprints 4 and 5 are available for building. **Must + Should fits, Could items do not.** (Sprint 3 may have been an unusually low sprint, so the true velocity may be slightly higher. This is a conservative forecast.) |
| Documentation | Updated backlog and forecast, retrospective actions, risk register (vendor dependency) |
| Communication | Message below |
| Expected outcome | Honest forecast, a smaller risk of repeating the problem, and Maria choosing to defer the Could items |
| Lessons | Done means Done. Split large stories. Manage dependencies before committing |
| Possible exam question | "A team misses its Sprint Goal. What should happen to the Sprint?" Answer: it ends at its planned time; unfinished items return to the backlog for the PO to reorder; the team inspects causes in the Retrospective |

> **Message to sponsor:** "Maria, Sprint 3 did not reach its goal. The deposit payment isn't finished because the provider's sandbox arrived late and the story was too large. We delivered stylist time-off. We've split the payment work and re-forecast. We can still deliver all Must and Should items by Sprint 5, which leaves Sprint 6 for testing and launch. The Could items (calendar colors, report, SMS) won't fit unless velocity improves. Can we confirm that trade-off at tomorrow's review?"

---

## Part 6 Checkpoint Quiz

Try these **without looking back**:

1. Name the five Scrum events and the three artifacts with their commitments.
2. Name three practices that are common in Scrum teams but are **not** required by the Scrum Guide.
3. A team completes 14, 18, and 16 points in three sprints. 80 points remain. How many sprints are needed?
4. What is the difference between the Definition of Done and acceptance criteria?
5. A sprint burndown stays flat for a week, then drops to zero on the last day. What does this suggest, and what would you try?
6. A manager asks a developer to add urgent work in the middle of a sprint. What should happen?
7. Give one difference between Scrum and Kanban.
