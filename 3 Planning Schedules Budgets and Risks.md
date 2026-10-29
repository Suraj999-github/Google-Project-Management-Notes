# Part 3: Planning, Schedules, Budgets, and Risks

**Source note:** As publicly described, Google's *Project Planning* course covers the work breakdown structure (WBS), estimating, schedules, budgets, procurement, risk management, and communication and quality planning. I haven't re-checked Coursera live, so confirm the current course contents there. **[Supplemental]** marks my additions, such as PMBOK comparisons and extra formulas. The templates, numbers, and questions are my original material, not official Google content.

---

## 1. Learning Objectives

By the end of Part 3 you should be able to:
- Break a project into a WBS and estimate effort, time, and cost
- Build a schedule and find the critical path and slack
- Create a budget, set a baseline, and track cost and schedule performance
- Identify, score, and respond to risks using a risk register
- Calculate CV, SV, CPI, SPI, EAC, ETC, EMV, and PERT estimates

**Running example:** BrightCuts Online Booking App, with a **$30,000** budget and **12 weeks**.

---

## 2. How the Pieces Connect

```
Signed scope → WBS → Activities → Estimates → Schedule + Budget
                                      ↓
                        Risk register ← tests every estimate
                                      ↓
                         Approved baseline → Execution
```

The WBS shows what the work is. Estimates and dependencies turn it into a schedule and budget. The risk register challenges those estimates. Once approved, the plan becomes the **baseline**, the reference you measure progress against.

---

## 3. Skill 2: Project Planning

**Definition:** Turning the approved scope into a realistic, agreed plan for work, time, cost, people, risk, communication, and quality.

**Why it matters:** A plan lets you predict problems, set expectations, and measure progress. Without a baseline you can't say whether you're behind.

**When to use:** After the charter is signed, and again when approved changes occur.

**Step-by-step process**
1. Review the charter and scope statement.
2. Build the **WBS** (break scope into work packages).
3. List **activities** and **dependencies**.
4. **Estimate** effort and duration.
5. Build the **schedule**, find the critical path, and set milestones.
6. Estimate **costs** and build the budget, including contingency.
7. Assign people (RACI).
8. Create the risk, communication, quality, and procurement plans.
9. Get approval and set the **baseline**.
10. Hold a **kickoff meeting**.

**Estimation techniques**

| Technique | How it works | Best when |
|---|---|---|
| Analogous | Based on a similar past project | Early, quick estimates |
| Bottom-up | Estimate small tasks, then add up | You need accuracy |
| Parametric | Uses a unit rate (e.g., hours per screen) | Repeatable work |
| Three-point / PERT | Uses best, likely, and worst cases | High uncertainty |
| Expert judgment | Ask experienced people | Always, as a cross-check |

**Dependency types:** *Finish-to-start* (most common: B starts when A finishes), *start-to-start*, *finish-to-finish*, *start-to-finish* (rare).

**Schedule compression:** *Crashing* adds resources, which costs more. *Fast-tracking* overlaps tasks, which adds risk. Adding people late can slow a project down because of onboarding and coordination overhead.

**Procurement:** Buying from outside vendors. Documents typically include a request for information (RFI), request for proposal (RFP), request for quotation (RFQ), and a statement of work (SOW). For BrightCuts, the payment provider is a procurement relationship.

### Template: Work Breakdown Structure (completed)

```
1 BrightCuts Booking App
├─ 1.1 Project management (charter, plan, status reports, closure)
├─ 1.2 Requirements and design
│   ├─ 1.2.1 Requirements document
│   ├─ 1.2.2 UI design
│   └─ 1.2.3 Design approval
├─ 1.3 Development
│   ├─ 1.3.1 Booking flow
│   ├─ 1.3.2 Admin dashboard
│   └─ 1.3.3 Payment integration
├─ 1.4 Testing
│   ├─ 1.4.1 System testing
│   └─ 1.4.2 User acceptance testing (UAT)
└─ 1.5 Launch and training
```

**Rules:** the 100% rule (the WBS contains all scope and nothing outside it), deliverable-focused names, and a lowest level small enough to estimate and assign (a **work package**).

### Template: Schedule with Critical Path (completed)

Durations are in weeks.

| ID | Task | Duration | Depends on | ES | EF | LS | LF | Slack |
|---|---|---|---|---|---|---|---|---|
| A | Requirements | 2 | none | 0 | 2 | 0 | 2 | 0 |
| B | UI design | 2 | A | 2 | 4 | 2 | 4 | 0 |
| C | Booking flow | 4 | B | 4 | 8 | 4 | 8 | 0 |
| D | Admin dashboard | 3 | B | 4 | 7 | 5 | 8 | 1 |
| E | Payment integration | 2 | B | 4 | 6 | 6 | 8 | 2 |
| F | System testing | 2 | C, D, E | 8 | 10 | 8 | 10 | 0 |
| G | UAT | 1 | F | 10 | 11 | 10 | 11 | 0 |
| H | Training and launch | 1 | G | 11 | 12 | 11 | 12 | 0 |

*ES = earliest start, EF = earliest finish, LS = latest start, LF = latest finish.*

**Critical path: A → B → C → F → G → H = 12 weeks.** Any delay on these tasks delays launch. D has 1 week of slack and E has 2.

### Template: Gantt Chart (completed)

```
                   1  2  3  4  5  6  7  8  9 10 11 12
A Requirements    ■■ ■■
B Design                ■■ ■■
C Booking flow                ■■ ■■ ■■ ■■
D Admin dashboard             ■■ ■■ ■■
E Payment API                 ■■ ■■
F System testing                          ■■ ■■
G UAT                                           ■■
H Training/launch                                  ■■
```

### Template: Milestone Plan (completed)

| Milestone | Target | Evidence |
|---|---|---|
| M1 Charter signed | Week 1 | Signed charter |
| M2 Requirements approved | End wk 2 | Sponsor sign-off |
| M3 Design approved | End wk 4 | Sponsor sign-off |
| M4 Development complete | End wk 8 | Features demo |
| M5 UAT passed | End wk 11 | Test report |
| M6 Go-live | End wk 12 | Live app, trained staff |

### Template: Project Budget and Cost Tracking (completed)

| Category | Budget | Actual to date | Variance (Budget − Actual) |
|---|---|---|---|
| Developer labor | $16,000 | $8,200 | n/a until complete |
| UI designer | $3,000 | $3,000 | $0 |
| QA / testing | $2,500 | $0 | n/a |
| Hosting, licenses, payment API fees | $1,500 | $400 | n/a |
| Training materials | $1,000 | $0 | n/a |
| PM and coordination | $3,000 | $1,400 | n/a |
| **Contingency reserve (10%)** | $3,000 | $0 | n/a |
| **Total** | **$30,000** | **$13,000** | |

**[Supplemental]** PMBOK separates *contingency reserve* (for known risks, inside the cost baseline) from *management reserve* (for unknown risks, held outside the baseline and released by management).

---

## 4. Essential Formulas and Numerical Problems

**Predictive vs. Agile:** The formulas below suit predictive (plan-driven) projects with a fixed baseline. Agile teams usually track progress with velocity and burndown charts, which I cover in Part 6. EMV, PERT, and the critical path can still help on hybrid projects.

### 4.1 Critical Path Method (CPM)
- **Idea:** The longest path through the dependent tasks sets the minimum project duration.
- **Variables:** duration = time for each task. A path's length is the sum of its task durations.
- **Useful when:** you need the earliest finish date and want to know which tasks you can't afford to delay.
- **Worked example:** BrightCuts path A-B-C-F-G-H = 2+2+4+2+1+1 = **12**. Path A-B-D-F-G-H = 2+2+3+2+1+1 = 11. Path A-B-E-F-G-H = 10.
- **Plain English:** The project can't finish in under 12 weeks, and the tasks on that path have no room to slip.

| Practice | Solution |
|---|---|
| 1. A(4) and B(6) both precede C(3). Duration? | A-C = 7, B-C = 9. **9**, critical path B-C |
| 2. A(2)→B(5)→D(1); A(2)→C(3)→D(1). Duration? | A-B-D = 8, A-C-D = 6. **8** |
| 3. In Q2, B slips by 2. New duration? | B is critical, so **10** |

### 4.2 Slack (Float)
- **Formula:** Slack = LS − ES (or LF − EF).
- **Variables:** LS = latest start without delaying the project, ES = earliest start.
- **Useful when:** deciding which tasks can flex.
- **Worked example:** Task D: LS 5 − ES 4 = **1 week**.
- **Plain English:** D can slip a week without moving the launch date. Slack of 0 means the task is critical.

| Practice | Solution |
|---|---|
| 1. ES=4, EF=7, LS=5, LF=8. Slack? | 5−4 = **1** |
| 2. Using 4.1 Q2, slack of C? | Critical length 8, C-path 6, so **2** |
| 3. A task has ES=10, LS=10. Critical? | Slack 0, so **yes** |

### 4.3 Three-Point Estimate (simple average)
- **Formula:** Estimate = (O + M + P) ÷ 3.
- **Variables:** O = optimistic, M = most likely, P = pessimistic.
- **Useful when:** an estimate is uncertain and you want to include a range.
- **Worked example:** Booking flow O=3, M=4, P=7 weeks → (3+4+7)÷3 = 14÷3 = **4.67 weeks**.
- **Plain English:** The expected duration is a bit above the most likely value because the downside is bigger.

| Practice | Solution |
|---|---|
| 1. O=2, M=5, P=11 | 18÷3 = **6** |
| 2. O=4, M=6, P=8 | 18÷3 = **6** |
| 3. O=10, M=12, P=20 | 42÷3 = **14** |

### 4.4 PERT (Program Evaluation and Review Technique) Estimate
- **Formulas:** Estimate = (O + 4M + P) ÷ 6. Standard deviation (SD) = (P − O) ÷ 6.
- **Useful when:** you want the most likely value to carry more weight and want a measure of uncertainty.
- **Worked example:** O=3, M=4, P=7 → (3+16+7)÷6 = 26÷6 = **4.33 weeks**. SD = (7−3)÷6 = **0.67**. About 68% likely to land between 3.67 and 5.0 weeks.
- **Plain English:** The weighted estimate is 4.33 weeks, and the wider the range between O and P, the less certain you are.

| Practice | Solution |
|---|---|
| 1. O=2, M=5, P=11 | (2+20+11)÷6 = **5.5**; SD = 9÷6 = **1.5** |
| 2. O=4, M=6, P=8 | 36÷6 = **6**; SD = 4÷6 ≈ **0.67** |
| 3. O=10, M=12, P=20 | 78÷6 = **13**; SD = 10÷6 ≈ **1.67** |

### 4.5 Expected Monetary Value (EMV)
- **Formula:** EMV = Probability × Impact.
- **Variables:** probability = chance the event happens (as a decimal), impact = money gained (+) or lost (−).
- **Useful when:** comparing risks or sizing contingency.
- **Worked example:** Payment API late: 40% × −$3,000 = **−$1,200**. Free hosting credit: 20% × +$1,000 = **+$200**. Net = −$1,000.
- **Plain English:** On average, these two uncertainties cost about $1,000. That is the basis for a contingency estimate, not a prediction of what will happen.

| Practice | Solution |
|---|---|
| 1. 20% chance of −$10,000 | **−$2,000** |
| 2. Risk 1: 50% × −$4,000. Risk 2: 10% × −$15,000. Larger exposure? | −$2,000 vs −$1,500, so **Risk 1**; total −$3,500 |
| 3. Opportunity 30% × +$5,000; threat 25% × −$8,000. Net? | +1,500 − 2,000 = **−$500** |

### 4.6 Budget Variance
- **Formula:** Budget variance = Budgeted − Actual. Percent = variance ÷ budgeted × 100.
- **Variables:** budgeted = planned cost, actual = real cost.
- **Useful when:** comparing a completed item or category with its budget.
- **Worked example:** Developer labor budgeted $16,000, actual $17,500 → **−$1,500** (**−9.4%**).
- **Plain English:** Negative means over budget, positive means under.

| Practice | Solution |
|---|---|
| 1. Budget $10,000, actual $8,500 | **+$1,500** (15% under) |
| 2. Budget $5,000, actual $5,600 | **−$600** (12% over) |
| 3. Budget $20,000, actual $20,000 | **$0** (on budget) |

### 4.7 Percentage Complete
- **Formula:** % complete = EV ÷ BAC × 100 (or work done ÷ total work).
- **Variables:** EV = earned value (budgeted value of work actually done), BAC = budget at completion (total baseline budget).
- **Worked example:** BAC $30,000, EV $12,000 → **40%**.
- **Plain English:** 40% of the planned value of the work is done.

| Practice | Solution |
|---|---|
| 1. EV $6,000, BAC $24,000 | **25%** |
| 2. 18 of 24 deliverables done (equal value) | **75%** |
| 3. BAC $50,000, 35% complete. EV? | **$17,500** |

### 4.8 Earned Value Management (EVM): the Core Variables

All four of the next metrics use the same example at the **end of week 6**:

| Variable | Meaning | Value |
|---|---|---|
| BAC | Budget at completion | $30,000 |
| PV | Planned value: budgeted value of work *scheduled* by now | $15,000 (50% planned) |
| EV | Earned value: budgeted value of work *actually done* | $12,000 (40% done) |
| AC | Actual cost spent so far | $14,000 |

### 4.9 Cost Variance (CV)
- **Formula:** CV = EV − AC. **Useful when:** you want to know if you're over or under budget in money terms.
- **Example:** 12,000 − 14,000 = **−$2,000**.
- **Plain English:** We've spent $2,000 more than the value of work done, so we are over budget.

| Practice | Solution |
|---|---|
| 1. EV $8,000, AC $9,000 | **−$1,000** (over budget) |
| 2. EV $15,000, AC $12,000 | **+$3,000** (under budget) |
| 3. EV $20,000, AC $20,000 | **$0** |

### 4.10 Schedule Variance (SV)
- **Formula:** SV = EV − PV. **Useful when:** you want to know if you're ahead of or behind plan, expressed in money.
- **Example:** 12,000 − 15,000 = **−$3,000**.
- **Plain English:** We've completed $3,000 less planned work than scheduled, so we are behind.

| Practice | Solution |
|---|---|
| 1. EV $8,000, PV $10,000 | **−$2,000** (behind) |
| 2. EV $12,000, PV $9,000 | **+$3,000** (ahead) |
| 3. EV $5,000, PV $5,000 | **$0** (on schedule) |

### 4.11 Cost Performance Index (CPI)
- **Formula:** CPI = EV ÷ AC. **Useful when:** you want an efficiency ratio. Above 1 is good, below 1 is bad.
- **Example:** 12,000 ÷ 14,000 = **0.86**.
- **Plain English:** For every $1 spent we're getting about 86 cents of planned value.

| Practice | Solution |
|---|---|
| 1. EV $8,000, AC $10,000 | **0.80** |
| 2. EV $15,000, AC $12,000 | **1.25** |
| 3. EV $9,000, AC $9,000 | **1.00** |

### 4.12 Schedule Performance Index (SPI)
- **Formula:** SPI = EV ÷ PV. **Useful when:** you want a schedule efficiency ratio.
- **Example:** 12,000 ÷ 15,000 = **0.80**.
- **Plain English:** We're progressing at 80% of the planned pace.

| Practice | Solution |
|---|---|
| 1. EV $6,000, PV $8,000 | **0.75** |
| 2. EV $11,000, PV $10,000 | **1.10** |
| 3. EV $4,500, PV $4,500 | **1.00** |

### 4.13 Estimate at Completion (EAC)
- **Formulas:**
  - If current cost performance continues: **EAC = BAC ÷ CPI**
  - If the past variance was a one-off: **EAC = AC + (BAC − EV)**
- **Useful when:** forecasting the final cost.
- **Example:** 30,000 ÷ 0.857 = **$35,000**. One-off version: 14,000 + (30,000 − 12,000) = **$32,000**.
- **Plain English:** If we keep performing like this, the project will cost $35,000, which is $5,000 over (VAC = BAC − EAC = −$5,000). If the overrun was a one-time event, about $32,000.

| Practice | Solution |
|---|---|
| 1. BAC $100,000, CPI 0.8 | **$125,000** |
| 2. BAC $50,000, CPI 1.25 | **$40,000** |
| 3. BAC $60,000, EV $20,000, AC $25,000, one-off variance | 25,000 + 40,000 = **$65,000** |

### 4.14 Estimate to Complete (ETC)
- **Formula:** ETC = EAC − AC. **Useful when:** you need to know how much more money is required.
- **Example:** 35,000 − 14,000 = **$21,000**.
- **Plain English:** We expect to spend $21,000 more.

| Practice | Solution |
|---|---|
| 1. EAC $125,000, AC $50,000 | **$75,000** |
| 2. EAC $40,000, AC $30,000 | **$10,000** |
| 3. EAC $65,000, AC $25,000 | **$40,000** |

*Sprint velocity and burndown interpretation are covered in Part 6 alongside Agile.*

---

## 5. Skill 6: Project Risk Management

**Definition:** Identifying, analyzing, responding to, and monitoring uncertain events that could affect project objectives, either negatively (**threats**) or positively (**opportunities**).

**Why it matters:** Managing risk early is cheaper than reacting to a crisis. It also builds credibility with sponsors.

**Process**
1. **Plan:** agree how risk will be handled (roles, scales, thresholds).
2. **Identify:** brainstorm, review past projects, interview stakeholders, check assumptions.
3. **Analyze:** *qualitative* (rank by probability and impact) and *quantitative* (numbers, such as EMV).
4. **Plan responses:** assign an owner and an action.
5. **Monitor and control:** review regularly, watch triggers, update the register.

**Response strategies**

| Threats | Meaning | BrightCuts example |
|---|---|---|
| **Avoid** | Remove the cause | Choose a payment provider with a proven API |
| **Mitigate** | Reduce probability or impact | Build against a mock API until the real one arrives |
| **Transfer** | Shift impact to a third party | Use a provider that handles card data and its liability |
| **Accept** | Do nothing now, or hold a contingency | Accept a minor styling delay |

**[Supplemental]** For opportunities, PMBOK lists *exploit, enhance, share, accept*.

**Key terms:** *Trigger* is an early warning sign. *Residual risk* remains after a response. *Secondary risk* is created by a response. *Contingency plan* is a fallback activated if the risk occurs.

### Template: Probability-Impact Matrix

Scale 1 (very low) to 5 (very high). **Score = Probability × Impact.**

| Score | Rating | Action |
|---|---|---|
| 1 to 5 | Low | Monitor |
| 6 to 11 | Medium | Plan a response |
| 12 to 25 | High | Prioritize, report to the sponsor |

```
Impact →      1    2    3    4    5
Prob 5     |  5 | 10 | 15 | 20 | 25 |
Prob 4     |  4 |  8 | 12 | 16 | 20 |
Prob 3     |  3 |  6 |  9 | 12 | 15 |
Prob 2     |  2 |  4 |  6 |  8 | 10 |
Prob 1     |  1 |  2 |  3 |  4 |  5 |
```

### Template: Risk Register (completed)

| ID | Risk | P | I | Score | Response | Owner | Trigger |
|---|---|---|---|---|---|---|---|
| R1 | Payment API delivered late | 4 | 4 | **16 (High)** | Mitigate: get date in writing, build mock API | Developer | No sandbox access by week 4 |
| R2 | Low customer adoption | 3 | 4 | **12 (High)** | Mitigate: in-salon signage, first-booking discount | Maria | Under 20% online bookings in month 1 |
| R3 | Sponsor requests uncontrolled changes | 4 | 3 | **12 (High)** | Mitigate: change control, weekly decisions | PM | More than 2 change requests in one week |
| R4 | Customer data breach | 2 | 5 | 10 (Med) | Transfer and mitigate: provider handles card data, encrypt personal data | Developer | Security scan fails |
| R5 | Developer unavailable (illness) | 2 | 4 | 8 (Med) | Mitigate: documented code, backup contractor on call | PM | Absence over 3 days |

**Relationships:** Risks feed the **contingency budget** and **schedule buffers**. High risks go into **status reports**. Stakeholder analysis helps identify people risks. When a risk occurs, it moves to the **issue log**.

---

## 6. Common Challenges and Solutions (Skills 2 and 6)

| Challenge | Solution |
|---|---|
| Optimistic estimates | Use three-point estimates and ask for assumptions |
| Hidden padding on every task | Keep contingency visible and owned by the PM |
| Plan never updated | Review weekly and re-baseline only through approved changes |
| Risk register filled once, then forgotten | Review risks in every status meeting |
| Team hides bad news | Reward early reporting; don't punish messengers |
| Dependencies on external vendors ignored | Track as milestones with owners and trigger dates |

---

## 7. Module Summary and Revision Notes

- WBS defines the work; estimates and dependencies create the schedule.
- The **critical path** is the longest path and has **zero slack**.
- The **baseline** is the approved plan you measure against.
- **CV = EV − AC**, **SV = EV − PV**, **CPI = EV ÷ AC**, **SPI = EV ÷ PV**. Negative variances and indices below 1 are bad.
- **EAC = BAC ÷ CPI** (typical), **ETC = EAC − AC**.
- **PERT = (O + 4M + P) ÷ 6**. **EMV = probability × impact**.
- Risk responses for threats: **avoid, mitigate, transfer, accept**.
- A risk is a possible future event, and an issue is happening now.

---

## 8. Skill-by-Skill Question Sets

*Brief explanations are included here. The full 10-field format appears in the numbered bank in Part 8.*

### Skill 2: Project Planning

**Beginner**
1. **What is a WBS?** A hierarchical breakdown of project scope into smaller deliverables and work packages.
2. **What is a baseline?** The approved scope, schedule, and cost plan used to measure performance.
3. **What is a dependency?** A relationship where one task relies on another.
4. **Name the four dependency types.** Finish-to-start, start-to-start, finish-to-finish, start-to-finish.
5. **True or false: a milestone has a duration.** False. It marks a point in time.

**Intermediate**
1. **Analogous vs. bottom-up estimating?** Analogous uses a similar past project, so it is fast but rougher. Bottom-up sums small-task estimates, so it is slower but more accurate.
2. **What is a work package?** The lowest WBS level, small enough to estimate and assign.
3. **What is the 100% rule?** The WBS must include all the work in scope and nothing more.
4. **Why include contingency?** Estimates carry uncertainty, so contingency covers known risks openly instead of hidden padding.
5. **Crashing vs. fast-tracking?** Crashing adds resources, which costs more. Fast-tracking overlaps tasks, which adds risk.

**Scenario**
1. **The developer says 4 weeks, you expect 6.** Ask for the basis, compare with past work, and use three-point or PERT. *Reasoning:* resolve estimates with evidence, not opinion.
2. **The sponsor demands launch in 8 weeks, but the plan says 12.** Show the critical path and offer options (cut scope, compress with stated costs and risks, or move the date). Document the decision. *Reasoning:* make trade-offs visible, don't silently agree.
3. **Task F depends on a vendor.** Add the dependency, a milestone with a date, an owner, and a risk entry.
4. **The developer is booked at 150% in week 6.** Resource-level by shifting non-critical tasks (D has slack) or adding help.
5. **The plan is approved but nobody reads it.** Hold a kickoff, share a one-page summary, store it in a shared place, and review it in weekly meetings.

**Interview**
1. **How do you build a project plan?** *Sample:* "I start from the signed scope, build a WBS, estimate with the team, map dependencies, find the critical path, add a budget with contingency, then plan risks and communication. I get sign-off to set a baseline."
2. **How do you estimate?** "I combine team input with historical data and use three-point estimates for uncertain tasks."
3. **Tell me about an unrealistic schedule.** *Sample (STAR):* "The sponsor wanted a 6-week launch for a 10-week scope. I showed the critical path and options. We cut two low-priority features and launched on time."
4. **What is the critical path and why does it matter?** "It's the longest dependent chain, which sets the minimum duration. Delays there delay the project."
5. **How do you plan a budget with uncertainty?** "I build bottom-up, add a documented contingency based on risk EMV, and track it with earned value."

### Skill 6: Project Risk Management

**Beginner**
1. **Define risk.** An uncertain future event that can positively or negatively affect objectives.
2. **Risk vs. issue?** A risk might happen. An issue is already happening.
3. **What is a risk register?** A log of risks with probability, impact, response, owner, and status.
4. **Four responses to threats?** Avoid, mitigate, transfer, accept.
5. **True or false: all risks are negative.** False. Opportunities are positive risks.

**Intermediate**
1. **How is a risk score calculated?** Probability × impact on agreed scales.
2. **Mitigate vs. transfer?** Mitigating reduces probability or impact. Transferring shifts the consequence to another party, such as through a contract or insurance, without removing the risk.
3. **What is a risk trigger?** An early warning sign that the risk may be about to occur.
4. **Residual vs. secondary risk?** Residual remains after the response. Secondary is created by the response itself.
5. **Qualitative vs. quantitative analysis?** Qualitative ranks risks with scales. Quantitative uses numbers, such as EMV.

**Scenario**
1. **A risk's probability rises from medium to high.** Update the register, reassess the response, and tell the sponsor. *Reasoning:* the register is a living document.
2. **A risk happens.** It becomes an issue: log it, activate the contingency plan, assign an owner, and communicate.
3. **Team members hide problems.** Build psychological safety, ask about risks in every meeting, and thank people for early warnings.
4. **Mitigation costs $5,000 but EMV is $1,200.** Don't overspend. Accept the risk and hold contingency.
5. **A high-impact risk has very low probability.** Keep it in the register, monitor it, and set a contingency if the impact is severe.

**Interview**
1. **How do you manage risks?** *Sample:* "I run a risk workshop at the start, score by probability and impact, assign owners and responses, and review the register weekly."
2. **Tell me about a risk you mitigated.** *Sample (STAR):* "A vendor's API was likely to be late. I built against a mock API and tracked a trigger date. When the delay came, we lost two days instead of two weeks."
3. **How do you prioritize risks?** "Using a probability-impact score, then adjusting for proximity and urgency."
4. **How do you explain risk to executives?** "I show the top three risks, their cost exposure, my planned response, and any decision I need from them."
5. **Risk vs. issue?** "A risk is a potential future event. An issue is happening now and needs action."

### Revision Checklist
- [ ] I can build a WBS and find the critical path
- [ ] I can calculate slack, PERT, and EMV
- [ ] I can compute CV, SV, CPI, SPI, EAC, ETC
- [ ] I can fill in a risk register and a probability-impact matrix
- [ ] I can name the four threat responses with examples

---

## 9. Case Studies (3 more of the 15)

### Case 3: A project that is behind schedule

| Element | Detail |
|---|---|
| Situation | End of week 6: SPI = 0.80. The booking flow (critical path) is a week behind. |
| Main problem | The launch date is at risk |
| Root cause | The payment rules were more complex than estimated, and requirements were clarified late |
| Options | (a) Crash by adding a developer, (b) fast-track testing of finished modules, (c) cut low-priority scope, (d) move the date |
| Recommended | (b) plus (c): start testing finished modules early and defer "could have" features. Adding a person late would slow the team in onboarding |
| Resolution steps | Confirm the delay on the critical path, quantify, list options with cost and risk, present them to the sponsor, update the schedule through change control, add the risk of rushed testing to the register |
| Documentation | Updated schedule, change log, risk register, status report |
| Communication | Tell Maria early: "We're one week behind on the critical path. Here are three options and my recommendation." |
| Outcome | Launch holds at 12 weeks with two minor features deferred |
| Lessons | Track the critical path weekly and raise delays early |
| Possible exam question | "Which tasks matter most when a project is behind?" Answer: those on the critical path |

### Case 4: A project exceeding its budget

| Element | Detail |
|---|---|
| Situation | End of week 6: CPI = 0.86, EAC = $35,000 against $30,000 |
| Main problem | Forecast overrun of $5,000 |
| Root cause | Payment integration hours were underestimated and rework followed unclear requirements |
| Options | (a) Use the $3,000 contingency and trim scope, (b) ask for more budget, (c) both |
| Recommended | (c): use contingency, drop SMS reminders (keep email), and request a small budget increase if needed |
| Resolution steps | Find the root cause, re-forecast with EAC and ETC, check whether the variance is typical or a one-off, present options with numbers, get a documented decision |
| Documentation | Updated budget, change request, status report |
| Communication | Lead with the forecast, not the problem: "At the current rate we'll finish at $35,000. Here's how we can close $5,000." |
| Outcome | Scope trim plus contingency closes most of the gap, and the sponsor approves a $1,000 increase |
| Lessons | Watch CPI trends. Don't wait for the money to run out |
| Possible exam question | "CPI is 0.86. What does that mean?" Answer: we get 86 cents of value per dollar spent |

### Case 7: A high-probability, high-impact risk

| Element | Detail |
|---|---|
| Situation | Payment vendor's sandbox API is promised for week 4 but has slipped before (R1, score 16) |
| Main problem | A late API would delay the critical path and the launch |
| Root cause | Dependence on an external party you don't control |
| Options | Avoid (switch vendor), mitigate (mock API, written commitment), transfer (contract penalty), accept |
| Recommended | Mitigate, with a contingency plan and a clear trigger |
| Resolution steps | Get the vendor's delivery date in writing, escalate through their account manager, build against a mock API, set the trigger "no sandbox by end of week 4", pre-approve switching to a backup vendor if triggered |
| Documentation | Risk register entry, contingency plan, procurement notes |
| Communication | Brief Maria on R1 and the trigger. Update in every status report |
| Outcome | The API arrives 8 days late, but integration is nearly ready, so only 2 days are lost |
| Lessons | Plan the response before the risk happens |
| Possible exam question | "What action best reduces the impact of a likely vendor delay?" Answer: mitigate with a mock and a contingency plan |

---

## Part 3 Checkpoint Quiz

Try these **without looking back**:

1. Tasks: A(3)→B(5)→D(2) and A(3)→C(4)→D(2). What is the duration and critical path?
2. Calculate CPI and SPI: EV = $9,000, AC = $10,000, PV = $12,000.
3. Calculate the PERT estimate: O = 4, M = 6, P = 14 days.
4. A risk has a 25% chance and a −$8,000 impact. What is the EMV?
5. Name the four threat-response strategies and give one BrightCuts example of any.