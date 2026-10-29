# Part 2: Initiation and Project Scoping

**Source note:** As publicly described, Google's *Project Initiation* course covers goals, scope, the charter, stakeholders, risks, and team setup. Items marked **[Supplemental]** are my additions, such as PMBOK comparisons and extra templates. The tools, templates, and 60 questions are my original material, not official Google content.

---

## 1. Learning Objectives

By the end of Part 2 you should be able to:
- Define a project's goals, scope, and success criteria so they are measurable
- Write a business case and a project charter
- Identify, analyze, and prioritize stakeholders
- Build a RACI matrix (who does, who answers, who advises, who is informed)
- Control scope and handle change requests

**Running example: BrightCuts Salon.** The owner (**Maria Lopez**, the sponsor) wants an online booking app. Budget: **$30,000**. Target: **12 weeks**. You are the project manager.

---

## 2. How the Pieces Connect

```
Business problem → Business case → Goals (SMART) → Scope
       → Stakeholders agree → Charter signed → Planning begins
```

Initiation answers **"Should we do this, and what exactly are we promising?"** Every later document (schedule, budget, risk register) builds on what you define here.

---

## 3. Skill 1: Project Scoping

**Definition:** Agreeing on and documenting what the project will and will not deliver, including goals, deliverables, boundaries, constraints, assumptions, and success criteria.

**Why it matters:** Unclear scope is among the most common causes of rework, overruns, and disputes.

**When to use:** At initiation, and again whenever a major change is proposed.

**Step-by-step process**
1. Clarify the **problem** ("phone bookings take 15 hours a week and customers book after hours").
2. Interview key stakeholders about needs, not solutions.
3. Write **SMART goals** (specific, measurable, achievable, relevant, time-bound).
4. List **deliverables** (what will exist at the end).
5. Define **in scope** and **out of scope**.
6. Record **constraints, assumptions, dependencies**.
7. Define **acceptance criteria** (how we know a deliverable is done).
8. Get written **sign-off**.

**Tools and documents:** business case, project goals, scope statement, charter, requirements list.

**Common challenges and fixes**

| Challenge | Fix |
|---|---|
| Stakeholders describe solutions, not problems | Ask "What problem would that solve?" |
| Vague wording ("user-friendly") | Convert to measurable criteria ("a customer books in under 3 minutes") |
| No "out of scope" list | Write exclusions explicitly and have the sponsor sign them |

**Relationships:** Scoping feeds the **WBS** (Part 3), **risk identification**, and **change control**. Stakeholder analysis tells you whom to ask.

### SMART goals: worked example

| Letter | BrightCuts goal |
|---|---|
| Specific | Launch a web booking app for appointments and cancellations |
| Measurable | 60% of bookings made online within 3 months of launch |
| Achievable | Team of 3, proven tooling, $30,000 |
| Relevant | Reduces staff phone time, supports growth |
| Time-bound | Live within 12 weeks of project start |

### Template: Business Case (completed)

| Section | Content |
|---|---|
| Problem | Staff spend ~15 hrs/week on phone bookings; ~20% of calls missed |
| Proposed solution | Web-based booking app with calendar and reminders |
| Benefits | Save ~10 staff hrs/week; capture after-hours bookings; fewer no-shows via reminders |
| Costs | $30,000 build, $150/month hosting and support |
| Options considered | (1) Do nothing, (2) Buy off-the-shelf software with monthly fees, (3) Custom build |
| Recommendation | Custom build, because it fits salon-specific rules and avoids long-term license fees |
| Risks | Low adoption by customers; integration with payment provider |
| Success measure | 60% online bookings; no-show rate down from 12% to 6% |

### Template: Project Charter (completed)

| Field | Content |
|---|---|
| Project name | BrightCuts Online Booking App |
| Sponsor / PM | Maria Lopez / (you) |
| Purpose | Reduce phone workload and enable 24/7 booking |
| Goals | See SMART goals above |
| Deliverables | Customer web app, staff admin dashboard, email/SMS reminders, training guide |
| High-level scope | Booking, cancellation, reminders, staff calendar |
| Out of scope | Loyalty program, native mobile app, inventory management |
| Budget / timeline | $30,000 / 12 weeks |
| Key stakeholders | Owner, stylists, receptionist, customers, developer, payment provider |
| Assumptions | Owner provides service list and prices by week 1 |
| Constraints | Fixed budget; launch before holiday season |
| Major risks | Late vendor API; low customer adoption |
| Success criteria | Goals met, acceptance tests passed, staff trained |
| Approval | Signature and date of sponsor |

### Template: Project Scope Statement (completed)

| Section | Content |
|---|---|
| In scope | Online booking, cancellation, reminders, admin calendar, payment at booking |
| Out of scope | Loyalty points, mobile apps, multi-location support |
| Deliverables and acceptance | Booking flow: customer completes a booking in under 3 minutes in testing |
| Constraints | $30,000 cap; 12 weeks |
| Assumptions | Payment provider API ready by week 4 |
| Exclusions rule | Anything not listed in scope requires a change request |

---

## 4. Skill 4: Stakeholder Analysis

**Definition:** Identifying everyone affected by or able to affect the project, then assessing their influence, interest, expectations, and attitude to decide how to engage them.

**Why it matters:** Projects fail more from people problems than technical ones. A missed stakeholder can cause late objections.

**Step-by-step process**
1. **Identify** (brainstorm; ask "who else?" of everyone you interview).
2. **Analyze** each person's role, power, interest, expectations, attitude (supportive, neutral, resistant).
3. **Prioritize** using a power-interest grid.
4. **Plan engagement** (how often, what channel, who owns the relationship).
5. **Record** in a stakeholder register.
6. **Review** regularly, because stakeholders and attitudes change.

### Template: Stakeholder Register (completed)

| Stakeholder | Role | Main interest | Power | Interest | Attitude | Strategy |
|---|---|---|---|---|---|---|
| Maria Lopez | Sponsor | ROI, on-time launch | High | High | Supportive | Manage closely; weekly update |
| Receptionist (Tom) | Daily admin user | Easy tool, less stress | Low | High | Neutral, worried | Keep informed; involve in testing |
| Stylists | Calendar users | Control over their schedules | Medium | High | Mixed | Consult; demo early |
| Customers | End users | Fast, simple booking | Low | Medium | Unknown | Gather feedback via short survey |
| Developer | Builds app | Clear requirements | Medium | High | Supportive | Daily contact |
| Payment provider | External vendor | Correct integration | Medium | Low | Neutral | Monitor; confirm API dates |

### Power-Interest Matrix

```
              Low Interest        High Interest
High Power  | KEEP SATISFIED    | MANAGE CLOSELY
            | (payment provider)| (Maria)
Low Power   | MONITOR           | KEEP INFORMED
            | (landlord)        | (Tom, customers)
```

*Placement above is a simplified view of the register. Tools may place stakeholders differently, and that's fine if you can justify it.*

### Template: RACI Matrix (completed)

**R** = Responsible (does the work), **A** = Accountable (final answer, one per task), **C** = Consulted (two-way input), **I** = Informed (one-way updates).

| Task | Maria (Sponsor) | PM | Developer | Receptionist | Stylists |
|---|---|---|---|---|---|
| Approve charter | A | R | I | I | I |
| Define booking rules | A | R | C | C | C |
| Build booking flow | I | A | R | C | I |
| User acceptance testing | A | R | C | R | R |
| Staff training | I | A | C | R | R |

**Rule:** Each row has exactly **one A**.

**Common challenges and fixes**

| Challenge | Fix |
|---|---|
| Hidden stakeholder appears late | Ask every interviewee "Who else should I talk to?" |
| Resistant high-power stakeholder | Understand their concern first, then involve them in decisions |
| Too many "A"s on a task | Reduce to one accountable person |

**Relationships:** The stakeholder register feeds the **communication plan** (Part 4), **risk register** (people risks), and **RACI**.

---

## 5. Skill 5: Scope Management

**Definition:** Making sure the project includes all the work required, and only that work, from planning scope through validating and controlling it.

**Process**
1. **Plan** how scope will be defined, validated, and controlled.
2. **Collect requirements** (interviews, surveys, observation, user stories).
3. **Define scope** (scope statement).
4. **Create the WBS** (Part 3).
5. **Validate** deliverables with the customer (formal acceptance).
6. **Control** scope using a change process.

### Change control process (use this every time)

1. Someone raises a **change request**.
2. PM logs it and **assesses impact** on schedule, cost, quality, risk.
3. Present **options** to the decision-maker (approve, reject, defer, trade off).
4. **Decide** and document.
5. **Update** plans and **communicate**.

### Template: Change Request Log (completed)

| ID | Date | Requester | Description | Impact | Decision | Owner |
|---|---|---|---|---|---|---|
| CR-001 | Wk 5 | Maria | Add loyalty points | +3 weeks, +$4,500 | Deferred to phase 2 | PM |
| CR-002 | Wk 6 | Stylists | Color-code calendar by stylist | +2 days, no cost | Approved, absorbed | Developer |

**Memorize:** Scope creep is *uncontrolled* growth. A *managed* change is not scope creep. **[Supplemental]** PMBOK calls verification "Validate Scope" (customer acceptance) and "Control Quality" (internal checking). Don't confuse them.

---

## 6. Common Mistakes

| Mistake | How to avoid |
|---|---|
| Starting work without a charter | Write a one-page charter fast |
| Goals not measurable | Apply the SMART test |
| No out-of-scope list | Write exclusions and get them signed |
| Treating stakeholders as one group | Analyze individually |
| Saying yes to changes instantly | Assess impact first |
| Verbal approvals | Get written sign-off |

## 7. Module Summary and Revision Notes

- Initiation justifies and authorizes the project (business case, charter).
- SMART goals make success measurable.
- Scope = work included **and excluded**.
- Stakeholder analysis: identify, analyze, prioritize, engage.
- RACI: one **A** per task.
- Change control: log, assess, decide, update, communicate.

---

## 8. Skill-by-Skill Question Sets

*Brief explanations are included. The full 10-field format (difficulty, distractor analysis, takeaway) is used for the numbered bank in Part 8.*

### Skill 1: Project Scoping

**Beginner**
1. **What is a project's scope?** The work included to deliver the result, plus what is excluded. *Why:* it sets boundaries both sides agree to.
2. **What does the "M" in SMART stand for?** Measurable. *Why:* without measurement, you can't prove success.
3. **What is a deliverable?** A tangible or verifiable output, such as the admin dashboard.
4. **Why list out-of-scope items?** They prevent assumptions and later disputes.
5. **True or false: scope is set once and never changes.** False. It can change through controlled change requests.

**Intermediate**
1. **Rewrite "Make the app fast" as measurable.** "Pages load in under 2 seconds for 95% of requests." *Why:* testable criteria avoid arguments.
2. **Difference between a goal and a deliverable?** A goal is the desired outcome (60% online bookings); a deliverable is an output (the app).
3. **Where do assumptions belong?** In the charter or scope statement and an assumption log. *Why:* unverified assumptions become risks.
4. **What is an acceptance criterion?** A condition a deliverable must meet to be accepted, for example "A customer can cancel a booking up to 2 hours before."
5. **Which is a constraint: "Budget cannot exceed $30,000" or "Client will send photos by Friday"?** The budget cap is a constraint. The photos statement is an assumption.

**Scenario**
1. **The sponsor says "Build something modern like Airbnb." What do you do?** Ask what problem it solves and which features matter, then turn answers into measurable scope. *Reasoning:* translate preferences into requirements.
2. **Two stakeholders give conflicting requirements.** Facilitate a discussion with the sponsor as tiebreaker, document the decision. *Reasoning:* conflicts are resolved by someone with authority.
3. **Midway, nobody can recall what "booking" includes.** The scope statement was too vague. Clarify, update, and re-sign it. *Reasoning:* fix the document, not the memory.
4. **A vendor assumes your project includes data migration.** Check the scope statement. If it's absent, issue a clarification or change request. *Reasoning:* the signed scope is the reference.
5. **The deadline is fixed but scope keeps growing.** Show the trade-off using the triple constraint and ask the sponsor to prioritize. *Reasoning:* something has to give.

**Interview**
1. **How do you define scope for a new project?** *Sample:* "I start with the business problem, interview stakeholders, write measurable goals, then list deliverables and exclusions. I get written sign-off before planning. On a booking app I built, exclusions like mobile apps prevented later disputes."
2. **Tell me about a time scope was unclear.** *Sample (STAR):* "Situation: requirements were vague. Task: define scope in two weeks. Action: ran stakeholder workshops, wrote acceptance criteria. Result: signed scope and zero major disputes."
3. **How do you prevent scope creep?** "A clear scope statement, a change process, and impact assessments with options for decision-makers."
4. **How do you write measurable goals?** "I apply SMART and ask 'How will we know?' until a number or test emerges."
5. **What goes in a charter?** "Purpose, goals, scope, deliverables, budget and timeline, stakeholders, assumptions, constraints, risks, and sponsor approval."

### Skill 4: Stakeholder Analysis

**Beginner**
1. **Define stakeholder.** Anyone affected by or able to affect the project.
2. **Name the two axes of the power-interest grid.** Power (or influence) and interest.
3. **What goes in a stakeholder register?** Names, roles, interests, influence, attitude, engagement strategy.
4. **What does the "A" in RACI mean?** Accountable, the single owner of the outcome.
5. **True or false: only internal people are stakeholders.** False. Customers, vendors, and regulators count.

**Intermediate**
1. **Strategy for high power, low interest?** Keep satisfied. *Why:* they can block you but don't want detail.
2. **Strategy for low power, high interest?** Keep informed. They care, but cannot decide.
3. **Difference between Responsible and Accountable?** Responsible does the work; Accountable answers for it. Only one A per task.
4. **Why revisit the register?** Interests and influence change as the project progresses.
5. **What does "Consulted" mean?** Two-way input before decisions, in contrast to "Informed," which is one-way.

**Scenario**
1. **A department head you never identified objects at week 8.** Meet them to understand concerns, add them to the register, assess impact, and update the plan. *Reasoning:* listen, assess, adjust, and then prevent a repeat by asking "who else?"
2. **The receptionist is resisting the new app.** Ask why, involve her in design and testing, and offer training. *Reasoning:* resistance often reflects unaddressed concerns.
3. **Sponsor wants daily updates; others want weekly.** Tailor frequency by stakeholder in the communication plan.
4. **Two people claim they're Accountable.** Clarify with the sponsor and update the RACI so each task has one A.
5. **An influential stylist is publicly critical.** Meet privately, address concerns, and consider giving her a pilot role. *Reasoning:* turn a critic into a contributor.

**Interview**
1. **How do you identify stakeholders?** "Brainstorm with the sponsor, review org charts, and ask every interviewee who else should be involved."
2. **Describe handling a resistant stakeholder.** *Sample:* "A manager worried about workload. I listened, adjusted the rollout, and involved him in testing. He became a champion."
3. **How do you prioritize stakeholders?** "A power-interest grid, then I tailor engagement."
4. **How do you keep stakeholders aligned?** "A communication plan, regular updates, and confirmation of decisions in writing."
5. **What is RACI and why use it?** "It clarifies roles for each task so nothing falls through the cracks or gets duplicated."

### Skill 5: Scope Management

**Beginner**
1. **What is scope creep?** Uncontrolled additions to scope.
2. **What is a change request?** A formal proposal to alter scope, schedule, or budget.
3. **Why log change requests?** For traceability and decisions.
4. **Who usually approves scope changes?** The sponsor or a change control board, depending on the project.
5. **What is "out of scope"?** Work explicitly not included.

**Intermediate**
1. **First step on receiving a change request?** Record it and assess impact before responding.
2. **Difference between scope creep and an approved change?** Creep is uncontrolled; an approved change follows the process.
3. **What is scope validation?** Formal customer acceptance of deliverables **[Supplemental: PMBOK term]**.
4. **Three ways to handle a change when the budget is fixed?** Add budget, extend time, or remove other scope.
5. **Why get written approval for changes?** To avoid disputes and keep records.

**Scenario**
1. **Client requests a feature after approval.** Log it, estimate the impact, present options, and get a documented decision. *Reasoning:* approval doesn't prohibit change, only uncontrolled change.
2. **Developer adds a "nice extra" without asking.** This is **gold plating**. Remove or review it and remind the team that extras need approval.
3. **A small change takes five minutes.** Still log it, because small changes accumulate.
4. **The sponsor insists on a change with no extra time.** Show the trade-offs and ask the sponsor to choose. Document the decision either way.
5. **Customers reject a deliverable that met the signed criteria.** Compare against the criteria. If it passes, explain; if the need changed, raise a change request.

**Interview**
1. **How do you manage scope changes?** "I log, assess impact, present options, get a documented decision, and update the plan."
2. **Example of scope creep you handled?** *Sample:* "A client kept adding reports. I quantified each addition's cost, then we agreed on a phase 2 for them."
3. **How do you say no to a sponsor?** "I don't say no. I show the impact and offer trade-offs."
4. **What is gold plating?** "Adding unrequested features. It wastes time and adds risk."
5. **How do you keep requirements traceable?** "A requirements list linked to deliverables and acceptance criteria."

### Revision Checklist
- [ ] I can write a SMART goal
- [ ] I can fill in a charter and scope statement
- [ ] I can build a stakeholder register and power-interest matrix
- [ ] I can create a RACI with one A per task
- [ ] I can run the change control steps from memory

---

## 9. Case Studies (3 of the 15; the rest follow in later parts)

### Case 1: Unclear scope

| Element | Detail |
|---|---|
| Situation | The owner asks for "an app like our competitor's." No list of features exists. |
| Main problem | Undefined deliverables |
| Root cause | Initiation skipped detailed scoping |
| Options | (a) Start building and adjust, (b) run requirements workshop first, (c) split into discovery phase and build |
| Recommended | (c), a two-week discovery with fixed output: scope statement and prioritized features |
| Resolution steps | Interview staff and customers, write user stories, rank with MoSCoW (must, should, could, won't), draft scope statement, get sign-off |
| Documentation | Requirements list, scope statement, charter update |
| Communication | Share a one-page summary; confirm by email |
| Outcome | Agreed scope; reduced rework risk |
| Lessons | Never estimate without defined scope |
| Possible exam question | "What should the PM do first when requirements are vague?" Answer: clarify and document scope with stakeholders |

### Case 2: A stakeholder who frequently changes requirements

| Element | Detail |
|---|---|
| Situation | Maria changes the booking rules weekly. |
| Main problem | Rework and schedule slips |
| Root cause | No change process; decisions not documented |
| Options | Accept all, refuse all, or introduce change control |
| Recommended | Introduce a lightweight change process and a weekly decision meeting |
| Resolution steps | Explain the cost of change with data, create the change log, batch requests weekly, show impact on timeline |
| Documentation | Change request log, updated schedule |
| Communication | Frame it as protecting her launch date. Example: "Each change takes about 3 days. Which would you like first?" |
| Outcome | Fewer, more considered changes |
| Lessons | Visible impact changes behavior |
| Possible exam question | "How do you handle repeated changes?" Answer: formal change control with impact assessment |

### Case 11: Client requests changes after approval

| Element | Detail |
|---|---|
| Situation | After design sign-off, the client wants a new homepage layout. |
| Main problem | Change affects baseline |
| Root cause | The client sees the design differently now that it's concrete |
| Options | Reject, accept silently, or process as a change |
| Recommended | Process as a change request |
| Resolution steps | Log it, estimate (+4 days, +$1,200), present options (accept with new cost, defer, or choose a smaller tweak), document decision |
| Documentation | Change log, updated schedule and budget baseline |
| Communication | Confirm the decision in writing to all affected parties |
| Outcome | Client chooses a smaller tweak within the buffer |
| Lessons | Approval is a baseline, not a freeze |
| Possible exam question | "After approval, the client asks for a change. What next?" Answer: assess impact and use change control |

---