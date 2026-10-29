# Part 5: Execution, Quality, and Change Management

**Source note:** As publicly described, Google's *Project Execution* course covers tracking and reporting progress, quality management, change management, leadership, and closing. I haven't re-checked Coursera live, so confirm the current contents there. **[Supplemental]** marks my additions (cost of quality, PDCA, ADKAR, PMBOK terms). Templates, numbers, and questions are my original material, not official Google content.

This part covers Skills 8, 9, 10, 11, 12, and 15. Skills 10 to 12 overlap a lot, so I separate them as follows: **assessment** measures, **management** plans and improves, and **assurance** protects the process.

---

## 1. Learning Objectives

By the end of Part 5 you should be able to:
- Run the executing phase: track work, report status, and manage issues and decisions
- Use variances and RAG (Red-Amber-Green) status to decide when to take action
- Plan quality, assess deliverables, and separate quality assurance from quality control
- Find root causes with the 5 Whys, fishbone diagrams, and Pareto analysis
- Run project change control and help people through organizational change

**Running example:** BrightCuts Online Booking App, now in weeks 6 to 10, with development under way and system testing starting.

---

## 2. How the Pieces Connect

```
Baseline (plan) → Do the work (Skill 8) → Measure vs baseline (Skill 9)
                         ↓                          ↓
        Quality plan (11) → Assure process (12) → Assess product (10)
                         ↓                          ↓
          Variance or defect found → Root cause → Corrective action
                         ↓
         Baseline affected? → Change control (Skill 15) → Update plan
```

Execution produces work. Monitoring compares it to the baseline. Quality activities check that the work is *right*, not just *done*. When any of this shows the baseline must change, change management makes the change deliberate instead of accidental.

---

## 3. Skill 8: Project Implementation

**Definition:** Carrying out the approved plan: coordinating people and resources, producing deliverables, managing issues and decisions, and keeping stakeholders engaged.

**Why it matters:** Most of the budget is spent here. A good plan fails if execution is uncoordinated.

**When to use:** From kickoff until the deliverables are complete.

**Step-by-step process**
1. **Launch:** confirm the baseline, roles, and team agreement.
2. **Assign** work packages with clear done criteria.
3. **Coordinate:** stand-ups, a shared task board, dependency checks.
4. **Produce and review** deliverables against acceptance criteria.
5. **Manage issues:** log, assign an owner, set a due date, resolve or escalate.
6. **Record decisions** so they aren't re-argued.
7. **Engage stakeholders** per the communication plan.
8. **Manage vendors:** track delivery dates and quality.
9. **Report** status on a regular rhythm.

### Template: Issue Log (completed)

| ID | Date | Issue | Priority | Owner | Action | Due | Status |
|---|---|---|---|---|---|---|---|
| I-01 | Wk 5 | Payment sandbox not delivered | High | Dev | Use mock API; escalate to vendor account manager | Wk 6 | Open |
| I-02 | Wk 6 | Booking rules unclear for partial payments | High | PM | Get Maria's decision | Wk 6 | Closed |
| I-03 | Wk 7 | Test server slow | Medium | Dev | Upgrade hosting tier | Wk 8 | In progress |

### Template: Decision Log (completed)

| Date | Decision | Made by | Reason | Impact |
|---|---|---|---|---|
| Wk 6 | Defer SMS reminders to phase 2 (email only) | Maria | Saves ~$2,000 and 3 days | Scope reduced via CR-003 |
| Wk 6 | Allow bookings up to 60 days ahead | Maria | Matches salon demand | None |

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| "90% done" for weeks | Break tasks into small pieces with objective done criteria |
| Tracker is out of date | Update it during stand-up, not as extra paperwork |
| Decisions forgotten or disputed | Decision log, shared and dated |
| Blockers stay hidden | Ask "What's blocking you?" daily, and thank people for raising them |
| Team overloaded | Check capacity weekly and rebalance |

**Relationships:** Implementation delivers the **WBS** work, feeds **monitoring** (Skill 9), uses the **communication plan**, and generates **issues**, **risks**, and **change requests**.

---

## 4. Skill 9: Project Management (Monitoring, Controlling, and Reporting)

**Definition:** Continuously comparing actual progress, cost, quality, and risk against the baseline, then taking action when results drift. In Google's framing this runs *within* execution. **[Supplemental]** PMBOK treats "Monitoring and Controlling" as its own process group.

**Why it matters:** Early detection of drift gives you more and cheaper options.

### The monitoring cycle
1. **Collect** actual data (task status, hours, costs, test results).
2. **Compare** with the baseline (variances, CPI, SPI, critical path).
3. **Analyze** causes and forecast (EAC, trend).
4. **Decide** on action: corrective action, change request, or escalate.
5. **Report** to stakeholders.
6. **Repeat** weekly.

**Leading vs. lagging indicators:** *Lagging* tells you what already happened (actual cost, finished tasks). *Leading* hints at what's coming (rising defect rate, risk triggers, slipping task dates, falling team morale).

**Thresholds (example only; organizations set their own):**

| Status | Meaning | Example rule |
|---|---|---|
| **Green** | On track | CPI and SPI ≥ 0.95 |
| **Amber** | At risk; manageable | 0.85 to 0.94 |
| **Red** | Off track; needs decision | < 0.85 |

**Caution:** SV is measured in money and ignores the critical path. A negative SV on a task with plenty of slack may not threaten the launch. Check the critical path as well as the indices.

### Template: Weekly Status Report (completed, Week 7)

| Section | Content |
|---|---|
| **Overall** | **AMBER**: launch achievable with agreed scope trim |
| Scope | Green. CR-003 approved (SMS deferred) |
| Schedule | Amber. Booking flow 1 week late on critical path |
| Budget | Amber. See metrics below |
| Quality | Green. Peer reviews done on booking flow |
| Risks | R1 payment API (High): mock in use, sandbox arrived 8 days late. R3 changes: 1 request this week |
| Accomplished | Admin dashboard 60% complete. Payment mock integrated |
| Next week | Finish booking flow. Start system testing on completed modules |
| Decisions needed | Approve an extra $1,000 (or accept a launch date one week later) |

**Metrics at end of week 7:** BAC $30,000, PV $17,500, EV $14,400, AC $16,000.
- CV = 14,400 − 16,000 = **−$1,600** (over budget)
- SV = 14,400 − 17,500 = **−$3,100** (behind)
- CPI = 14,400 ÷ 16,000 = **0.90**
- SPI = 14,400 ÷ 17,500 ≈ **0.82**
- EAC (current performance continues) = 30,000 ÷ 0.90 ≈ **$33,300**. The approved SMS deferral saves about $2,000, so the forecast is roughly **$31,300**.

**Plain English:** We get 90 cents of value per dollar and are progressing at about 82% of the planned pace. Without action we'd finish about $3,300 over, and the scope trim reduces the gap to about $1,300.

### Sample dialogue: status "green" but the team is worried

> **PM:** "The tracker shows green, but I'm hearing concern. Help me understand what's really happening."
> **Dev:** "The booking flow is 'done' but it hasn't been tested. I think it's riskier than it looks."
> **PM:** "Thanks. I'll mark it 'built, not verified' and move testing earlier. Better to show amber than a green that turns red next week."

Status that looks green outside but is red inside is sometimes called a *watermelon* status. Defend against it by checking objective evidence, not just opinions.

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Reports are long and unread | One page: status, forecast, top risks, decisions needed |
| Status based on gut feeling | Tie it to measures: done criteria, variances, test results |
| Spending is mistaken for progress | Check EV. Money spent isn't work completed |
| Action only when red | Set amber triggers and act early |
| Bad news delayed | Report it with options, as early as possible |

**Relationships:** Monitoring uses the **baseline** (Part 3), the **risk register**, and **quality** results. It triggers **change requests** and **escalation** (Part 4).

---

## 5. Skill 10: Project Quality Assessment

**Definition:** Measuring whether deliverables and project processes meet the agreed standards and acceptance criteria, using inspection, testing, review, and audit.

**Why it matters:** Defects found late are expensive to fix. Assessment gives evidence for acceptance, not opinions.

**Common methods**

| Method | What it is | BrightCuts example |
|---|---|---|
| **Inspection / review** | Examine work without running it | Peer review of the booking code; design walkthrough |
| **Testing** | Run it and compare to expected results | Book, cancel, and pay in a test environment |
| **Audit** | Independent check against process or standards | Review of data-protection practices |
| **User acceptance testing (UAT)** | Real users check it meets their needs | Tom and stylists test daily tasks |
| **Metrics review** | Check numbers against targets | Page load time, defects found |

**Defect basics:** *Severity* = how bad the effect is. *Priority* = how soon to fix it. They can differ: a typo on the homepage has low severity but may be high priority for a launch demo.

**Regression testing:** re-running earlier tests after a fix to confirm nothing else broke.

### Template: Defect Log (completed)

| ID | Description | Severity | Found in | Owner | Status |
|---|---|---|---|---|---|
| D-14 | Two customers can book the same slot | Critical | System test | Dev | Fixed, retest |
| D-15 | Payment fails when card has special characters | High | System test | Dev | Open |
| D-16 | Reminder email shows wrong time zone | Medium | System test | Dev | Open |
| D-17 | Button label misspelled | Low | UAT | Priya | Closed |

### Worked numerical examples **[Supplemental]**

**Test pass rate** = tests passed ÷ tests run × 100. 34 passed of 40 → **85%**. Plain English: 6 tests need attention before acceptance.

**Defect density** = defects ÷ size. 50 defects across 25 features → **2 per feature**. Useful for comparing modules.

**Pareto analysis** (the 80/20 idea: a few causes produce most defects). System test found 50 defects:

| Category | Defects | % of total | Cumulative % |
|---|---|---|---|
| Payment errors | 20 | 40% | 40% |
| Calendar sync | 14 | 28% | 68% |
| Email reminders | 8 | 16% | 84% |
| UI layout | 5 | 10% | 94% |
| Other | 3 | 6% | 100% |

**Plain English:** Payment and calendar issues cause 68% of defects, and adding reminders brings it to 84%. Fix the biggest categories first for the most improvement. Pareto is a guide, not a law, and the exact 80/20 split rarely appears.

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Testing squeezed at the end | Test early and continuously; use risk-based prioritization |
| Acceptance criteria vague | Write measurable criteria at scoping |
| Only testers check quality | Everyone owns quality: reviews, definition of done |
| All defects treated equally | Rank by severity and business impact |
| Retest skipped after fixes | Include regression testing in the plan |

**Relationships:** Assessment checks the deliverables against **scope** acceptance criteria, produces data for **monitoring**, and feeds **root-cause analysis** and **lessons learned**.

---

## 6. Skill 11: Quality Management

**Definition:** The overall approach to planning, assuring, controlling, and improving quality so deliverables satisfy requirements and are fit for their purpose.

**Four connected activities**

| Activity | Question it answers | Timing |
|---|---|---|
| **Quality planning** | What does "good" mean here, and how will we achieve and check it? | Planning |
| **Quality assurance** | Are we following processes that prevent defects? | Throughout |
| **Quality control** | Do the deliverables meet the criteria? | During and at the end of work |
| **Continuous improvement** | How do we get better? | Throughout, especially retrospectives |

**Prevention vs. detection:** Prevention builds quality in (clear criteria, reviews, training). Detection finds defects after they exist (testing). Prevention is generally cheaper.

**Cost of quality [Supplemental]**

| Category | Meaning | BrightCuts example |
|---|---|---|
| Prevention | Costs to avoid defects | Training, code standards, design reviews |
| Appraisal | Costs to find defects | Testing, inspections |
| Internal failure | Defects found before delivery | Rework after system test |
| External failure | Defects found by customers | Double-booking in live use, refunds, reputation damage |

**Plain English:** Spending a little on prevention and appraisal usually costs far less than failures found by customers.

**Quality versus grade [Supplemental]:** *Grade* is the category or feature level (a basic vs. premium booking app). *Quality* is how well the product meets requirements for its grade. A basic app can be high quality. A feature-rich app can be low quality if it's full of defects.

**PDCA (Plan-Do-Check-Act) [Supplemental]:** a simple improvement loop: plan a change, try it, check results, adopt or adjust.

### Template: Quality Management Plan (completed)

| Section | Content |
|---|---|
| Quality objectives | Zero critical defects at launch; page load under 2 seconds for 95% of requests; booking completed in under 3 minutes |
| Standards | Acceptance criteria per deliverable; accessibility and data-protection basics; team coding standards |
| Definition of done | Reviewed, tested, merged, documented |
| Prevention activities | Peer review of all payment and booking code; design walkthrough with stylists |
| Assessment activities | Unit tests, system tests, UAT with 5 users |
| Metrics | Test pass rate (target ≥ 95%), defects by severity, response time, user task success |
| Roles | Dev: code reviews. Sam: test execution. PM: quality reviews. Maria: acceptance |
| Defect handling | Log, rank by severity, fix, retest, regression test |
| Improvement | Retrospective after each phase; lessons learned log |

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Quality seen as extra cost | Show cost of failure vs. cost of prevention |
| No agreed standard | Define acceptance criteria and definition of done early |
| Gold plating (adding unrequested extras) | Build to criteria; extras go through change control |
| Metrics that don't matter | Choose measures linked to what stakeholders value |
| Quality sacrificed under pressure | Trade scope or time, not hidden quality |

**Relationships:** The quality plan comes from the **scope** acceptance criteria and **stakeholder** expectations, includes **risk** (quality risks), and is delivered through **QA** and **assessment**.

---

## 7. Skill 12: Quality Assurance

**Definition:** Making sure the *processes* used to create deliverables are sound and being followed, so defects are prevented. Quality assurance (QA) is **process-focused and preventive**. Quality control (QC) is **product-focused and detective**.

| | Quality assurance | Quality control |
|---|---|---|
| Focus | Process | Product |
| Aim | Prevent defects | Detect defects |
| Timing | Throughout | Once work is produced |
| Examples | Process audits, standards, checklists, training, review procedures | Testing, inspection, measuring results |
| BrightCuts | "All payment code gets a second reviewer" | "Run 40 test cases on the booking flow" |

**[Supplemental] Terminology trap:** In PMBOK language, assurance is "Manage Quality" and control is "Control Quality." In many **software companies, "QA" means testing**, which is quality *control* in project management terms. If you have a development background, expect this mix-up in exams and interviews. State clearly which meaning you use.

### Root-cause analysis tools

**5 Whys:** ask "why?" repeatedly until you reach a cause you can fix (often around five times, not a strict rule).

| Why | Answer |
|---|---|
| Why did two customers book the same slot? | Two bookings were saved at nearly the same moment |
| Why was that allowed? | The system didn't lock the slot while payment was in progress |
| Why wasn't it locked? | Concurrent booking behavior was not in the requirements |
| Why not? | Requirements were gathered by interview only, and no scenario review was held |
| Why no review? | Scenario review wasn't part of our quality checklist |

**Root cause:** a process gap (no scenario-based requirements review), not just a coding mistake.

**Fishbone (Ishikawa) diagram:** groups possible causes by category. Example for "double bookings":

```
People ───────┐           Process ──────┐
 Rushed code   │            No scenario   │
 review        ├──────────  review       ├──────►  DOUBLE
Tools ────────┤           Environment ──┤         BOOKINGS
 No load test  │            Test data     │
               │            too simple    │
Requirements ──┘           Measurement ───┘
 Concurrency                No concurrency
 not stated                 test cases
```

**Actions:**
- **Corrective action:** fixes the *cause* of a problem that has happened (add slot locking; add concurrency tests).
- **Preventive action:** reduces the chance of a *potential* problem (add scenario reviews to the checklist for all future features).
- **Defect repair:** fixes the faulty item itself (correct the bug).

### Template: QA and QC Checklist (completed)

| # | Check | Type | Done? |
|---|---|---|---|
| 1 | Acceptance criteria written for each deliverable | QA | ✔ |
| 2 | Payment and booking code peer-reviewed | QA | ✔ |
| 3 | Process audit: is the definition of done being used? | QA | ☐ |
| 4 | Unit tests passing | QC | ✔ |
| 5 | System test: ≥ 95% pass, no critical defects | QC | ☐ |
| 6 | UAT: 5 users complete a booking in under 3 minutes | QC | ☐ |
| 7 | Defects logged, ranked, and closed or deferred with approval | QC | ☐ |
| 8 | Lessons recorded | QA | ☐ |

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Process steps skipped when rushed | Make the key steps part of the definition of done |
| Blame culture around defects | Focus on root causes in the process |
| Audit becomes a paper exercise | Audit for learning; fix the findings |
| Same defect keeps returning | Add preventive actions, not just repairs |
| Over-bureaucratic process | Keep checks proportional to risk |

**Relationships:** Assurance protects the **plan**, uses the **team agreement** (Part 4), produces process evidence for **assessment**, and feeds **continuous improvement** and **lessons learned**.

---

## 8. Skill 15: Change Management

Two meanings appear in project work. Keep them distinct.

| | Project change control | Organizational change management |
|---|---|---|
| Focus | Controlling changes to scope, schedule, cost, and other baselines | Helping people adopt new ways of working |
| Question | "Should we approve this change?" | "Will people actually use it?" |
| Tools | Change request, change log, change control board | Communication, training, involvement, reinforcement |
| BrightCuts | Maria asks for loyalty points | Tom and the stylists must change how they take bookings |

**Why it matters:** Uncontrolled change causes scope creep, budget overruns, and confusion. Unmanaged people-side change causes low adoption, so a "successful" project delivers little value.

### Project change control

1. **Raise** a change request (form or log), including from the team or vendors.
2. **Log** it. Even small changes are recorded.
3. **Assess impact** on scope, schedule, cost, quality, risk, and resources.
4. **Review** by the decision-maker (sponsor or **change control board (CCB)**, the group authorized to approve or reject changes).
5. **Decide:** approve, reject, defer, or request more information.
6. **Implement** and update baselines, plans, and registers.
7. **Communicate** the decision to everyone affected.
8. **Verify** the change delivered what was intended.

**Thresholds:** many organizations let the PM approve small changes (for example, under 2 days and no cost) and require sponsor or CCB approval above that. Agree on this early.

**Urgent changes:** use an *expedited* process: fast impact assessment, a named person with authority to approve within hours, and full documentation immediately afterward. Urgent does not mean undocumented.

### Template: Change Request Form (completed)

| Field | Content |
|---|---|
| ID / date | CR-004 / Week 9 |
| Requested by | PM (due to payment provider notice) |
| Description | Migrate payment integration to provider's new API version |
| Reason | Old version will be switched off two weeks after planned launch |
| Impact: scope | One extra integration task |
| Impact: schedule | +4 days on the critical path (absorbed with buffer; launch date unchanged if approved by Friday) |
| Impact: cost | +$1,500 |
| Impact: risk / quality | Adds retest of payments; lowers long-term failure risk |
| Options | (1) Migrate now, (2) Launch on old version and migrate later, (3) Switch provider |
| Recommendation | Option 1 |
| Decision / date / approver | Approved, Week 9, Maria |
| Baseline updates | Schedule, budget, risk register, test plan |

### Organizational change (people side)

**ADKAR [Supplemental]:** a widely used model of what an individual needs to change.

| Letter | Meaning | BrightCuts action |
|---|---|---|
| **A**wareness | Why change is needed | Explain phone-time savings to staff |
| **D**esire | Wanting to take part | Show benefits: fewer missed calls, easier schedules |
| **K**nowledge | How to change | Training sessions and quick guides |
| **A**bility | Being able to do it | Practice time, a helper during launch week |
| **R**einforcement | Making it stick | Celebrate early wins; check in after 30 days |

Another well-known approach is Kotter's 8-step model **[Supplemental]**. The common thread is the same: explain the why, involve people, support them, and reinforce.

### Template: Change Management Plan (completed)

| Section | Content |
|---|---|
| Purpose | Control changes to the BrightCuts baseline and support staff adoption |
| Roles | Maria: approves changes over 2 days or $500. PM: assesses and logs. Dev: estimates effort |
| Process | Raise → log → assess → decide → implement → communicate → verify |
| Thresholds | Under 2 days, no cost: PM approves. Above: Maria. Emergency: Maria approves within 24 hours |
| Documents | Change request form, change log, updated baselines |
| Communication | Decisions emailed to affected people within 1 working day |
| People-side plan | Demo every 2 weeks, hands-on training in week 11, super-user (Tom), 30-day review |
| Success measures | 100% of changes logged. Staff using app for 80% of bookings by month 1 |

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Changes requested informally | Politely log every request and answer with impact |
| Approved change not shared | Update baselines, notify everyone, control document versions |
| Change process too slow | Thresholds and expedited path for urgent changes |
| Staff resist | Listen, involve, train, reinforce |
| "Change fatigue" | Batch changes, explain priorities, avoid unnecessary change |

**Relationships:** Change control protects **scope** and **baselines**, uses **impact analysis** from the schedule, budget, and risk register, and is communicated per the **communication plan**. People-side change links to **stakeholder analysis** and **team leadership** (Part 4).

---

## 9. Common Mistakes (Execution, Quality, Change)

| Mistake | How to avoid |
|---|---|
| Reporting activity instead of progress | Report against done criteria and EV |
| Letting issues sit with no owner | Every issue: owner and due date |
| Testing only at the end | Review and test continuously |
| Confusing QA with QC | Process prevention vs. product detection |
| Fixing the bug but not the cause | Root-cause analysis plus preventive action |
| Approving changes verbally | Written request, impact, and decision |
| Ignoring the people side of change | Plan training, involvement, and reinforcement |
| Cutting quality silently to save time | Make trade-offs visible to the sponsor |

---

## 10. Module Summary and Revision Notes

- **Execution** turns the baseline into deliverables. Track issues, decisions, and status.
- **Monitoring** compares actual vs. plan: CV, SV, CPI, SPI, EAC, critical path. Act at amber, not just red.
- **Quality assessment** uses inspection, testing, audit, UAT, and metrics. Severity ≠ priority.
- **Quality management** = plan, assure, control, improve. Prevention is cheaper than failure.
- **QA = process, preventive. QC = product, detective.** Beware the software-industry use of "QA."
- **Root cause tools:** 5 Whys, fishbone, Pareto.
- **Corrective** (fix the cause), **preventive** (avoid a potential problem), **defect repair** (fix the item).
- **Change control:** log, assess, decide, implement, communicate, verify. **Change management (people):** ADKAR.
- Urgent changes still need documentation.

---

## 11. Skill-by-Skill Question Sets

*Brief explanations are included. The full 10-field format appears in the numbered bank in Part 8.*

### Skill 8: Project Implementation

**Beginner**
1. **What happens during execution?** The team does the planned work while the PM coordinates, tracks, and communicates.
2. **What is an issue log?** A record of current problems with owner, priority, due date, and status.
3. **What is a decision log for?** It records decisions, who made them, and why, so they aren't re-argued.
4. **True or false: the PM does most of the project work.** False. The PM coordinates and enables the team.
5. **What is deliverable acceptance?** The customer's confirmation that a deliverable meets the agreed criteria.

**Intermediate**
1. **Why have a short daily stand-up?** It surfaces blockers and keeps the team aligned.
2. **What does a RAG status communicate?** A quick summary of health: Red, Amber, or Green.
3. **How do you avoid "90% done" reporting?** Use small tasks with objective done criteria.
4. **Why track vendor deliveries as milestones?** Vendor delays sit outside your control and can hit the critical path.
5. **What should an issue entry always have?** An owner and a due date.

**Scenario**
1. **The team doesn't update the tracker.** Make updates part of the stand-up, keep it simple, and model it. *Reasoning:* reduce friction, don't just demand compliance.
2. **A vendor misses a delivery date.** Log it as an issue, activate the contingency, and escalate with a recommendation.
3. **A stakeholder wants you to skip testing to hit the date.** Explain the risk, offer scope or schedule options, and document the sponsor's decision. *Reasoning:* quality trade-offs must be visible.
4. **Two urgent tasks need the same developer.** Prioritize by critical path and business value, with the sponsor deciding if needed.
5. **A task has been "almost done" for three weeks.** Split it into small items, find what blocks it, and re-estimate.

**Interview**
1. **How do you keep execution on track?** *Sample:* "Clear done criteria, a daily stand-up, a shared board, a weekly variance check, and an issue log with owners."
2. **Describe re-planning mid-project.** *Sample (STAR):* "A key vendor slipped. I analyzed the critical path, presented three options, got a sponsor decision, and updated the plan. We lost two days instead of two weeks."
3. **How do you run status meetings?** "Short, agenda-led, focused on blockers and decisions, with written notes after."
4. **What if the team hides bad news?** "I make raising problems safe, thank people for early warnings, and look for objective evidence."
5. **How do you measure progress objectively?** "Done criteria, earned value, test results, and the critical path."

### Skill 9: Project Management (Monitoring and Reporting)

**Beginner**
1. **What is monitoring?** Comparing actual performance with the plan.
2. **What does RAG stand for?** Red, Amber, Green.
3. **What goes in a status report?** Progress, issues, risks, forecast, decisions needed, next steps.
4. **What does CPI below 1 mean?** You're getting less than $1 of value per $1 spent, so you're over budget on current performance.
5. **What is a variance?** The difference between planned and actual.

**Intermediate**
1. **Why use both CPI and SPI?** CPI shows cost efficiency, SPI shows schedule efficiency.
2. **What is a corrective action?** An action that brings performance back toward the plan.
3. **What is a threshold?** An agreed variance level that triggers action or escalation.
4. **Is a negative SV always serious?** No. Check whether the late work is on the critical path or has slack.
5. **Leading vs. lagging indicator?** Leading predicts (risk triggers, defect trend). Lagging reports the past (actual cost).

**Scenario**
1. **SPI is 0.8 and CPI is 1.1.** Behind but economical. Consider adding resources on the critical path and weigh the cost trade-off. *Reasoning:* the numbers point to a capacity problem, not a cost problem.
2. **Status is green but the team looks worried.** Check the evidence behind the status and talk to the team directly. *Reasoning:* a status is only as reliable as its data.
3. **The sponsor wants daily updates.** Offer a self-service dashboard and a short weekly report.
4. **Spending is on plan but deliverables are late.** Money spent isn't progress, so check EV, SPI, and the critical path.
5. **A variance crosses the threshold.** Analyze the cause, list options, raise a change request if the baseline moves, and communicate.

**Interview**
1. **How do you monitor performance?** *Sample:* "Weekly I compare actuals to baseline using earned value and the critical path, review risks and quality data, and then decide on action."
2. **What do you put in a status report?** "Overall RAG, key metrics, what's done and next, top risks, and decisions needed. One page."
3. **Tell me about a status that turned red.** *Sample (STAR):* "SPI fell to 0.78. I found a vendor delay, presented options to the sponsor within a day, and we protected the launch by trimming two low-priority features."
4. **How do you use earned value?** "I use CPI and SPI to spot trends, then EAC to forecast, and pair them with the critical path."
5. **How do you present bad news?** "Early, factual, with impact, options, and a recommendation."

### Skill 10: Project Quality Assessment

**Beginner**
1. **Define quality assessment.** Checking whether deliverables and processes meet agreed requirements.
2. **Name three assessment methods.** Inspection, testing, audit, peer review, UAT (any three).
3. **What is an acceptance criterion?** A condition a deliverable must meet to be accepted.
4. **What is a defect?** A deliverable that doesn't meet a requirement.
5. **What does a defect log hold?** Description, severity, owner, and status for each defect.

**Intermediate**
1. **Severity vs. priority?** Severity is the effect's seriousness. Priority is the fix order.
2. **What is regression testing?** Re-running tests after a change to make sure nothing else broke.
3. **Test pass rate with 34 of 40 passed?** 85%.
4. **What does a Pareto chart show?** Causes ranked by frequency, showing the vital few.
5. **Inspection vs. testing?** Inspection reviews the work without running it. Testing runs it and compares results to expectations.

**Scenario**
1. **A deliverable fails acceptance testing.** Log defects, find root causes, fix, retest (including regression), and update stakeholders. *Reasoning:* fix and prove, don't just fix.
2. **The customer says quality is poor, but every criterion passed.** Explore the expectation gap. If the need is new, raise a change request. *Reasoning:* criteria are the contract.
3. **Defects keep recurring in payments.** Run Pareto and root-cause analysis, then add preventive actions.
4. **Testing time is squeezed.** Use risk-based testing (high-impact areas first), don't silently skip, and escalate the trade-off.
5. **A typo and a double-booking are both open.** Fix the double-booking first because it has higher severity and customer impact.

**Interview**
1. **How do you assess quality on a project?** *Sample:* "I define measurable acceptance criteria early, review and test throughout, track defects by severity, and use UAT for final acceptance."
2. **Tell me about a failed quality check.** *Sample (STAR):* "System test found a critical double-booking bug. We ran a root-cause analysis, fixed the lock logic, added concurrency tests, and retested before launch."
3. **How do you balance quality and deadlines?** "I make the trade-off visible: adjust scope or time, and never hide quality shortcuts."
4. **What quality metrics do you use?** "Test pass rate, defects by severity, defect density, performance targets, and user task success."
5. **How do you work with QA or test teams?** "Share criteria early, agree on defect severity definitions, and review results together."

### Skill 11: Quality Management

**Beginner**
1. **Name the main quality management activities.** Plan, assure, control, and improve.
2. **Define quality.** How well deliverables meet requirements and are fit for purpose.
3. **What is a quality management plan?** A document defining standards, activities, metrics, and responsibilities for quality.
4. **Prevention vs. detection?** Prevention stops defects from occurring. Detection finds existing ones.
5. **What is continuous improvement?** Ongoing effort to make processes and results better.

**Intermediate**
1. **Name the four cost-of-quality categories.** Prevention, appraisal, internal failure, external failure.
2. **Quality vs. grade?** Grade is category or features. Quality is how well requirements for that grade are met.
3. **What is PDCA?** Plan, Do, Check, Act: a loop for testing and adopting improvements.
4. **Give two quality metrics for BrightCuts.** Page load time under 2 seconds; booking completed within 3 minutes.
5. **Why define quality standards early?** They guide the work and prevent disputes at acceptance.

**Scenario**
1. **The sponsor wants to cut testing to save money.** Show the cost of failure vs. prevention and propose risk-based testing. *Reasoning:* argue with cost data.
2. **No quality plan exists in week 5.** Draft a lightweight one: criteria, definition of done, reviews, metrics. Agree on it with the team.
3. **A developer adds unrequested features.** That's gold plating. Build to criteria, and route extras through change control.
4. **Metrics look good but users complain.** The metrics may not reflect user needs, so revisit requirements and add user-focused measures.
5. **A data-privacy regulation applies.** Add compliance to standards and include audits in the plan.

**Interview**
1. **How do you build quality into a project?** *Sample:* "Measurable acceptance criteria, a definition of done, peer review, early testing, and retrospectives."
2. **Prevention or inspection?** "Both, but I invest most in prevention because defects found later cost more."
3. **Describe a continuous improvement you led.** *Sample (STAR):* "Retrospectives showed late requirement changes caused rework. We added a scenario review before development, and defects fell by a third."
4. **How do you define quality with stakeholders?** "I ask what success looks like for them and convert it to measurable criteria."
5. **How do you convince a sponsor to invest in quality?** "I compare the cost of prevention with the cost of failure, using real numbers."

### Skill 12: Quality Assurance

**Beginner**
1. **What does QA focus on?** The process that creates the work.
2. **What does QC focus on?** The product or deliverable itself.
3. **Give an example of a QA activity.** A process audit, a code-review standard, or a checklist.
4. **Give an example of a QC activity.** Testing the booking flow.
5. **True or false: QA and QC are identical.** False. QA prevents, QC detects.

**Intermediate**
1. **What are the 5 Whys?** Repeated "why?" questions to reach a root cause.
2. **What is a fishbone diagram?** A cause-and-effect diagram grouping potential causes by category.
3. **Corrective vs. preventive action?** Corrective fixes the cause of an existing problem. Preventive reduces the chance of a potential one.
4. **What is a quality audit?** A structured, independent review of whether processes and standards are followed.
5. **Why is "QA" confusing in software?** Many software teams use "QA" for testing, which project management calls QC.

**Scenario**
1. **Developers skip code reviews under deadline pressure.** Keep lightweight reviews for high-risk code, include them in the definition of done, and explain the defect cost.
2. **An audit finds documentation isn't updated.** Record a corrective action, add it to the checklist, and train the team.
3. **A critical defect appears the day before launch.** Assess severity, then decide with the sponsor: fix, workaround, or delay.
4. **The team blames the tester for bugs.** Reframe: quality is a team responsibility, so use root-cause analysis instead of blame.
5. **A process step adds delay with no value.** Review it with the team and simplify. *Reasoning:* assurance should be proportionate.

**Interview**
1. **QA vs. QC?** *Sample:* "QA prevents defects by improving processes. QC detects defects in the product. In software, 'QA' often means testing, so I clarify the term."
2. **Give a preventive action you implemented.** "After a payment bug, we added a scenario review to our checklist so similar gaps were caught before coding."
3. **How do you do root-cause analysis?** "5 Whys for simple problems, fishbone for complex ones, and Pareto to prioritize."
4. **How do you promote a quality culture?** "Clear standards, shared ownership, blame-free retrospectives, and recognizing good practice."
5. **With a developer background, how do you apply quality as a PM?** "I use my technical insight to ask the right questions about reviews and testing, but I rely on the team's expertise and focus on criteria, process, and risk."

### Skill 15: Change Management

**Beginner**
1. **What is a change request?** A formal proposal to alter scope, schedule, cost, or another baseline.
2. **What is a change control board?** A group authorized to review and approve or reject changes.
3. **Why not accept every change immediately?** Each change has impact on time, cost, quality, and risk.
4. **What is a change log?** A record of requests, impacts, decisions, and owners.
5. **True or false: every change needs the CCB.** False. Thresholds allow small changes to be approved by the PM.

**Intermediate**
1. **List the change control steps.** Raise, log, assess, decide, implement, communicate, verify.
2. **Project change control vs. organizational change management?** One controls baseline changes. The other helps people adopt new ways of working.
3. **What does ADKAR stand for?** Awareness, Desire, Knowledge, Ability, Reinforcement.
4. **How do you handle an emergency change?** Use an expedited approval, then document fully straight afterward.
5. **What does a change management plan define?** Roles, process, thresholds, documents, communication, and people-side activities.

**Scenario**
1. **Staff resist the new app.** Use ADKAR: explain why, show benefits, train, give practice, and check in after launch. *Reasoning:* find which step is missing.
2. **A change was approved but the team built the old version.** Fix the communication gap, update versions, and add "notify the team" to the process.
3. **The sponsor sends a change by casual email.** Log it formally, then reply with the impact and options.
4. **A change affects another team's project.** Consult that team and escalate to the program or portfolio level if needed.
5. **After go-live, requests keep arriving.** Move to a post-launch backlog or support process with its own prioritization.

**Interview**
1. **Describe your change control process.** *Sample:* "I log every request, assess impact with the team, present options to the approver, document the decision, update baselines, and communicate."
2. **How do you handle an urgent change?** "I use an expedited path: quick impact assessment, a named approver, and full documentation right after."
3. **Tell me about leading people through change.** *Sample (STAR):* "Staff feared a new booking tool. I involved them in testing, trained them, and named a super-user. Adoption reached 85% in a month."
4. **How do you decide whether to approve a change?** "I compare benefit with impact on the objectives, but the approver decides with my analysis."
5. **How do you prevent change fatigue?** "Batch changes, explain priorities, and avoid unnecessary changes."

### Revision Checklist
- [ ] I can run a weekly monitoring cycle and write a one-page status report
- [ ] I can compute CV, SV, CPI, SPI, and EAC from a scenario
- [ ] I can explain QA vs. QC and the software-industry confusion
- [ ] I can use 5 Whys, fishbone, and Pareto
- [ ] I can separate corrective, preventive, and repair actions
- [ ] I can run change control and an expedited change
- [ ] I can apply ADKAR to a resistance scenario

---

## 12. Case Studies (2 more of the 15)

### Case 8: A failed quality assessment

| Element | Detail |
|---|---|
| Situation | Week 9 system test: 34 of 40 test cases pass (85%, target 95%). One critical defect: two customers can book the same slot (D-14). |
| Main problem | The booking flow is not ready for acceptance, and launch is at risk |
| Root cause | 5 Whys led to a process gap: concurrent booking behavior was missing from requirements and the quality checklist |
| Options | (a) Launch anyway with a manual check, (b) fix and retest, extending by a few days, (c) fix and retest, de-scope something low-priority to protect the date |
| Recommended | (c). Don't launch with a critical defect. Fix it, then use the schedule slack and a small trade-off |
| Resolution steps | Log and rank defects. Fix D-14 first, then payment errors (Pareto shows 68% of defects in payments and calendar). Retest, run regression on the booking flow, and add concurrency tests. Add a scenario review to the QA checklist (preventive action) |
| Documentation | Defect log, updated test report, root-cause analysis, updated quality checklist, risk register update |
| Communication | Message to Maria, below. Brief the team without blame |
| Expected outcome | Critical defect closed, pass rate ≥ 95%, launch holds or moves by a few days with agreement |
| Lessons | Bugs often point to process gaps. Fix the cause, not just the defect |
| Possible exam question | "A critical defect is found in system test. What should the PM do?" Answer: assess severity, fix and retest with regression testing, find the root cause, and inform the sponsor |

> **Message to sponsor:** "Maria, system testing found a serious issue: two customers could book the same slot. We have a fix underway and expect to retest by Thursday. Pass rate is 85% today, and our target is 95%. I recommend we do not launch until it is fixed. We should still hit the launch date by using schedule slack and deferring two low-priority fixes. I'll confirm after Thursday's retest."

### Case 12: A project requiring urgent change management

| Element | Detail |
|---|---|
| Situation | Week 9: the payment provider announces its current API version will be switched off two weeks after the planned launch |
| Main problem | The app would stop taking payments soon after go-live |
| Root cause | External dependency change that the team didn't control and had not foreseen |
| Options | (1) Migrate to the new API version before launch, (2) launch on the old version and migrate later, (3) switch provider |
| Recommended | Option 1. Option 2 risks a rushed migration during live use. Option 3 is too large this late |
| Resolution steps | Raise CR-004 on the same day. Dev estimates +4 days and +$1,500. PM checks float and the contingency budget. Maria approves within 24 hours (expedited path in the change management plan). Update the schedule, budget, test plan, and risk register. Retest the payment flows. Inform Tom and the stylists if training screens change |
| Documentation | Change request form, change log, updated baseline, risk register |
| Communication | Message to Maria, below. Update the team in stand-up. Update the training guide |
| Expected outcome | Migration completed, launch date kept, small cost increase approved |
| Lessons | Prepare an expedited change path before you need it, and monitor vendor announcements |
| Possible exam question | "An urgent change arrives. What should the PM do?" Answer: assess impact quickly, get approval from the authorized person using the expedited path, and document it |

> **Message to sponsor:** "Maria, the payment provider has announced it will switch off our current API version two weeks after launch. I recommend we migrate before launch. That adds about 4 days and $1,500, and we can absorb the time using buffer. Could you approve by Friday so we keep the launch date? Details are in CR-004."

---

## Part 5 Checkpoint Quiz

Try these **without looking back**:

1. Calculate CPI and SPI: EV = $14,400, AC = $16,000, PV = $17,500. What do they mean?
2. Defects found: payments 20, calendar 14, reminders 8, UI 5, other 3. What percentage do the top two represent?
3. State one difference between QA and QC, and explain why "QA" can be confusing in software.
4. A bug is fixed, but it keeps coming back in other places. Name the type of action that would address this and give an example.
5. List the steps of change control in order.
6. Staff don't want to use the new tool. Which ADKAR element might be missing, and what would you do?
