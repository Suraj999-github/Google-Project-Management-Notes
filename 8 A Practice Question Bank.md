# Part 8A: Practice Question Bank (Q21 to Q60)

**Note:** These are original practice questions, not official Google assessment content. The 10-field format is used throughout: number, topic and skill, difficulty, question, choices, correct answer, why it is correct, why the others are wrong, the concept tested, and a workplace takeaway.

**Plan change:** I said 8A would hold 100+ questions. Questions this fully explained would make one message too long to check carefully, so I'm delivering **40 per installment**. Q1 to Q20 were in Part 1.

| Installment | Questions |
|---|---|
| **8A (this one)** | Q21 to Q60 |
| 8B to 8E | Q61 to Q220 (40 each), which finishes the 200+ bank |
| 8F to 8I | Four full-length mock tests (50 questions each) with answer keys and score sheets |

**Formats here:** MCQ, multiple-select (with the number to select stated), true/false, matching, numerical, and scenario.

---

## Initiation and Scoping (Q21 to Q27)

**Q21 | Project Scoping | Beginner | MCQ (select 1)**
Which statement is a measurable acceptance criterion?
A. "The app should look modern."
B. "A customer can complete a booking in under 3 minutes during user acceptance testing."
C. "The project budget is $30,000."
D. "Maria Lopez is the sponsor."

**Correct answer: B.**
**Why correct:** It can be tested with a pass or fail result.
**Why others are wrong:** A is subjective. C is a constraint. D is a role.
**Concept:** Acceptance criteria. **Takeaway:** If two people could disagree about whether it passed, rewrite it with a number or a test.

---

**Q22 | Project Scoping | Intermediate | True/False**
"If the in-scope list is detailed, an out-of-scope list is unnecessary."

**Correct answer: False.**
**Why:** Stakeholders fill silence with assumptions. An explicit exclusions list (for example, "no native mobile app") stops disputes before they start.
**Concept:** Scope boundaries. **Takeaway:** Get exclusions signed with the scope.

---

**Q23 | SMART goals | Intermediate | Multiple-select (select 2)**
Which two goals are SMART?
A. "Improve customer satisfaction."
B. "Raise online bookings to 60% of all bookings within 3 months of launch."
C. "Make the app fast."
D. "Reduce the no-show rate from 12% to 6% within 90 days of launch."

**Correct answer: B and D.**
**Why correct:** Each is specific, measurable, and time-bound, with a baseline or target.
**Why others are wrong:** A and C are vague and have no measure or deadline.
**Concept:** SMART goals. **Takeaway:** Ask "How will we know, and by when?" until a number appears.

---

**Q24 | Stakeholder Analysis | Beginner | MCQ (select 1)**
A city regulator has high power over your project but little interest in day-to-day details. The best engagement approach is:
A. Monitor
B. Keep informed
C. Keep satisfied
D. Manage closely

**Correct answer: C.**
**Why correct:** High power and low interest means meeting their needs without overwhelming them.
**Why others are wrong:** A suits low power and low interest. B suits low power and high interest. D suits high power and high interest.
**Concept:** Power-interest grid. **Takeaway:** Ignoring a high-power stakeholder is the costly mistake.

---

**Q25 | Stakeholder Analysis | Intermediate | Matching**
Match each quadrant to its strategy.
1. High power, high interest
2. High power, low interest
3. Low power, high interest
4. Low power, low interest
a. Keep informed
b. Monitor
c. Manage closely
d. Keep satisfied

**Correct answer: 1-c, 2-d, 3-a, 4-b.**
**Why:** The strategy matches how much influence they hold and how much they care.
**Concept:** Engagement strategy. **Takeaway:** The grid is a starting point, so review placements as attitudes change.

---

**Q26 | RACI | Intermediate | Scenario (select 1)**
Your RACI shows two people marked "A" (Accountable) for "approve test results." What should you do?
A. Leave it, since more accountability is better.
B. Ask the sponsor to confirm one accountable person and update the RACI.
C. Remove both and let the team decide.
D. Make yourself accountable.

**Correct answer: B.**
**Reasoning:** Accountability means a single owner of the outcome. Two As means each can assume the other will decide. The sponsor has the authority to settle it.
**Why others are wrong:** A defeats the purpose. C leaves no owner. D bypasses authority.
**Concept:** One A per task. **Takeaway:** Resolve role overlaps before work starts.

---

**Q27 | Scope Management | Advanced | Scenario (select 1)**
A developer adds an unrequested calendar-export feature. It works and passes tests. What is the best response?
A. Keep it, since it adds value.
B. Delete it without discussion.
C. Treat it as gold plating: review it through change control, then remove it or formally approve it, and remind the team that extras need approval.
D. Charge the sponsor for it.

**Correct answer: C.**
**Reasoning:** Unrequested work adds maintenance, testing, and risk even if it looks harmless. Change control lets the sponsor decide with the real cost in view.
**Why others are wrong:** A skips the decision. B wastes work and alienates the developer. D bills for unapproved work.
**Concept:** Gold plating. **Takeaway:** Praise initiative, but route extras through the same process as every other change.

---

## Planning, Estimating, and Schedule (Q28 to Q31)

**Q28 | Project Planning | Beginner | MCQ (select 1)**
Estimating a new project's duration from a similar past project is:
A. Bottom-up estimating
B. Analogous estimating
C. Parametric estimating
D. Three-point estimating

**Correct answer: B.**
**Why correct:** Analogous estimating uses a comparable earlier project as the reference.
**Why others are wrong:** A sums small task estimates. C uses a unit rate. D uses optimistic, likely, and pessimistic values.
**Concept:** Estimation techniques. **Takeaway:** Analogous is quick but rough, so use it early.

---

**Q29 | Project Planning (PERT) | Intermediate | Numerical (select 1)**
A task has O = 6, M = 9, P = 18 days. What is the PERT estimate and standard deviation?
A. 9 days, SD 2
B. 10 days, SD 2
C. 11 days, SD 4
D. 12 days, SD 6

**Correct answer: B.**
**Calculation:** (6 + 4×9 + 18) ÷ 6 = 60 ÷ 6 = **10**. SD = (18 − 6) ÷ 6 = **2**.
**Why others are wrong:** A is just the most likely value. C is the simple three-point average, (6 + 9 + 18) ÷ 3 = 11. D has no basis.
**Plain English:** The expected duration is 10 days, and about two-thirds of the time it lands within 8 to 12 days.
**Concept:** PERT. **Takeaway:** Notice which formula a question asks for, because simple average and PERT differ.

---

**Q30 | Critical Path | Intermediate | Numerical (select 1)**
Task A (3 days) comes first. B (5 days) and C (7 days) each start after A. D (2 days) starts after both B and C finish. What is the project duration and the slack on B?
A. 10 days; B slack 0
B. 12 days; B slack 2
C. 12 days; B slack 0
D. 17 days; B slack 2

**Correct answer: B.**
**Calculation:** A-B-D = 3 + 5 + 2 = 10. A-C-D = 3 + 7 + 2 = **12** (critical path). B's slack = 12 − 10 = **2**.
**Why others are wrong:** A takes the shorter path. C ignores that B has float. D adds every task, but B and C run in parallel.
**Concept:** CPM and slack. **Takeaway:** Parallel tasks don't add up, and the longest path sets the duration.

---

**Q31 | Schedule Management | Advanced | Numerical (select 1)**
Using the network in Q30, task B slips by 3 days. What is the new project duration?
A. 12 days
B. 13 days
C. 14 days
D. 15 days

**Correct answer: B.**
**Calculation:** B's path becomes 3 + (5 + 3) + 2 = **13**, which is now longer than 12.
**Why others are wrong:** A assumes all slack absorbs the delay, but only 2 days of slack exist. C and D overstate it.
**Takeaway:** A delay delays the project only by the amount that exceeds the slack.

---

## Budget and Earned Value (Q32 to Q35)

**Q32 | Earned Value (CPI, SPI) | Intermediate | Numerical (select 1)**
BAC = $80,000, PV = $40,000, EV = $32,000, AC = $36,000. What are CPI and SPI?
A. CPI 1.13, SPI 1.25
B. CPI 0.89, SPI 0.80
C. CPI 0.80, SPI 0.89
D. CPI 0.89, SPI 1.25

**Correct answer: B.**
**Calculation:** CPI = EV ÷ AC = 32,000 ÷ 36,000 = **0.89**. SPI = EV ÷ PV = 32,000 ÷ 40,000 = **0.80**.
**Why others are wrong:** A and D invert a ratio. C swaps the two indices.
**Plain English:** The project earns about 89 cents per dollar spent and is progressing at 80% of the planned pace, so it is over budget and behind schedule.
**Concept:** CPI and SPI. **Takeaway:** EV is always the numerator, and the denominator is cost for CPI and plan for SPI.

---

**Q33 | Forecasting (EAC, ETC) | Advanced | Numerical (select 1)**
Using Q32's figures, assume the current cost performance will continue. What are EAC and ETC?
A. EAC $84,000; ETC $48,000
B. EAC $90,000; ETC $54,000
C. EAC $80,000; ETC $44,000
D. EAC $90,000; ETC $90,000

**Correct answer: B.**
**Calculation:** EAC = BAC ÷ CPI = 80,000 ÷ 0.8889 = **$90,000**. ETC = EAC − AC = 90,000 − 36,000 = **$54,000**.
**Why others are wrong:** A uses the one-off variance formula, AC + (BAC − EV). C assumes there is no overrun. D forgets to subtract AC.
**Plain English:** At the current rate the project finishes $10,000 over budget, and another $54,000 is needed.
**Concept:** EAC and ETC. **Takeaway:** The wording matters. "Current performance continues" means BAC ÷ CPI.

---

**Q34 | Risk (EMV) | Intermediate | Numerical (select 1)**
Three uncertainties: Risk A: 30% chance of −$10,000. Risk B: 60% chance of −$4,000. Opportunity C: 50% chance of +$2,000. What is the net EMV?
A. −$5,400
B. −$4,400
C. −$3,400
D. +$1,000

**Correct answer: B.**
**Calculation:** −3,000 + (−2,400) + 1,000 = **−$4,400**.
**Why others are wrong:** A leaves out the opportunity. C and D are arithmetic errors.
**Concept:** Expected monetary value. **Takeaway:** EMV sizes contingency but doesn't predict one outcome.

---

**Q35 | Budget | Advanced | True/False**
"Under PMBOK terminology, management reserve is part of the cost baseline."

**Correct answer: False.**
**Why:** Contingency reserve (for known risks) sits inside the cost baseline. Management reserve (for unknown risks) sits outside it, and management must approve its release.
**Concept:** Reserves **[Supplemental]**. **Takeaway:** Know where each reserve sits and who controls it.

---

## Risk (Q36 to Q38)

**Q36 | Risk Management | Intermediate | Matching**
Match each action to the threat response.
1. Switch to a proven vendor instead of using an unproven technology
2. Build against a mock API while waiting for the real one
3. Buy insurance or use a fixed-price contract
4. Hold contingency and take no action unless the risk occurs
a. Transfer
b. Accept
c. Avoid
d. Mitigate

**Correct answer: 1-c, 2-d, 3-a, 4-b.**
**Why:** Avoid removes the cause, mitigate reduces probability or impact, transfer shifts the consequence to a third party, and accept acknowledges the risk.
**Takeaway:** Transfer shifts impact, but the risk still exists.

---

**Q37 | Risk Management | Beginner | MCQ (select 1)**
Using the course scale (score = probability × impact; 1 to 5 low, 6 to 11 medium, 12 to 25 high), a risk with probability 4 and impact 3 is:
A. Low
B. Medium
C. High
D. Cannot be determined

**Correct answer: C.**
**Calculation:** 4 × 3 = 12, which falls in the high band.
**Why others are wrong:** A and B use the wrong band. D is wrong because both inputs are given.
**Concept:** Probability-impact matrix. **Takeaway:** Organizations define their own bands, so check yours.

---

**Q38 | Risk Management | Advanced | Scenario (select 1)**
A risk has a 10% chance of causing a $15,000 loss. Mitigation would cost $6,000. What is the most sensible response?
A. Mitigate at $6,000.
B. Accept actively: keep it in the register, set a trigger, and hold contingency.
C. Delete it from the register.
D. Transfer it by switching vendors regardless of cost.

**Correct answer: B.**
**Reasoning:** EMV = 0.10 × 15,000 = **$1,500**, far below the $6,000 cost of mitigation. Accepting while monitoring is proportionate. Non-money factors such as safety or legal exposure could change this.
**Why others are wrong:** A overspends. C loses the warning trigger. D adds cost without justification.
**Concept:** Cost-effective response. **Takeaway:** Compare response cost with exposure before committing.

---

## Communication, Teams, and Leadership (Q39 to Q44)

**Q39 | Stakeholder Communications | Beginner | MCQ (select 1)**
Which document is the main input when building a communication plan?
A. Closure report
B. Stakeholder register
C. Burndown chart
D. Defect log

**Correct answer: B.**
**Why correct:** It lists who the stakeholders are and what they need.
**Why others are wrong:** A is produced at the end. C and D track progress and quality, not audience needs.
**Takeaway:** Start from the audience, not the channel.

---

**Q40 | Stakeholder Communications | Intermediate | Scenario (select 1)**
Your sponsor says she learned of a two-week delay from a team member, not from you. What is the best response?
A. Explain that it wasn't serious enough to report.
B. Acknowledge the gap, share the facts and recovery options, and agree how and when she wants updates.
C. Send daily emails from now on.
D. Ask the team to stop talking to her.

**Correct answer: B.**
**Reasoning:** The sponsor should hear significant news from you first, with options. Agreeing on her preferences fixes the process, not only the symptom.
**Why others are wrong:** A defends instead of repairing trust. C may overload her. D damages openness.
**Concept:** Escalation and expectations. **Takeaway:** If a stakeholder is surprised, the communication plan failed.

---

**Q41 | Team Management | Beginner | MCQ (select 1)**
Frequent disagreements and friction as roles are tested usually indicate which Tuckman stage?
A. Forming
B. Storming
C. Norming
D. Performing

**Correct answer: B.**
**Why:** Storming is the conflict stage. **Why others are wrong:** Forming is polite and uncertain, norming is cooperative, and performing is efficient.
**Concept:** Team development **[Supplemental]**. **Takeaway:** Storming is normal, so facilitate rather than suppress it.

---

**Q42 | Conflict Resolution | Intermediate | Scenario (select 1)**
Two team members disagree about a design approach and the argument is slowing work. What should you do first?
A. Pick a winner immediately.
B. Talk to each privately to understand their view, then bring them together around shared goals.
C. Ignore it.
D. Report both to HR.

**Correct answer: B.**
**Reasoning:** Private conversations separate facts from emotion and reveal interests. A joint session then agrees on specific actions.
**Why others are wrong:** A may cause resentment. C lets it grow. D is for behavior or policy breaches, not a design disagreement.
**Takeaway:** Understand before deciding.

---

**Q43 | Team Management | Intermediate | Multiple-select (select 3)**
Which three belong in effective delegation?
A. Explain the outcome and why it matters
B. Define success criteria and checkpoints
C. Dictate every step
D. Give authority and resources
E. Disappear until the deadline

**Correct answer: A, B, D.**
**Why correct:** They give clarity, accountability, and capability.
**Why others are wrong:** C is micromanagement. E removes support and visibility.
**Takeaway:** Delegate outcomes and stay accountable.

---

**Q44 | Team Leadership (negotiation) | Advanced | Scenario (select 1)**
The sponsor insists on a feature that would add 3 weeks, with no extra time or money. What is the best approach?
A. Agree and tell the team to work overtime.
B. Refuse.
C. Ask what outcome the feature serves, show the impact on time and cost, and offer options (phase it, swap scope, or add time or budget).
D. Quietly delay other work.

**Correct answer: C.**
**Reasoning:** Negotiate interests, not positions. Options with trade-offs let the sponsor choose.
**Why others are wrong:** A hides the cost. B damages the relationship. D hides the trade-off.
**Concept:** Negotiating priorities. **Takeaway:** Never answer a change with an instant yes or no.

---

## Execution, Monitoring, and Quality (Q45 to Q49)

**Q45 | Project Management (monitoring) | Intermediate | MCQ (select 1)**
CPI is 1.10 and SPI is 0.80. The best interpretation is:
A. Over budget and ahead of schedule
B. Under budget (cost-efficient) and behind schedule
C. Over budget and behind schedule
D. On budget and on schedule

**Correct answer: B.**
**Why:** CPI above 1 means more value per dollar than planned. SPI below 1 means slower than planned progress.
**Takeaway:** This pattern may suggest a capacity problem rather than a cost problem. Check the critical path before adding resources.

---

**Q46 | Quality Assurance | Intermediate | Multiple-select (select 2)**
Which two are quality *assurance* (process) activities?
A. A process audit
B. Running test cases on the booking flow
C. Reviewing and updating the code-review standard
D. Inspecting the final deliverable

**Correct answer: A, C.**
**Why correct:** Both address the process that produces work.
**Why others are wrong:** B and D examine the product, which is quality *control*.
**Concept:** QA vs. QC. **Takeaway:** In many software companies "QA" means testing, so clarify the term.

---

**Q47 | Quality Assessment (Pareto) | Intermediate | Numerical (select 1)**
A defect log shows categories with 30, 25, 20, 15, and 10 defects (100 total). How many of the largest categories are needed to account for more than 70% of the defects?
A. 2
B. 3
C. 4
D. 5

**Correct answer: B.**
**Calculation:** Cumulative: 30%, 55%, **75%**. Three categories exceed 70%.
**Why others are wrong:** Two categories cover only 55%.
**Takeaway:** Fix the biggest categories first.

---

**Q48 | Quality Assessment | Advanced | Scenario (select 1)**
Two days before a launch event, testers find the salon's name misspelled on the home page. It breaks nothing. How would you classify it?
A. High severity, high priority
B. Low severity, high priority
C. High severity, low priority
D. Low severity, low priority

**Correct answer: B.**
**Reasoning:** Severity is the effect on function (none). Priority is the urgency of the fix, which is high because of the visible launch.
**Takeaway:** Severity and priority are separate decisions.

---

**Q49 | Quality Management | Intermediate | MCQ (select 1)**
After a bug is repaired, the team adds a scenario-review step to the checklist so similar bugs are caught before coding in future work. This is a:
A. Defect repair
B. Corrective action
C. Preventive action
D. Scope validation

**Correct answer: C.**
**Why:** It reduces the chance of a *potential* future problem through process change.
**Why others are wrong:** A fixes the item itself. B fixes the cause of the problem that already occurred. D is customer acceptance.
**Note:** If you restated it as fixing the cause of *this* defect, many courses would call it corrective. Exams may blur the two, so read what the question emphasizes.
**Takeaway:** Repair the item, fix the cause, and prevent the recurrence.

---

## Change Management (Q50 to Q51)

**Q50 | Change Management | Beginner | MCQ (select 1)**
After receiving a change request, the first step is:
A. Approve it
B. Reject it
C. Log it and assess the impact on scope, schedule, cost, quality, and risk
D. Implement it informally

**Correct answer: C.**
**Why:** Decisions need impact information. **Why others are wrong:** A, B, and D skip the assessment.
**Takeaway:** Even small changes get logged.

---

**Q51 | Change Management (people side) | Intermediate | Scenario (select 1)**
Staff understand why the new booking tool is needed and want to use it, but they don't know how. Using ADKAR, which element is missing?
A. Awareness
B. Desire
C. Knowledge
D. Reinforcement

**Correct answer: C.**
**Why:** Awareness and Desire are present. Knowledge (how to change) needs training and guides.
**Takeaway:** Diagnose which ADKAR step is blocking people, then address that step.

---

## Agile, Scrum, and Backlogs (Q52 to Q59)

**Q52 | Agile Project Management | Beginner | MCQ (select 1)**
The maximum length of a Daily Scrum is:
A. 5 minutes
B. 15 minutes
C. 30 minutes
D. 1 hour

**Correct answer: B.**
**Concept:** Scrum events (Scrum Guide 2020). **Takeaway:** It is a short planning event for the Developers, not a status meeting for managers.

---

**Q53 | Agile Project Management | Intermediate | Multiple-select (select 3)**
Which three are **required** by the Scrum Guide?
A. A Sprint Goal
B. Story points
C. The Daily Scrum
D. A Definition of Done
E. Planning poker
F. Burndown charts

**Correct answer: A, C, D.**
**Why others are wrong:** B, E, and F are common practices, not Scrum requirements.
**Takeaway:** Exams often test required versus popular practice.

---

**Q54 | Agile Project Management | Advanced | Scenario (select 1)**
Mid-sprint, a VP asks a developer to add a quick task. What should happen?
A. The developer does it quietly.
B. The request goes to the Product Owner, who adds it to the backlog. If it truly can't wait, the PO and Developers renegotiate scope without changing the Sprint Goal.
C. The Scrum Master cancels the sprint.
D. The PM assigns it to another team member.

**Correct answer: B.**
**Reasoning:** The PO orders the backlog, and the Developers own the sprint plan. The Sprint Goal stays stable.
**Why others are wrong:** A bypasses the PO. C is wrong because only the PO can cancel a sprint. D pushes work in from outside.
**Takeaway:** Protect the team's focus and route requests through the backlog.

---

**Q55 | Agile Metrics (velocity forecast) | Intermediate | Numerical (select 1)**
A team completed 21, 24, 18, and 25 points in four sprints. 110 points remain. Using the average of the last three sprints, how many sprints are needed?
A. 4
B. 5
C. 6
D. 7

**Correct answer: B.**
**Calculation:** Average of last three = (24 + 18 + 25) ÷ 3 = 22.33. 110 ÷ 22.33 = 4.93, so round **up** to **5**.
**Why others are wrong:** A rounds down, which would leave work unfinished.
**Takeaway:** Forecasts are ranges, so recalculate after each sprint.

---

**Q56 | Agile Metrics (burndown) | Intermediate | MCQ (select 1)**
A sprint burndown line rises on day 5. The likely cause is:
A. The team finished early.
B. Scope was added or an item was re-estimated upward.
C. The sprint is over.
D. Velocity increased.

**Correct answer: B.**
**Why:** Remaining work went up. **Takeaway:** Check with the PO whether the Sprint Goal is still safe.

---

**Q57 | Backlogs | Intermediate | MCQ (select 1)**
What is the main difference between acceptance criteria and the Definition of Done?
A. They are the same thing.
B. Acceptance criteria are specific to one backlog item. The Definition of Done is a shared quality standard for all items.
C. Acceptance criteria apply to sprints only.
D. The Definition of Done is optional in Scrum.

**Correct answer: B.**
**Why others are wrong:** A is wrong because they differ in scope. C is wrong because they relate to items. D is wrong because the Definition of Done is the Increment's commitment in Scrum.
**Takeaway:** An item must meet both to be truly done.

---

**Q58 | Backlogs (MoSCoW) | Intermediate | MCQ (select 1)**
A feature classed as "Won't have (this time)" means:
A. It will never be built.
B. It is excluded from this release but may be considered later.
C. It is the highest priority.
D. It is already complete.

**Correct answer: B.**
**Takeaway:** Parking an item avoids scope creep without rejecting the idea.

---

**Q59 | Agile (Kanban) | Intermediate | Numerical (select 1)**
A Kanban team has an average of 9 items in progress and finishes 3 items per week. Using Little's Law, the average cycle time is about:
A. 1 week
B. 3 weeks
C. 6 weeks
D. 27 weeks

**Correct answer: B.**
**Calculation:** Cycle time ≈ WIP ÷ throughput = 9 ÷ 3 = **3 weeks**.
**Why others are wrong:** D multiplies instead of dividing.
**Takeaway:** Lowering WIP shortens cycle time.

---

## Closure (Q60)

**Q60 | Project Closure | Intermediate | Scenario (select 1)**
All deliverables are complete. The sponsor says in a hallway, "Looks good to me." What should you do?
A. Close the project, since approval was given.
B. Verify the deliverables against the acceptance criteria and obtain written, signed acceptance, recording any known exceptions.
C. Wait three months.
D. Ask the team to approve it.

**Correct answer: B.**
**Reasoning:** Verbal approval is easily forgotten or disputed. Signed acceptance against agreed criteria ends the discussion.
**Why others are wrong:** A is risky. C delays closure. D is wrong because the customer accepts, not the team.
**Concept:** Formal acceptance. **Takeaway:** If it isn't written down, it isn't approved.

---

## Part 8A Score Sheet

Give yourself 1 point per correct answer. For multiple-select and matching, count the question correct only if every part is right.

| Topic | Questions | Your score |
|---|---|---|
| Initiation and scoping | Q21 to Q27 (7) | ___ |
| Planning, schedule, budget, EVM | Q28 to Q35 (8) | ___ |
| Risk | Q36 to Q38 (3) | ___ |
| Communication, teams, leadership | Q39 to Q44 (6) | ___ |
| Execution and quality | Q45 to Q49 (5) | ___ |
| Change | Q50 to Q51 (2) | ___ |
| Agile and backlogs | Q52 to Q59 (8) | ___ |
| Closure | Q60 (1) | ___ |
| **Total** | **40** | ___ |

**Reading your result:** this isn't an official pass mark. A reasonable self-check is to review any topic where you missed more than a third of the questions.

## Part 8A Checkpoint

Without looking back:
1. What is the difference between PERT and the simple three-point average for O = 6, M = 9, P = 18?
2. Which risk response is "transfer," and does it remove the risk?
3. Name three Scrum elements required by the Scrum Guide and three that are only common practice.

---

# Part 8B: Practice Question Bank (Q61 to Q100)

**Note:** These are original practice questions, not official Google assessment content. Each question uses the same 10-field format as 8A. The score sheet and checkpoint are at the end.

**Formats here:** MCQ, multiple-select (with the number to select stated), true/false, matching, numerical, scenario, short-answer, and practical document questions.

---

## Foundations, Initiation, and Scoping (Q61 to Q67)

**Q61 | Foundations (organizational structures) | Beginner | MCQ (select 1)**
Team members report to both their department head and the project manager. This is a:
A. Functional structure
B. Projectized structure
C. Matrix structure
D. Portfolio

**Correct answer: C.**
**Why correct:** A matrix shares authority between functional managers and the PM.
**Why others are wrong:** In A, authority sits with department heads. In B, the PM has most of the authority. D is a collection of projects, not a reporting structure.
**Concept:** Organizational structures. **Takeaway:** In a matrix, agree priorities and time allocation with the functional managers early.

---

**Q62 | Life cycle | Beginner | True/False**
"The project charter is normally created and signed during the Planning phase."

**Correct answer: False.**
**Why:** The charter authorizes the project, so it belongs to Initiating. Planning builds on it.
**Concept:** Phase documents. **Takeaway:** Without a charter, authority and scope are undefined before planning starts.

---

**Q63 | Scoping (constraints, assumptions, risks, dependencies) | Intermediate | Matching**
Match each statement to its category.
1. "The app must launch before the December 1 holiday season."
2. "The payment provider might change its API."
3. "The owner will supply the service list in week 1."
4. "Testing cannot begin until the booking flow is built."
a. Assumption
b. Dependency
c. Risk
d. Constraint

**Correct answer: 1-d, 2-c, 3-a, 4-b.**
**Why:** A constraint is a fixed limit. A risk is an uncertain future event. An assumption is believed true but unconfirmed. A dependency is a required order between tasks.
**Concept:** Planning terminology. **Takeaway:** Assumptions that turn out false become risks or issues, so record and validate them.

---

**Q64 | Planning (WBS) | Intermediate | MCQ (select 1)**
The "100% rule" for a work breakdown structure (WBS) means:
A. Every task must be 100% complete before the next starts.
B. The WBS includes all the work in scope and nothing outside it.
C. The budget must be fully spent.
D. All stakeholders must approve each work package.

**Correct answer: B.**
**Why:** Completeness cuts both ways: no missing work and no extras. **Why others are wrong:** A, C, and D describe unrelated ideas.
**Concept:** WBS rules. **Takeaway:** Check the WBS against the scope statement line by line.

---

**Q65 | Planning (WBS) | Intermediate | Multiple-select (select 2)**
Which two statements about a WBS are true?
A. It breaks scope into deliverable-focused components.
B. It should include extra work "just in case."
C. Its lowest level (work packages) is small enough to estimate and assign.
D. It shows the dates on which tasks happen.

**Correct answer: A and C.**
**Why others are wrong:** B violates the 100% rule. D describes a schedule, which is built *from* the WBS.
**Concept:** WBS vs. schedule. **Takeaway:** WBS answers "what," and the schedule answers "when."

---

**Q66 | Initiation (charter) | Intermediate | Short answer (practical document)**
List six elements a project charter normally contains, and say who signs it.

**Model answer:** Any six of: project purpose, SMART goals, deliverables or high-level scope, out-of-scope items, budget and timeline, key stakeholders, assumptions, constraints, major risks, success criteria. The sponsor signs it.
**Why:** The charter authorizes the project and records the agreements that later documents depend on.
**Concept:** Project charter. **Takeaway:** A one-page charter agreed quickly beats a long one agreed late.

---

**Q67 | Business case (payback) | Advanced | Numerical (select 1)**
A salon's online booking tool costs $12,000 to build. It is expected to bring a net benefit of $800 per month. What is the simple payback period?
A. 9 months
B. 12 months
C. 15 months
D. 18 months

**Correct answer: C.**
**Calculation:** Payback = cost ÷ monthly net benefit = 12,000 ÷ 800 = **15 months**.
**Why others are wrong:** 12,000 ÷ 1,000 would give 12, and 12,000 ÷ 666 about 18. None matches the given figures.
**Plain English:** It takes 15 months for the benefits to repay the cost. This is a simple measure and ignores the time value of money **[Supplemental]**.
**Concept:** Business case justification. **Takeaway:** Compare options on money and benefits, not only features.

---

## Planning, Estimating, and Schedule (Q68 to Q70)

**Q68 | Project Planning (PERT) | Intermediate | Numerical (select 1)**
A task has O = 5, M = 8, P = 17 days. What is the PERT estimate?
A. 8 days
B. 9 days
C. 10 days
D. 12 days

**Correct answer: B.**
**Calculation:** (5 + 4×8 + 17) ÷ 6 = 54 ÷ 6 = **9**.
**Why others are wrong:** A is just the most likely value. C is the simple average, (5 + 8 + 17) ÷ 3 = 10. D has no basis.
**Concept:** PERT. **Takeaway:** Read which formula the question asks for.

---

**Q69 | Critical Path | Advanced | Numerical (select 1)**
Task A (4 days) is first. B (6 days) and C (3 days) start after A. D (5 days) starts after both B and C. E (2 days) starts after C. F (3 days) starts after both D and E. What is the project duration and the slack on C?
A. 15 days; slack 0
B. 18 days; slack 3
C. 18 days; slack 6
D. 12 days; slack 3

**Correct answer: B.**
**Calculation:** A-B-D-F = 4 + 6 + 5 + 3 = **18** (critical). A-C-D-F = 15. A-C-E-F = 12. C's longest path is 15, so slack = 18 − 15 = **3**. (E's slack would be 18 − 12 = 6.)
**Why others are wrong:** A uses the wrong path. C gives E's slack instead of C's. D takes the shortest path.
**Takeaway:** A task's slack depends on the *longest* path through it.

---

**Q70 | Schedule Compression | Intermediate | Scenario (select 1)**
The sponsor wants an earlier date. The team overlaps UI design and development, which were planned in sequence. This technique is:
A. Crashing, which adds risk of rework
B. Fast-tracking, which adds risk of rework
C. Crashing, which adds cost
D. Resource leveling

**Correct answer: B.**
**Reasoning:** Doing sequential tasks in parallel is fast-tracking. The risk is rework if the design changes after development starts.
**Why others are wrong:** Crashing adds resources, which raises cost. Resource leveling smooths workloads and can lengthen the schedule.
**Takeaway:** Tell the sponsor the price of speed: crashing costs money, fast-tracking costs risk.

---

## Stakeholders (Q71 to Q72)

**Q71 | Stakeholder Analysis | Intermediate | True/False**
"Once a stakeholder is supportive, they no longer need active engagement."

**Correct answer: False.**
**Why:** Attitudes and influence change. A supportive stakeholder can become neutral or resistant if they feel uninformed.
**Concept:** Ongoing stakeholder engagement. **Takeaway:** Review the stakeholder register regularly.

---

**Q72 | RACI | Beginner | MCQ (select 1)**
In a RACI matrix, a person who gives two-way input before a decision is:
A. Responsible
B. Accountable
C. Consulted
D. Informed

**Correct answer: C.**
**Why:** Consulted means two-way input. **Why others are wrong:** Responsible does the work, Accountable owns the outcome, Informed receives one-way updates.
**Takeaway:** Stakeholders who are only informed can feel ignored, so check whether they should be consulted.

---

## Risk (Q73 to Q75)

**Q73 | Risk vs. Issue | Intermediate | Multiple-select (select 2)**
Which two are **issues**, not risks?
A. "The vendor may deliver late."
B. "The test server crashed yesterday and testing is blocked."
C. "A key developer might resign."
D. "Two team members' ongoing conflict is delaying handoffs."

**Correct answer: B and D.**
**Why correct:** Both are already happening and need action, an owner, and a due date.
**Why others are wrong:** A and C are uncertain future events.
**Concept:** Risk register vs. issue log. **Takeaway:** When a risk occurs, move it to the issue log.

---

**Q74 | Risk Management | Intermediate | Scenario (select 1)**
To reduce a schedule risk, you add an outside contractor who doesn't know the codebase. The contractor's inexperience is now a new risk. This is a:
A. Residual risk
B. Secondary risk
C. Trigger
D. Issue

**Correct answer: B.**
**Why:** A secondary risk is created by the response itself. **Why others are wrong:** A residual risk is what remains of the *original* risk. A trigger is a warning sign. An issue is a problem already happening.
**Takeaway:** Check each response for new risks it may create.

---

**Q75 | Risk (EMV) | Advanced | Numerical (select 1)**
R1: 40% chance of −$5,000. R2: 25% chance of −$12,000. R3: 10% chance of −$20,000. Which has the largest expected loss, and what is the total EMV?
A. R1; −$7,000
B. R2; −$7,000
C. R3; −$7,000
D. R2; −$37,000

**Correct answer: B.**
**Calculation:** R1 = −$2,000. R2 = −$3,000. R3 = −$2,000. Total = **−$7,000**. R2 is the largest.
**Why others are wrong:** D adds the raw impacts instead of weighting by probability.
**Plain English:** On average these risks cost about $7,000, a basis for contingency, not a prediction.
**Takeaway:** R3 has the biggest impact but not the biggest expected loss, so also watch severe, low-probability risks separately.

---

## Earned Value (Q76 to Q78)

**Q76 | Earned Value (CV, SV) | Intermediate | Numerical (select 1)**
EV = $45,000, PV = $50,000, AC = $42,000. What are CV and SV, and what do they mean?
A. CV +$3,000 and SV −$5,000: under budget, behind schedule
B. CV −$3,000 and SV +$5,000: over budget, ahead of schedule
C. CV +$3,000 and SV +$5,000: under budget, ahead of schedule
D. CV −$5,000 and SV +$3,000: over budget, behind schedule

**Correct answer: A.**
**Calculation:** CV = EV − AC = 45,000 − 42,000 = **+3,000**. SV = EV − PV = 45,000 − 50,000 = **−5,000**.
**Why others are wrong:** The other options flip a sign or swap the two variances.
**Takeaway:** Positive is good and negative is bad for both variances. Then check the critical path, because SV ignores it.

---

**Q77 | Earned Value (EAC, VAC) | Advanced | Numerical (select 1)**
BAC = $120,000, EV = $40,000, AC = $50,000. The overrun was a one-off event, and the remaining work will run to plan. What is EAC and the variance at completion (VAC = BAC − EAC)?
A. EAC $130,000; VAC −$10,000
B. EAC $150,000; VAC −$30,000
C. EAC $120,000; VAC $0
D. EAC $130,000; VAC +$10,000

**Correct answer: A.**
**Calculation:** EAC = AC + (BAC − EV) = 50,000 + 80,000 = **$130,000**. VAC = 120,000 − 130,000 = **−$10,000**.
**Why others are wrong:** B uses BAC ÷ CPI (CPI = 0.8, giving $150,000), which assumes the poor performance continues. C ignores the overrun. D has the wrong sign.
**Takeaway:** "One-off" and "continues" lead to different formulas, so read the wording.

---

**Q78 | Earned Value (percent complete, CPI) | Intermediate | Numerical (select 1)**
BAC = $60,000, the project is 35% complete, and AC = $24,000. What is CPI?
A. 0.75
B. 0.88
C. 1.14
D. 1.43

**Correct answer: B.**
**Calculation:** EV = 35% × 60,000 = **$21,000**. CPI = EV ÷ AC = 21,000 ÷ 24,000 = **0.875**, about 0.88.
**Why others are wrong:** C is AC ÷ EV (inverted). A and D come from wrong inputs.
**Plain English:** About 88 cents of planned value earned for each dollar spent.
**Takeaway:** Convert percent complete into EV before computing indices.

---

## Communication (Q79 to Q81)

**Q79 | Stakeholder Communications | Intermediate | Short answer (practical)**
Write a two-sentence, bottom-line-first opening for a sponsor update. The project is two weeks behind on the critical path and you have three recovery options.

**Model answer:** "The project is two weeks behind on the critical path, and I need your decision on one of three recovery options by Friday. I recommend option B (defer two low-priority features), which protects the launch date and costs nothing extra."
**Why it works:** It leads with status, the decision needed, and a recommendation, and details can follow.
**Concept:** Writing for executives. **Takeaway:** Bottom line first, then context, options, and the ask.

---

**Q80 | Stakeholder Communications | Beginner | MCQ (select 1)**
A team posts weekly progress on a shared dashboard that stakeholders open when they choose. This is:
A. Push communication
B. Pull communication
C. Interactive communication
D. Formal escalation

**Correct answer: B.**
**Why:** Pull means the audience retrieves information. **Why others are wrong:** Push is sent to people (email). Interactive is two-way (meetings).
**Takeaway:** Pair pull channels with a short push summary, so important news isn't missed.

---

**Q81 | Stakeholder Communications | Advanced | Scenario (select 1)**
A remote team in three time zones keeps missing decisions made in live calls. What is the best fix?
A. Hold more live calls.
B. Record every decision in a shared decision log with owner and date, and send a short written summary after each call.
C. Tell people to attend all calls.
D. Make decisions only by email.

**Correct answer: B.**
**Reasoning:** Written, shared records make decisions visible regardless of who attended or when.
**Why others are wrong:** A and C burden people across time zones. D removes useful real-time discussion.
**Takeaway:** If it isn't written down, remote teammates don't have it.

---

## Teams, Leadership, and Roles (Q82 to Q84)

**Q82 | Team Management | Intermediate | Scenario (select 1)**
A capable team member rarely speaks in meetings, and good ideas surface only afterwards in chat. What should you do?
A. Ignore it.
B. Change the meeting format (invite input in rounds, ask for written ideas beforehand) and check privately how they prefer to contribute.
C. Tell them to speak up.
D. Stop inviting them.

**Correct answer: B.**
**Reasoning:** Facilitation changes lower the barrier, and the private check shows what works for them.
**Why others are wrong:** A wastes ideas. C ignores why they stay quiet. D excludes a contributor.
**Takeaway:** Quiet doesn't mean disengaged.

---

**Q83 | Team Leadership (escalation) | Advanced | MCQ (select 1)**
A vendor hasn't responded for two weeks and a critical task is at risk. Which escalation message is best?
A. "The vendor is useless. Please fix this."
B. "The vendor missed the agreed date of the 10th. Impact: the critical path slips 1 day for each day of delay. I've emailed twice and called once. Could you contact their senior contact this week? If there's no reply by Friday, I recommend activating the backup plan."
C. "FYI, things are a bit behind."
D. No message, since escalation signals failure.

**Correct answer: B.**
**Why:** It states facts, impact, what you tried, a specific ask, and a recommendation. **Why others are wrong:** A blames, C is vague, and D hides a problem until it's too late.
**Takeaway:** Escalate early with facts and a proposal.

---

**Q84 | Roles | Intermediate | Matching**
Match each role to its main focus.
1. Project manager
2. Product Owner
3. Scrum Master
4. Technical lead
5. People manager
a. Helps the team understand and use Scrum effectively; helps remove impediments
b. Delivers a defined project on time, within scope and budget; manages risks, stakeholders, and change
c. Orders the product backlog to maximize value
d. Owns technical design and standards
e. Handles performance reviews and career development

**Correct answer: 1-b, 2-c, 3-a, 4-d, 5-e.**
**Note:** Titles and duties vary by company, and in Agile teams some PM duties are shared.
**Takeaway:** Know who decides what, so you don't step on another role.

---

## Quality (Q85 to Q88)

**Q85 | Quality Management (cost of quality) | Intermediate | Matching**
Match each cost to its category **[Supplemental]**.
1. Training developers on code standards
2. Running system tests
3. Rework after defects are found in testing
4. Refunds after customers hit a double-booking bug
a. External failure
b. Prevention
c. Internal failure
d. Appraisal

**Correct answer: 1-b, 2-d, 3-c, 4-a.**
**Why:** Prevention avoids defects, appraisal finds them, internal failure is found before delivery, and external failure is found by customers.
**Takeaway:** Failures found by customers are usually the most expensive.

---

**Q86 | Quality Assessment (tools) | Beginner | MCQ (select 1)**
The team wants to rank causes of defects by how often they occur, to decide what to fix first. Which tool fits best?
A. Fishbone diagram
B. Pareto chart
C. Gantt chart
D. RACI matrix

**Correct answer: B.**
**Why:** A Pareto chart ranks categories by frequency. **Why others are wrong:** A fishbone groups possible causes. C shows the schedule. D assigns roles.
**Takeaway:** Fishbone helps find causes, and Pareto helps prioritize them.

---

**Q87 | Quality Assessment (pass rate) | Advanced | Numerical (select 1)**
A system test has 48 test cases. 42 pass. The target is a pass rate of at least 95%. What is the pass rate, and how many more tests must pass to reach the target?
A. 87.5%; 4 more
B. 87.5%; 3 more
C. 85%; 5 more
D. 90%; 2 more

**Correct answer: A.**
**Calculation:** 42 ÷ 48 = **87.5%**. 95% × 48 = 45.6, so at least **46** must pass. 46 − 42 = **4 more**. (45 would give 93.75%, below target.)
**Why others are wrong:** B stops at 45. C and D use wrong percentages.
**Takeaway:** Round *up* when a target must be met.

---

**Q88 | Quality Management | Advanced | Scenario (select 1)**
The sponsor, under date pressure, tells you to skip regression testing. What is the best response?
A. Skip it quietly.
B. Refuse and stop the project.
C. Explain the risk, offer options (risk-based regression on the most critical areas, a short date change, or deferring low-priority features), and ask the sponsor to decide and record it.
D. Run it without telling anyone.

**Correct answer: C.**
**Reasoning:** Quality trade-offs must be visible and decided by the right person. Risk-based testing is a legitimate way to compress effort.
**Why others are wrong:** A hides risk. B is rigid. D ignores the sponsor's authority over the trade-off.
**Takeaway:** Trade scope or time openly, never hidden quality.

---

## Change Management (Q89 to Q90)

**Q89 | Change Management | Intermediate | MCQ (select 1)**
A critical change must be decided within a day. The best approach is:
A. Skip documentation.
B. Use an expedited path: fast impact assessment, a named approver, and full documentation straight afterward.
C. Wait for the monthly change board.
D. Let the team implement and report later.

**Correct answer: B.**
**Why:** Urgency speeds the process, not skips it. **Takeaway:** Agree the expedited path before you need it.

---

**Q90 | Change Management (thresholds) | Advanced | Scenario (select 1)**
Your change plan lets the PM approve changes under 2 days of effort and no cost. Request X: 1.5 days, no cost. Request Y: 1 day, $300 cost. What should you do?
A. Approve both.
B. Approve X yourself. Send Y to the sponsor.
C. Send both to the sponsor.
D. Reject both.

**Correct answer: B.**
**Reasoning:** X fits the PM threshold. Y involves cost, so it exceeds the threshold.
**Why others are wrong:** A exceeds your authority for Y. C adds needless delay for X. D rejects without assessing.
**Takeaway:** Log both, and follow the thresholds in your change plan.

---

## Agile, Scrum, and Backlogs (Q91 to Q98)

**Q91 | Agile Project Management | Beginner | MCQ (select 1)**
The purpose of the Sprint Retrospective is to:
A. Demonstrate the Increment to stakeholders
B. Plan how the team can improve its way of working
C. Plan the next sprint's backlog items
D. Report status to managers

**Correct answer: B.**
**Why others are wrong:** A is the Sprint Review. C is Sprint Planning. D is not its purpose.
**Takeaway:** Review inspects the *product*, and the retrospective inspects the *process*.

---

**Q92 | Agile Project Management | Intermediate | True/False**
"The Scrum Master assigns tasks to the Developers."

**Correct answer: False.**
**Why:** Developers plan and own their work. The Scrum Master coaches, facilitates, and helps remove impediments.
**Takeaway:** Don't confuse Scrum Master with team lead or manager.

---

**Q93 | Agile Metrics (velocity) | Intermediate | Numerical (select 1)**
A team committed to items of 8, 5, 5, 3, and 2 points. It finished the 8, one 5, and the 3. The second 5-point item is 80% done, and the 2-point item wasn't started. What is the sprint velocity?
A. 16
B. 17
C. 19
D. 23

**Correct answer: A.**
**Calculation:** 8 + 5 + 3 = **16**. Partial work counts as zero.
**Why others are wrong:** B and C credit partial work. D is the total committed.
**Takeaway:** Only items meeting the Definition of Done count.

---

**Q94 | Agile Project Management | Advanced | Scenario (select 1)**
Developers finish all Sprint Backlog items three days early. What should they do?
A. Stop working until the sprint ends.
B. Talk with the Product Owner about pulling in more work that supports the Sprint Goal, and use spare time for improvement.
C. Cancel the sprint.
D. Start unrelated work without telling anyone.

**Correct answer: B.**
**Reasoning:** Scope under the Sprint Goal can be adjusted by agreement with the PO.
**Why others are wrong:** A wastes capacity. C is only for an obsolete goal and only the PO can do it. D bypasses the PO.
**Takeaway:** Finishing early is also a signal to revisit estimates in the retrospective.

---

**Q95 | Agile (Kanban) | Intermediate | MCQ (select 1)**
In a Kanban team, the "In Progress" column has reached its WIP limit. A developer finishes their item. What is the best action?
A. Pull a new item immediately, ignoring the limit.
B. Help move existing items forward (for example, review work) before pulling something new.
C. Raise the limit.
D. Stop work for the day.

**Correct answer: B.**
**Why:** WIP limits encourage finishing over starting. If a column is full, the bottleneck is downstream. **Takeaway:** Fix the flow before adding work.

---

**Q96 | Agile vs. Predictive | Advanced | Scenario (select 1)**
A client signs a fixed-price contract with a fixed deadline, but the interface details are unclear and expected to evolve. The best approach is likely:
A. Pure waterfall
B. Pure Scrum with no fixed scope
C. Hybrid: fixed milestones and budget, with iterative sprints for interface details
D. Kanban only

**Correct answer: C.**
**Reasoning:** The contract needs predictability, while the unclear interface needs iteration.
**Why others are wrong:** A ignores uncertainty. B conflicts with the contract. D lacks fixed milestones.
**Takeaway:** Choose by uncertainty and contract constraints, not fashion.

---

**Q97 | Backlogs (acceptance criteria) | Intermediate | Short answer (practical)**
Write Given/When/Then acceptance criteria for the story: "As a customer, I want to reset my password so that I can regain access."

**Model answer:** *Given* I'm on the login page, *when* I choose "Forgot password" and enter my registered email, *then* I receive a reset link valid for 30 minutes. *Given* I open a valid link, *when* I set a new password meeting the rules, *then* I can log in and the link no longer works. *Given* the link is older than 30 minutes, *when* I open it, *then* I see a message and can request a new one.
**Concept:** Acceptance criteria. **Takeaway:** Each criterion should be testable with a clear pass or fail.

---

**Q98 | Backlogs (INVEST) | Intermediate | Multiple-select (select 3)**
Which three describe a well-formed user story (INVEST)?
A. Small enough to finish within a sprint
B. Testable
C. Valuable to a user or the business
D. Dependent on six other unfinished stories
E. Described only as "improve the system"

**Correct answer: A, B, C.**
**Why others are wrong:** D breaks "Independent." E is too vague to estimate or test.
**Takeaway:** INVEST is a common practice, not a Scrum requirement.

---

## Closure (Q99 to Q100)

**Q99 | Project Closure | Intermediate | Multiple-select (select 3)**
Which three are closure activities?
A. Obtaining formal acceptance
B. Archiving project documents
C. Holding a lessons-learned session
D. Adding new features to the scope
E. Deleting all records to save space

**Correct answer: A, B, C.**
**Why others are wrong:** D is a change handled before acceptance or in a new phase. E destroys information future teams need.
**Takeaway:** Plan closure tasks in the schedule so they aren't skipped.

---

**Q100 | Project Closure (reporting) | Advanced | Numerical (select 1)**
Original baseline: $50,000. Approved changes: +$4,000 and −$1,500. Actual cost: $52,300. How should the final cost be reported?
A. $2,300 over the original baseline and $200 under the revised budget
B. $2,300 under the revised budget
C. $200 over the original baseline
D. On budget in every comparison

**Correct answer: A.**
**Calculation:** Revised budget = 50,000 + 4,000 − 1,500 = **$52,500**. Against revised: 52,500 − 52,300 = **+$200 under**. Against original: 52,300 − 50,000 = **$2,300 over**.
**Why others are wrong:** B, C, and D each mix up the baselines.
**Takeaway:** Report both comparisons and explain the approved changes, so nobody misreads the result.

---

## Part 8B Score Sheet

Give yourself 1 point per correct answer. For multiple-select and matching, count the question correct only if every part is right. For short-answer questions, count it correct if your answer covers the main points of the model answer.

| Topic | Questions | Your score |
|---|---|---|
| Foundations, initiation, scoping | Q61 to Q67 (7) | ___ |
| Planning and schedule | Q68 to Q70 (3) | ___ |
| Stakeholders | Q71 to Q72 (2) | ___ |
| Risk | Q73 to Q75 (3) | ___ |
| Earned value | Q76 to Q78 (3) | ___ |
| Communication | Q79 to Q81 (3) | ___ |
| Teams, leadership, roles | Q82 to Q84 (3) | ___ |
| Quality | Q85 to Q88 (4) | ___ |
| Change | Q89 to Q90 (2) | ___ |
| Agile and backlogs | Q91 to Q98 (8) | ___ |
| Closure | Q99 to Q100 (2) | ___ |
| **Total** | **40** | ___ |

**Reading your result:** this isn't an official pass mark. Review any topic where you missed more than a third of the questions, and re-read the matching Part.

**Running total:** Q1 to Q100 are now done (Part 1: 20, 8A: 40, 8B: 40).

## Part 8B Checkpoint

Without looking back:
1. Q69's network has several paths. How do you find a task's slack?
2. When is EAC = AC + (BAC − EV) the right formula, and when is it BAC ÷ CPI?
3. Which Scrum event inspects the product, and which inspects the process?

---
# Part 8C: Practice Question Bank (Q101 to Q140)

**Note:** These are original practice questions, not official Google assessment content. The 10-field format is the same as in 8A and 8B. This installment has more scenario, numerical, and Agile questions. Questions on web presence and interviewing (Skills 19 and 20) come after Part 9 has taught them, in 8D and 8E.

---

## Foundations, Initiation, and Scoping (Q101 to Q106)

**Q101 | Foundations (project, program, portfolio) | Beginner | MCQ (select 1)**
A company reviews all its proposed initiatives and decides which ones to fund based on its strategy. This is:
A. Project management
B. Program management
C. Portfolio management
D. Operations management

**Correct answer: C.**
**Why correct:** Portfolio management selects and balances all initiatives against strategy.
**Why others are wrong:** A manages one effort. B manages related projects with a shared goal. D runs ongoing work.
**Concept:** Levels of work. **Takeaway:** Know which level your decisions sit at, because priorities and reporting lines differ.

---

**Q102 | Business case (options) | Intermediate | Numerical (select 1)**
Option A costs $20,000 and brings a net benefit of $1,500 per month. Option B costs $8,000 and brings $500 per month. Which statement is correct?
A. B has the shorter payback and the higher 24-month net benefit.
B. A has the shorter payback (about 13.3 months) and the higher 24-month net benefit ($16,000 vs. $4,000).
C. A has the shorter payback, but B has the higher 24-month net benefit.
D. Both have the same payback.

**Correct answer: B.**
**Calculation:** Payback A = 20,000 ÷ 1,500 = **13.3 months**. Payback B = 8,000 ÷ 500 = **16 months**. Net benefit over 24 months: A = 36,000 − 20,000 = **$16,000**. B = 12,000 − 8,000 = **$4,000**.
**Why others are wrong:** A, C, and D each contradict the calculations.
**Plain English:** Option A costs more up front but pays back sooner and earns more over two years.
**Concept:** Comparing options in a business case. **Takeaway:** The cheapest option is not always the best value.

---

**Q103 | Project Scoping | Intermediate | MCQ (select 1)**
A stakeholder says, "We need a chatbot on the website." What should the project manager do first?
A. Add a chatbot to the scope.
B. Ask what problem the chatbot should solve and how success would be measured.
C. Refuse, because chatbots are risky.
D. Ask the developer how long it takes.

**Correct answer: B.**
**Why correct:** Stakeholders often describe solutions. Scope should start from the problem, so you can check whether the solution fits and define measurable criteria.
**Why others are wrong:** A commits before understanding the need. C is premature. D estimates a solution that may be wrong.
**Takeaway:** Ask "What problem would that solve?"

---

**Q104 | Scope statement | Intermediate | Multiple-select (select 3)**
Which three normally belong in a project scope statement?
A. In-scope deliverables
B. Out-of-scope exclusions
C. Acceptance criteria
D. An individual team member's performance review
E. Notes from yesterday's stand-up

**Correct answer: A, B, C.**
**Why others are wrong:** D belongs to the people manager's process. E is a short-lived team record.
**Concept:** Scope statement contents. **Takeaway:** The scope statement is the reference you return to when disputes arise.

---

**Q105 | Charter | Beginner | True/False**
"The project charter formally authorizes the project and gives the project manager authority to apply resources."

**Correct answer: True.**
**Why:** The sponsor's signature on the charter is the formal start. Without it, authority and scope are undefined. This is consistent with PMBOK language **[Supplemental]**.
**Takeaway:** If the sponsor says "just start," offer a one-page charter to sign.

---

**Q106 | Scope (practical document) | Intermediate | Short answer**
For a restaurant table-reservation app, write one out-of-scope statement and one measurable acceptance criterion.

**Model answer:** *Out of scope:* "Online food ordering and delivery are not included." *Acceptance criterion:* "A customer can reserve a table for 2 to 8 people in under 2 minutes in user testing, and receives a confirmation email within 1 minute." Any similar pair that is explicit and testable is fine.
**Why it works:** The exclusion prevents assumptions, and the criterion has a pass or fail test.
**Concept:** Scope boundaries and acceptance criteria. **Takeaway:** Include numbers or tests, never adjectives.

---

## Planning and Schedule (Q107 to Q111)

**Q107 | Dependencies | Intermediate | Matching**
Match each example to its dependency type.
1. Painting cannot start until sanding finishes.
2. Testing starts when coding starts.
3. Documentation cannot finish until testing finishes.
4. The old system cannot be shut down until the new system has started.
a. Start-to-start
b. Finish-to-start
c. Finish-to-finish
d. Start-to-finish

**Correct answer: 1-b, 2-a, 3-c, 4-d.**
**Why:** Finish-to-start is the most common. Start-to-finish is rare and easy to confuse with finish-to-start.
**Takeaway:** Draw the dependency, because wrong types produce wrong schedules.

---

**Q108 | Critical Path | Intermediate | Numerical (select 1)**
Task A (2 days) is first. B (4 days) and C (6 days) start after A. D (3 days) starts after both B and C. E (2 days) starts after D. What is the project duration and the slack on B?
A. 11 days; B slack 0
B. 13 days; B slack 2
C. 13 days; B slack 4
D. 17 days; B slack 0

**Correct answer: B.**
**Calculation:** A-B-D-E = 2 + 4 + 3 + 2 = 11. A-C-D-E = 2 + 6 + 3 + 2 = **13** (critical). B's slack = 13 − 11 = **2**.
**Why others are wrong:** A uses the shorter path. C confuses B's duration with its slack. D adds B and C as though they ran in sequence.
**Takeaway:** Parallel tasks don't add up. The longest path sets the duration.

---

**Q109 | Slack | Intermediate | Numerical (select 1)**
A task has a duration of 4 days, an earliest start (ES) of day 5, and a latest finish (LF) of day 12. What is its slack?
A. 0 days
B. 3 days
C. 4 days
D. 7 days

**Correct answer: B.**
**Calculation:** EF = 5 + 4 = 9. LS = 12 − 4 = 8. Slack = LS − ES = 8 − 5 = **3** (or LF − EF = 12 − 9 = 3).
**Why others are wrong:** A would mean the task is critical. C is the duration. D mixes ES and LF.
**Takeaway:** Slack tells you how much a task can slip without moving the end date.

---

**Q110 | PERT | Advanced | Numerical (select 1)**
A task has O = 10, M = 14, P = 30 days. Which statement is correct?
A. Estimate 14 days; the range is 10 to 30.
B. Estimate 16 days; about 68% likely to finish between 12.7 and 19.3 days.
C. Estimate 18 days; the range is 16 to 20.
D. Estimate 16 days; about 68% likely to finish between 6 and 26 days.

**Correct answer: B.**
**Calculation:** PERT = (10 + 4×14 + 30) ÷ 6 = 96 ÷ 6 = **16**. SD = (30 − 10) ÷ 6 = **3.33**. One SD each side: 16 ± 3.33 = **12.7 to 19.3**.
**Why others are wrong:** A uses the most likely value and the full range. C has no basis. D is 3 SDs (about 99.7%), not 1.
**Takeaway:** A wide O-to-P range means high uncertainty, so add buffer or reduce the unknowns.

---

**Q111 | Resource planning | Intermediate | Scenario (select 1)**
Your developer is assigned 50 hours of work in a 40-hour week. Some of the work is on the critical path, and some tasks have slack. What is the best action?
A. Ask for overtime every week.
B. Rebalance: keep critical-path work on schedule, shift non-critical tasks into their slack, and add help or reduce scope if needed.
C. Ignore it, because estimates are padded.
D. Cancel the non-critical tasks.

**Correct answer: B.**
**Reasoning:** Resource leveling uses slack to smooth workloads without delaying the end date. Chronic overtime hurts quality and morale.
**Why others are wrong:** A hides the problem. C assumes without checking. D removes scope without approval.
**Takeaway:** Check workloads against the schedule every week.

---

## Budget and Earned Value (Q112 to Q117)

**Q112 | Budget variance | Beginner | Numerical (select 1)**
The budget for a task was $12,000 and the actual cost was $13,800. What are the budget variance and its percentage?
A. +$1,800; +15%
B. −$1,800; −15%
C. −$1,800; −13%
D. −$13,800; −115%

**Correct answer: B.**
**Calculation:** Budget − Actual = 12,000 − 13,800 = **−1,800**. 1,800 ÷ 12,000 = **15%**.
**Why others are wrong:** A has the wrong sign. C divides by the actual cost. D is nonsense.
**Plain English:** The task is 15% over budget.
**Takeaway:** Negative means over budget.

---

**Q113 | Earned Value (CV, CPI) | Intermediate | Numerical (select 1)**
BAC = $200,000, PV = $100,000, EV = $90,000, AC = $100,000. What are CV and CPI?
A. CV −$10,000; CPI 0.90
B. CV +$10,000; CPI 1.11
C. CV −$10,000; CPI 1.11
D. CV +$10,000; CPI 0.90

**Correct answer: A.**
**Calculation:** CV = EV − AC = 90,000 − 100,000 = **−10,000**. CPI = EV ÷ AC = 90,000 ÷ 100,000 = **0.90**.
**Why others are wrong:** B and C invert the ratio or the sign.
**Plain English:** The project is over budget, earning 90 cents for each dollar spent.
**Takeaway:** EV is always the starting point.

---

**Q114 | Earned Value (EAC, ETC) | Advanced | Numerical (select 1)**
Using Q113's figures, assume current cost performance will continue. What are EAC and ETC?
A. EAC $210,000; ETC $110,000
B. EAC $222,222; ETC $122,222
C. EAC $222,222; ETC $222,222
D. EAC $200,000; ETC $100,000

**Correct answer: B.**
**Calculation:** EAC = BAC ÷ CPI = 200,000 ÷ 0.90 = **$222,222**. ETC = EAC − AC = 222,222 − 100,000 = **$122,222**.
**Why others are wrong:** A uses the one-off formula (AC + BAC − EV). C forgets to subtract AC. D assumes no overrun.
**Plain English:** At this rate the project finishes about $22,000 over budget.
**Takeaway:** "Current performance continues" means BAC ÷ CPI.

---

**Q115 | Earned Value (terms) | Beginner | Matching**
Match each term to its meaning.
1. PV (planned value)
2. EV (earned value)
3. AC (actual cost)
4. BAC (budget at completion)
a. Budgeted value of the work actually completed
b. Money actually spent so far
c. Budgeted value of the work scheduled to be done by now
d. The total approved budget for the project

**Correct answer: 1-c, 2-a, 3-b, 4-d.**
**Takeaway:** PV is the plan, EV is the progress, and AC is the spending. All three use the same baseline.

---

**Q116 | Earned Value (SV) | Intermediate | True/False**
"A negative schedule variance (SV) always means the project end date will slip."

**Correct answer: False.**
**Why:** SV is measured in money and ignores the critical path. If the late work has slack, the end date may be safe. If it is on the critical path, the end date is at risk.
**Takeaway:** Check the critical path alongside SPI.

---

**Q117 | Risk (contingency from EMV) | Advanced | Numerical (select 1)**
Three risks: 20% chance of −$15,000; 50% chance of −$4,000; 10% chance of −$30,000. A $6,000 contingency has been set aside. Which statement is correct?
A. $6,000 is enough.
B. The total EMV is −$8,000, so $6,000 is $2,000 short.
C. The total EMV is −$49,000.
D. The total EMV is −$5,000.

**Correct answer: B.**
**Calculation:** 0.20 × 15,000 = 3,000. 0.50 × 4,000 = 2,000. 0.10 × 30,000 = 3,000. Total = **$8,000**.
**Why others are wrong:** C adds raw impacts without weighting. D has no basis.
**Plain English:** On average these risks cost $8,000. Contingency of $6,000 is thin. Raise it, reduce the risks, or tell the sponsor about the gap.
**Takeaway:** Size contingency from risks, not from habit.

---

## Risk (Q118 to Q120)

**Q118 | Risk (opportunity responses) | Advanced | Matching [Supplemental]**
Match each action to the response for a **positive** risk (opportunity).
1. Assign your best developer so that an early-delivery bonus is certain to be earned
2. Add resources to increase the size of the benefit
3. Partner with a vendor who has expertise, so both parties capture the benefit
4. Take the benefit if it happens but do nothing to pursue it
a. Accept
b. Exploit
c. Share
d. Enhance

**Correct answer: 1-b, 2-d, 3-c, 4-a.**
**Why:** Exploit makes the opportunity certain, enhance increases probability or impact, share involves a partner, and accept takes no active step.
**Takeaway:** The four threat responses have positive counterparts.

---

**Q119 | Risk Management | Intermediate | Scenario (select 1)**
Your risk register lists "payment sandbox late" with the trigger "no sandbox by end of week 4." It is now the end of week 4, and there is no sandbox. What should you do?
A. Wait another week.
B. Treat it as an issue: log it, activate the contingency plan, assign an owner, and inform the sponsor.
C. Delete the risk.
D. Blame the vendor in the status report.

**Correct answer: B.**
**Reasoning:** The trigger has fired, so the risk is now happening. A pre-planned response should start immediately.
**Why others are wrong:** A wastes the early warning. C erases the record. D skips action.
**Takeaway:** Plan the response and the trigger before the risk occurs.

---

**Q120 | Probability-impact matrix | Intermediate | Multiple-select (select 2)**
Using the scale (score = probability × impact; 1 to 5 low, 6 to 11 medium, 12 to 25 high), which two risks are **high**?
A. R-A: probability 5, impact 2
B. R-B: probability 3, impact 4
C. R-C: probability 2, impact 5
D. R-D: probability 4, impact 4

**Correct answer: B and D.**
**Calculation:** A = 10 (medium). B = **12** (high). C = 10 (medium). D = **16** (high).
**Takeaway:** R-C (low probability, severe impact) is medium by score but may still need a contingency plan. Don't rely on the number alone.

---

## Stakeholders and Communication (Q121 to Q124)

**Q121 | Stakeholder engagement | Intermediate | Scenario (select 1)**
Your sponsor rarely answers emails, and approvals are stalling. What is the best approach?
A. Keep sending longer emails.
B. Ask how she prefers to be contacted, make each request short with a clear decision and deadline, and agree a delegate for routine approvals.
C. Proceed without approvals.
D. Complain to her manager.

**Correct answer: B.**
**Reasoning:** Fix the communication design. A preferred channel, short specific asks, and a delegate make it easy to respond.
**Why others are wrong:** A adds to the overload. C breaks governance. D damages the relationship before you've tried to fix the process.
**Takeaway:** Make it easy for busy people to say yes.

---

**Q122 | Communication channels | Intermediate | Numerical (select 1)**
The number of communication channels is n(n − 1) ÷ 2. A team of 8 people grows to 10 people. How many channels exist with 10 people, and how many were added? **[Supplemental]**
A. 45 channels; 2 added
B. 45 channels; 17 added
C. 90 channels; 62 added
D. 28 channels; 17 added

**Correct answer: B.**
**Calculation:** 8 people: 8 × 7 ÷ 2 = **28**. 10 people: 10 × 9 ÷ 2 = **45**. Added = 45 − 28 = **17**.
**Why others are wrong:** A counts people, not channels. C forgets to divide by 2. D gives the old total.
**Takeaway:** Communication complexity grows faster than team size, so plan communication as teams grow.

---

**Q123 | RACI (practical document) | Intermediate | Short answer**
Assign R, A, C, and I for the task "approve final UI design" among the Sponsor, Designer, Project Manager, and Developer.

**Model answer:** *Sponsor: A* (final approval). *Designer: R* (prepares and presents the design). *Project Manager: C or R* (coordinates the review). *Developer: C* (confirms feasibility). Anyone not directly involved is *I*. Variations are acceptable if there is **exactly one A**.
**Why:** One accountable person prevents both "everyone thought someone else decided" and disputes about who has the final say.
**Takeaway:** Check every row for exactly one A.

---

**Q124 | Communication (channel choice) | Intermediate | MCQ (select 1)**
You must tell the sponsor that a key feature will be three weeks late. What is the best way?
A. A brief note at the bottom of the weekly report
B. A direct call or meeting, with a written follow-up covering impact, options, and your recommendation
C. Wait until she asks
D. Ask the team to tell her

**Correct answer: B.**
**Why:** Significant or sensitive news is best delivered live so she can ask questions, with a written record afterward.
**Why others are wrong:** A buries bad news. C and D avoid ownership.
**Takeaway:** Use live conversation for sensitive news and writing for decisions and records.

---

## Teams and Leadership (Q125 to Q127)

**Q125 | Feedback (SBI) | Intermediate | MCQ (select 1)**
Which statement best follows the Situation-Behavior-Impact structure?
A. "You're careless with the client."
B. "In Tuesday's client demo, you changed the layout without telling Priya, so the client saw two versions and asked which was final. What happened?"
C. "Everyone thinks you're unreliable."
D. "Please try to do better."

**Correct answer: B.**
**Why:** It names the situation, the specific behavior, and the impact, then asks for their view. **Why others are wrong:** A and C judge the person without specifics, and D gives no guidance.
**Takeaway:** Describe what happened, not who they are.

---

**Q126 | Conflict resolution | Intermediate | Matching [Supplemental]**
Match each situation to the best conflict-handling approach.
1. A production outage needs an immediate decision, with no time for discussion.
2. Two members each need part of a shared resource and time is short.
3. An important design disagreement, with time available, where both sets of needs matter.
4. Tempers are high over a minor issue and need to cool down.
a. Collaborate
b. Compromise
c. Force (compete)
d. Withdraw (temporarily)

**Correct answer: 1-c, 2-b, 3-a, 4-d.**
**Why:** Match the approach to urgency and importance. Force suits emergencies, compromise suits short time and moderate stakes, collaboration suits important issues with time, and withdrawing suits cooling off.
**Takeaway:** No single approach fits every conflict.

---

**Q127 | Decision-making | Advanced | Scenario (select 1)**
You must choose a hosting provider by Friday but don't know how much traffic to expect. What is the best approach?
A. Postpone the decision until traffic is known.
B. Choose a provider with flexible, scalable plans (a reversible choice), record your assumptions, and set a review date.
C. Choose the most expensive option.
D. Let the team vote and avoid ownership.

**Correct answer: B.**
**Reasoning:** With incomplete information, prefer reversible decisions, state assumptions, and revisit when facts arrive.
**Why others are wrong:** A blocks the project. C is not tied to evidence. D avoids accountability.
**Takeaway:** Decide, document, and review.

---

## Quality (Q128 to Q130)

**Q128 | Root-cause analysis | Advanced | MCQ (select 1)**
Problem: reminder emails were sent at the wrong time. 5 Whys: (1) The system used server time, not the customer's time zone. (2) Time zone wasn't in the requirements. (3) Requirements were gathered through interviews only. (4) The requirements checklist had no item for "time and locale." Which finding is the root cause best addressed by a **preventive action**?
A. The developer made a mistake.
B. The requirements checklist had no item for time and locale.
C. The emails were sent.
D. The customers were in different time zones.

**Correct answer: B.**
**Why:** It is a process gap. Adding the item to the checklist prevents similar defects in future work. **Why others are wrong:** A blames a person, C restates the problem, and D is a fact, not a cause you can fix.
**Takeaway:** Stop at a cause you can change.

---

**Q129 | Quality (defect density) | Intermediate | Numerical (select 1)**
Module X has 15 defects across 5 features. Module Y has 12 defects across 3 features. Which module has the higher defect density, and what is it?
A. X, at 3 defects per feature
B. Y, at 4 defects per feature
C. X, at 15 defects per feature
D. Both are equal

**Correct answer: B.**
**Calculation:** X = 15 ÷ 5 = **3**. Y = 12 ÷ 3 = **4**.
**Why others are wrong:** A has the right figure for X but the wrong comparison. C divides incorrectly.
**Takeaway:** Raw counts mislead, so compare defects relative to size.

---

**Q130 | QA vs. QC | Intermediate | Matching**
Classify each activity as quality assurance (QA) or quality control (QC).
1. An audit of whether code reviews are being carried out as the process requires
2. Running user acceptance testing
3. Training the team on coding standards
4. Measuring page load time against the target
a. Quality assurance (process)
b. Quality control (product)

**Correct answer: 1-a, 2-b, 3-a, 4-b.**
**Why:** QA targets the process, and QC examines the product. **Takeaway:** In many software teams "QA" means testing, which is QC in project management terms.

---

## Change Management (Q131 to Q132)

**Q131 | Change control | Intermediate | MCQ (select 1)**
A change was approved, but the developer built the old version because nobody told her. Which change-control step failed, and what is the best fix?
A. Assessment; stop approving changes.
B. Communication and baseline update; fix the work, add "notify everyone affected and update documents" to the process, and use version control.
C. Approval; require two approvers.
D. Logging; the developer should have asked.

**Correct answer: B.**
**Why:** Approval was fine. The decision wasn't shared or reflected in the working documents. **Why others are wrong:** A, C, and D address steps that worked.
**Takeaway:** A decision isn't done until the people doing the work know about it.

---

**Q132 | Change management (ADKAR) | Intermediate | Scenario (select 1)**
Staff were trained, wanted the new tool, and used it for a month. Two months later they are going back to the old spreadsheet. Which ADKAR element is weakest?
A. Awareness
B. Desire
C. Knowledge
D. Reinforcement

**Correct answer: D.**
**Why:** Reinforcement keeps new behavior in place through check-ins, recognition, and removing the old option. **Takeaway:** Plan follow-up after launch, not only before it.

---

## Agile, Scrum, and Kanban (Q133 to Q139)

**Q133 | Sprint Planning | Intermediate | Multiple-select (select 3)**
According to the Scrum Guide, Sprint Planning addresses which three topics?
A. Why this Sprint is valuable (the Sprint Goal)
B. What can be done this Sprint
C. How the chosen work will get done
D. Who will be blamed if the goal is missed
E. The annual budget for the company

**Correct answer: A, B, C.**
**Why others are wrong:** D and E are not Sprint Planning topics.
**Takeaway:** Why, what, and how.

---

**Q134 | Agile Metrics (forecast) | Intermediate | Numerical (select 1)**
A team completed 12, 15, 18, and 15 points in four sprints. 95 points remain. Using the average of all four sprints, how many sprints are needed?
A. 5
B. 6
C. 7
D. 8

**Correct answer: C.**
**Calculation:** Average = (12 + 15 + 18 + 15) ÷ 4 = 60 ÷ 4 = **15**. 95 ÷ 15 = 6.33, so round **up** to **7**.
**Why others are wrong:** B rounds down and would leave work unfinished.
**Takeaway:** Forecasts are ranges, so refresh them every sprint.

---

**Q135 | Agile Metrics (burndown) | Intermediate | Numerical (select 1)**
A 10-day sprint starts with 40 points. After day 5, 26 points remain. How does this compare with the ideal burndown?
A. 6 points behind
B. 6 points ahead
C. 4 points behind
D. Exactly on track

**Correct answer: A.**
**Calculation:** Ideal = 4 points per day, so 20 remain after day 5. Actual = 26. 26 − 20 = **6 points behind**.
**Why others are wrong:** B has the direction reversed. C and D have the wrong arithmetic.
**Takeaway:** Behind pace is a prompt for the team to talk to the PO about scope, not to push harder. Remember that points burn down only when items are Done.

---

**Q136 | Agile Project Management | Advanced | Scenario (select 1)**
The Product Owner has been unavailable for two sprints. Questions about priority go unanswered, and the team is guessing. What is the best action?
A. Let the team keep guessing.
B. Treat it as an impediment: raise it, have the Scrum Master or PM escalate to the sponsor, and agree how the PO role will be filled.
C. Let the PM quietly take over backlog decisions.
D. Cancel the project.

**Correct answer: B.**
**Reasoning:** The PO is accountable for backlog value and order. If that role is unfilled, the organization must fix it.
**Why others are wrong:** A wastes effort on guesses. C bypasses accountability. D is disproportionate.
**Takeaway:** Raise role gaps as impediments.

---

**Q137 | Backlogs (story splitting) | Advanced | MCQ (select 1)**
A 13-point story, "Customer pays a deposit," is too big for one sprint. Which split is best?
A. Front-end work first, back-end work second
B. Thin slices that each deliver user value: pay by card using a mock provider; connect the live provider; add refunds
C. Split into the 13 individual tasks
D. Leave it as it is

**Correct answer: B.**
**Why:** Vertical slices deliver something usable and testable each time. **Why others are wrong:** A splits by technical layer, so nothing is usable until both halves are finished. C splits into tasks, not value. D keeps it too large.
**Takeaway:** Split by user value, not by technical layer.

---

**Q138 | Backlogs (estimating) | Intermediate | MCQ (select 1)**
In planning poker, the team's estimates are 3, 3, 5, and 13. What should happen next?
A. Take the average.
B. Have the people with the highest and lowest estimates explain their reasoning, then re-vote.
C. Use the highest estimate.
D. Ignore the 13.

**Correct answer: B.**
**Why:** The gap usually reveals different assumptions or hidden work. Discussing it improves shared understanding.
**Why others are wrong:** A, C, and D discard that information.
**Takeaway:** The conversation matters more than the number. Story points are a common practice, not a Scrum requirement.

---

**Q139 | Agile (Kanban vs. Scrum) | Beginner | True/False**
"Kanban requires work to be organized in fixed-length sprints."

**Correct answer: False.**
**Why:** Kanban is continuous flow with WIP limits. Fixed-length sprints belong to Scrum.
**Takeaway:** Scrumban blends them, but know which rule belongs where.

---

## Closure (Q140)

**Q140 | Project Closure (handover) | Advanced | Scenario (select 1)**
You sent the operations team all the documentation. When you ask them to restore the system from a backup, they cannot do it. What is the best action?
A. Close the project, because the documents were delivered.
B. Hold a hands-on walkthrough and let them practice the restore, then get their confirmation before closing the handover.
C. Do it yourself every time it is needed.
D. Tell the operations team to read the documents again.

**Correct answer: B.**
**Reasoning:** A handover is complete when the receiver can operate what they've received, not when the documents are sent.
**Why others are wrong:** A confuses delivery with understanding. C leaves a dependency on the project team. D repeats what failed.
**Takeaway:** Confirm capability, not only delivery.

---

## Part 8C Score Sheet

Give yourself 1 point per correct answer. For multiple-select and matching, count the question correct only if every part is right. For short-answer questions, count it correct if your answer covers the main points of the model answer.

| Topic | Questions | Your score |
|---|---|---|
| Foundations, initiation, scoping | Q101 to Q106 (6) | ___ |
| Planning and schedule | Q107 to Q111 (5) | ___ |
| Budget and earned value | Q112 to Q117 (6) | ___ |
| Risk | Q118 to Q120 (3) | ___ |
| Stakeholders and communication | Q121 to Q124 (4) | ___ |
| Teams and leadership | Q125 to Q127 (3) | ___ |
| Quality | Q128 to Q130 (3) | ___ |
| Change | Q131 to Q132 (2) | ___ |
| Agile, Scrum, Kanban | Q133 to Q139 (7) | ___ |
| Closure | Q140 (1) | ___ |
| **Total** | **40** | ___ |

**Reading your result:** this isn't an official pass mark. Review any topic where you missed more than a third of the questions.

**Running total:** Q1 to Q140 are now done (Part 1: 20, 8A: 40, 8B: 40, 8C: 40).

## Part 8C Checkpoint

Without looking back:
1. In Q108, how do you find the slack of the task that is *not* on the critical path?
2. A team of 12 people: how many communication channels exist?
3. Why is a "13" estimate in planning poker valuable even when the other estimates are 3?

---
# Part 8D: Practice Question Bank (Q141 to Q180)

**Note:** These are original practice questions, not official Google assessment content. The 10-field format is the same as in 8A to 8C.

**Change to my earlier plan:** Part 9 hasn't taught web presence and interviewing yet. So that Q175 to Q180 are fair, here is a short primer. Part 9 covers both in depth, and this primer is **[Supplemental]**, not official Google content.

**Primer: Skills 19 and 20 in brief**
- **LinkedIn headline:** say what you do and the value you deliver, with keywords, not just a job title or "aspiring" labels.
- **Achievements:** write action + scope + measurable result (for example, "Led a 4-person team to launch a booking app on schedule, cutting phone bookings by 40%"). Only use numbers that are true.
- **Confidentiality:** don't reveal client names, internal figures, or proprietary details without permission. Generalize ("a regional retail client") or use percentages and ranges the employer has cleared.
- **STAR method:** **S**ituation (context), **T**ask (your responsibility), **A**ction (what *you* did), **R**esult (the outcome, with numbers if possible, and what you learned).
- **Credentials:** state exactly what you hold. The Google certificate is not a PMP, and neither guarantees a job.

---

## Foundations, Initiation, and Scoping (Q141 to Q144)

**Q141 | Foundations | Beginner | MCQ (select 1)**
Which is **not** a characteristic of a project?
A. It is temporary.
B. It produces a unique product, service, or result.
C. It continues indefinitely as a routine activity.
D. It has a defined start and end.

**Correct answer: C.**
**Why correct:** Indefinite, repeating work is operations.
**Why others are wrong:** A, B, and D define a project.
**Concept:** Project vs. operations. **Takeaway:** If the work has no end and repeats, don't run it as a project.

---

**Q142 | Initiation (goal alignment) | Intermediate | Scenario (select 1)**
At kickoff, the sponsor wants to cut costs, while the department head wants new features. Both are in your stakeholder register. What is the best action before the charter is signed?
A. Write the charter using the sponsor's goals only.
B. Facilitate a short alignment session, document measurable goals and priorities, and have the sponsor decide where they conflict.
C. Wait until they agree by themselves.
D. Start the project and handle it later.

**Correct answer: B.**
**Reasoning:** Conflicting goals become scope disputes later. A facilitated session surfaces interests, and the sponsor has the authority to decide.
**Why others are wrong:** A ignores a key stakeholder. C stalls. D carries the conflict into execution.
**Takeaway:** Resolve goal conflicts before signing the charter.

---

**Q143 | SMART goals (practical) | Intermediate | Short answer**
Rewrite "Improve website speed" as a SMART goal.

**Model answer:** "Reduce average home-page load time from 4 seconds to under 2 seconds for 95% of visits within 8 weeks of project start." Any version with a specific target, a baseline, a measure, and a deadline is acceptable.
**Why it works:** It is testable and time-bound. Whether it is *achievable* depends on the team's capability, which you would confirm before committing.
**Takeaway:** If nobody can say whether you met the goal, it isn't SMART yet.

---

**Q144 | Stakeholder register | Intermediate | True/False**
"A stakeholder register should avoid recording attitudes such as 'resistant,' so nobody is offended."

**Correct answer: False.**
**Why:** Attitudes drive engagement strategy. The better practice is to record them factually and restrict who can see the register, not to leave them out.
**Takeaway:** Keep the register professional and access-controlled.

---

## Planning and Schedule (Q145 to Q148)

**Q145 | Estimating | Beginner | MCQ (select 1)**
The team estimates each work package separately and adds them to get the project estimate. This is:
A. Analogous estimating
B. Bottom-up estimating
C. Parametric estimating
D. Expert judgment only

**Correct answer: B.**
**Why:** Bottom-up builds the total from detailed parts. **Why others are wrong:** A uses a past project. C uses unit rates. D relies on opinion without the build-up.
**Takeaway:** Bottom-up is slower but usually more accurate.

---

**Q146 | Critical Path | Advanced | Numerical (select 1)**
A (3 days) is first. B (4 days) and C (6 days) follow A. D (2 days) follows both B and C. E (3 days) follows C. F (1 day) follows both D and E. What is the project duration and the slack on D?
A. 12 days; slack 0
B. 13 days; slack 1
C. 13 days; slack 3
D. 16 days; slack 1

**Correct answer: B.**
**Calculation:** A-B-D-F = 3+4+2+1 = 10. A-C-D-F = 3+6+2+1 = 12. A-C-E-F = 3+6+3+1 = **13** (critical). D's longest path is 12, so slack = 13 − 12 = **1**.
**Why others are wrong:** A misses the longest path. C gives B's slack (13 − 10 = 3). D adds the durations of the parallel tasks.
**Takeaway:** Slack depends on the longest path *through that task*.

---

**Q147 | Milestones | Beginner | Multiple-select (select 2)**
Which two are milestones?
A. Design approved by the sponsor
B. Write the payment code
C. Go-live
D. Test the login page

**Correct answer: A and C.**
**Why:** Milestones mark points in time or decisions and have no duration. **Why others are wrong:** B and D are tasks with effort and duration.
**Takeaway:** Use milestones as stakeholder checkpoints.

---

**Q148 | Estimating (three-point vs. PERT) | Intermediate | Numerical (select 1)**
A task has O = 4, M = 7, P = 16 days. What are the simple three-point average and the PERT estimate?
A. 9 days and 8 days
B. 8 days and 9 days
C. 7 days and 9 days
D. 9 days and 9 days

**Correct answer: A.**
**Calculation:** Simple average = (4 + 7 + 16) ÷ 3 = 27 ÷ 3 = **9**. PERT = (4 + 4×7 + 16) ÷ 6 = 48 ÷ 6 = **8**.
**Why others are wrong:** B swaps them. C and D use wrong inputs.
**Takeaway:** PERT weights the most likely value more heavily, so read which formula is requested.

---

## Budget and Earned Value (Q149 to Q153)

**Q149 | Earned Value (SV, SPI) | Intermediate | Numerical (select 1)**
PV = $60,000, EV = $54,000, AC = $58,000. What are SV and SPI?
A. SV −$6,000; SPI 0.90
B. SV +$6,000; SPI 1.11
C. SV −$4,000; SPI 0.93
D. SV −$6,000; SPI 1.11

**Correct answer: A.**
**Calculation:** SV = EV − PV = 54,000 − 60,000 = **−6,000**. SPI = EV ÷ PV = 54,000 ÷ 60,000 = **0.90**.
**Why others are wrong:** B and D invert a sign or ratio. C is the cost variance and CPI.
**Plain English:** The project has done 90% of the planned work, so it is behind schedule.
**Takeaway:** Pair SPI with the critical path before acting.

---

**Q150 | Earned Value (EAC, ETC, one-off) | Advanced | Numerical (select 1)**
BAC = $90,000, EV = $30,000, AC = $36,000. The overrun came from a one-off problem, and the remaining work will run to plan. What are EAC and ETC?
A. EAC $96,000; ETC $60,000
B. EAC $108,000; ETC $72,000
C. EAC $90,000; ETC $54,000
D. EAC $96,000; ETC $96,000

**Correct answer: A.**
**Calculation:** EAC = AC + (BAC − EV) = 36,000 + 60,000 = **96,000**. ETC = EAC − AC = **60,000**.
**Why others are wrong:** B uses BAC ÷ CPI (CPI = 0.83), which assumes poor performance continues. C ignores the overrun. D forgets to subtract AC.
**Takeaway:** "One-off" means the AC + (BAC − EV) formula.

---

**Q151 | Earned Value (from % complete) | Intermediate | Numerical (select 1)**
BAC = $80,000, the project is 45% complete, and AC = $40,000. What are CV and CPI?
A. CV +$4,000; CPI 1.11
B. CV −$4,000; CPI 0.90
C. CV −$4,000; CPI 1.11
D. CV −$40,000; CPI 0.45

**Correct answer: B.**
**Calculation:** EV = 0.45 × 80,000 = **36,000**. CV = 36,000 − 40,000 = **−4,000**. CPI = 36,000 ÷ 40,000 = **0.90**.
**Why others are wrong:** A and C invert the sign or ratio. D uses wrong inputs.
**Takeaway:** Convert percent complete to EV first.

---

**Q152 | Earned Value (interpretation) | Intermediate | Matching**
Match each pair of indices to its meaning.
1. CPI 1.2, SPI 0.8
2. CPI 0.8, SPI 1.2
3. CPI 0.8, SPI 0.8
4. CPI 1.1, SPI 1.1
a. Over budget, ahead of schedule
b. Under budget, behind schedule
c. Over budget and behind schedule
d. Under budget and ahead of schedule

**Correct answer: 1-b, 2-a, 3-c, 4-d.**
**Why:** CPI above 1 means cost-efficient. SPI above 1 means ahead of plan.
**Takeaway:** Each index tells a different story, so read them separately.

---

**Q153 | Cost tracking | Intermediate | Scenario (select 1)**
Halfway through the schedule, 50% of the budget is spent, but only 30% of the work is complete. Which interpretation is best?
A. On track, since half the money is spent at the halfway point.
B. CPI is about 0.60 (30% ÷ 50%), a serious cost problem. Investigate causes, re-forecast, and take the options to the sponsor.
C. Under budget, since less work is done.
D. Ahead of schedule.

**Correct answer: B.**
**Reasoning:** Money spent isn't progress. EV (30%) divided by AC (50%) = 0.60, so each dollar earns 60 cents of planned value.
**Why others are wrong:** A confuses spending with progress. C and D read the numbers backwards.
**Takeaway:** Always compare spending with *work completed*.

---

## Risk (Q154 to Q156)

**Q154 | Risk identification | Beginner | Multiple-select (select 3)**
Which three are good ways to identify risks?
A. Brainstorming with the team
B. Reviewing lessons learned from past projects
C. Interviewing stakeholders and experts
D. Flipping a coin
E. Ignoring assumptions

**Correct answer: A, B, C.**
**Why others are wrong:** D has no basis, and E overlooks a major source of risk, since unverified assumptions can turn into risks.
**Takeaway:** Use several sources, and revisit identification regularly.

---

**Q155 | Risk (EMV decision) | Advanced | Numerical (select 1)**
A risk has a 25% chance of causing a $12,000 loss. A vendor offers a $2,000 service that would remove it completely. What does EMV suggest?
A. Buy the service. The expected loss is $3,000, which is more than the $2,000 cost.
B. Don't buy it. The expected loss is $1,500.
C. Don't buy it. $2,000 is more than 25%.
D. EMV cannot be used here.

**Correct answer: A.**
**Calculation:** EMV of loss = 0.25 × 12,000 = **$3,000**. The service costs $2,000, so the expected saving is about $1,000.
**Why others are wrong:** B has wrong arithmetic. C misreads the logic. D is wrong because EMV supports this comparison.
**Takeaway:** EMV is one input. Risk tolerance and non-financial impact also matter.

---

**Q156 | Risk statements | Intermediate | MCQ (select 1)**
Which is the best-written risk statement?
A. "Vendor problems."
B. "Because the vendor hasn't confirmed delivery dates, the payment API may arrive after week 4, delaying integration by up to two weeks."
C. "The vendor is unreliable."
D. "We might fail."

**Correct answer: B.**
**Why:** It gives a cause, an uncertain event, and an impact, so it can be scored and managed. **Why others are wrong:** A, C, and D are vague or judgments.
**Takeaway:** Use cause, event, impact.

---

## Stakeholders and Communication (Q157 to Q159)

**Q157 | Communication plan (practical) | Intermediate | Short answer**
List five columns a communication plan table normally includes.

**Model answer:** Audience, information to share, frequency, channel, and owner (sender). Purpose or feedback method are also common.
**Why:** Each column answers who, what, when, how, and by whom.
**Takeaway:** If a message has no owner, it usually doesn't get sent.

---

**Q158 | Meetings | Intermediate | MCQ (select 1)**
Weekly meetings run long and end without decisions. What is the best fix?
A. Hold the meeting more often.
B. Set a purpose and agenda in advance, timebox items, name a decision owner for each, and send notes with actions, owners, and dates.
C. Cancel all meetings.
D. Invite more people.

**Correct answer: B.**
**Why:** Structure turns discussion into decisions and records them. **Why others are wrong:** A and D add cost, and C removes useful coordination.
**Takeaway:** Ask whether the meeting could be an email, and if not, make it decision-focused.

---

**Q159 | Communication channels | Intermediate | Numerical (select 1)**
Channels = n(n − 1) ÷ 2. A team grows from 6 to 9 people **[Supplemental]**. How many channels exist at 9, and how many were added?
A. 36 channels; 21 added
B. 36 channels; 3 added
C. 72 channels; 57 added
D. 15 channels; 21 added

**Correct answer: A.**
**Calculation:** 6 people: 6 × 5 ÷ 2 = **15**. 9 people: 9 × 8 ÷ 2 = **36**. Added = **21**.
**Why others are wrong:** B counts added people. C forgets to divide by 2. D gives the old total.
**Takeaway:** Communication complexity grows faster than team size.

---

## Teams and Leadership (Q160 to Q162)

**Q160 | Delegation | Intermediate | Scenario (select 1)**
You delegated a task, but you check on the developer every hour. She is frustrated. What is the best fix?
A. Keep checking, since you stay accountable.
B. Agree on the outcome, success criteria, and checkpoints (for example, a demo on Wednesday), then step back and offer help when asked.
C. Take the task back.
D. Say nothing.

**Correct answer: B.**
**Reasoning:** You remain accountable, but ownership requires room to work. Checkpoints give visibility without micromanagement.
**Why others are wrong:** A undermines trust. C removes ownership. D leaves the problem unresolved.
**Takeaway:** Delegate outcomes with checkpoints.

---

**Q161 | Team development | Intermediate | Matching [Supplemental]**
Match each team behavior to its Tuckman stage.
1. Members are polite and unsure of roles.
2. Members disagree about methods and priorities.
3. Members have agreed working rules and cooperate.
4. Members work efficiently and solve problems on their own.
a. Performing
b. Forming
c. Norming
d. Storming

**Correct answer: 1-b, 2-d, 3-c, 4-a.**
**Takeaway:** Adjust your leadership. Give direction in forming and facilitation in storming, then delegate more in performing.

---

**Q162 | Difficult stakeholders | Advanced | Scenario (select 1)**
A senior stakeholder criticizes the project sharply in a team meeting. What is the best response?
A. Argue back with facts.
B. Stay calm, acknowledge the concern, say you'll look into it, and arrange a private conversation to understand the underlying issue.
C. Ignore the comment.
D. Report them to HR.

**Correct answer: B.**
**Reasoning:** De-escalate in public and resolve in private. The criticism may reveal a real problem or an unmet expectation.
**Why others are wrong:** A escalates. C leaves the concern unresolved. D is for behavior or policy breaches.
**Takeaway:** Listen for the interest behind the complaint.

---

## Quality (Q163 to Q165)

**Q163 | Pareto analysis | Intermediate | Numerical (select 1)**
A defect log shows categories with 40, 25, 15, 12, and 8 defects (100 total). How many of the largest categories are needed to account for at least 80% of defects?
A. 2
B. 3
C. 4
D. 5

**Correct answer: B.**
**Calculation:** Cumulative: 40%, 65%, **80%**. Three categories reach 80%.
**Why others are wrong:** Two categories reach only 65%.
**Takeaway:** Fix the vital few first.

---

**Q164 | Quality management plan | Intermediate | Multiple-select (select 3)**
Which three normally belong in a quality management plan?
A. Quality objectives and standards
B. Quality metrics
C. Roles and responsibilities for quality activities
D. Each team member's salary
E. The vendor's marketing plan

**Correct answer: A, B, C.**
**Why others are wrong:** D and E are unrelated to managing quality.
**Takeaway:** A quality plan states what "good" means, how you'll check it, and who does it.

---

**Q165 | Quality assessment (UAT) | Beginner | MCQ (select 1)**
Who should perform user acceptance testing (UAT)?
A. Only the developers who wrote the code
B. Representative end users or customer staff
C. Only the project manager
D. No one

**Correct answer: B.**
**Why:** UAT checks that the product meets real user needs. **Why others are wrong:** A tests its own work, C is not the user, and D skips validation.
**Takeaway:** Developers test whether it was built right, and users confirm it's the right thing.

---

## Change Management (Q166 to Q167)

**Q166 | Change control (impact) | Advanced | Numerical (select 1)**
A change adds 5 days to a critical-path task. The project has a 3-day schedule buffer. What is the likely net delay if the buffer is used, and what should you do?
A. 0 days; do nothing.
B. 2 days; present the impact and options (accept the 2-day slip, trade scope, or add resources) for a decision.
C. 5 days; ignore the buffer.
D. 8 days.

**Correct answer: B.**
**Calculation:** 5 − 3 = **2 days** of net delay.
**Why others are wrong:** A ignores the 2-day overrun. C ignores the buffer. D adds instead of subtracts.
**Takeaway:** Show the approver the delay after buffer, plus options.

---

**Q167 | Change control | Intermediate | Scenario (select 1)**
A stakeholder asks a developer directly to add a feature. The developer agrees. What should happen?
A. Nothing, since the developer agreed.
B. The developer politely says it will be logged as a change request. The PM assesses the impact and the approver decides.
C. The PM takes the feature out of the product immediately.
D. The developer works on it at night and doesn't tell anyone.

**Correct answer: B.**
**Why:** All changes go through one process, so impact is visible and decisions are recorded. **Why others are wrong:** A and D skip control, and C acts without assessment.
**Takeaway:** Agree a polite phrase the team can use: "Let's log that and check the impact."

---

## Agile, Scrum, and Backlogs (Q168 to Q172)

**Q168 | Scrum roles | Intermediate | True/False**
"In Scrum, 'Developers' means only people who write code."

**Correct answer: False.**
**Why:** In the 2020 Scrum Guide, Developers are the people who do the work of creating the Increment, which may include testers, designers, and others.
**Takeaway:** Watch for older wording ("development team") in exams.

---

**Q169 | Scrum events | Intermediate | MCQ (select 1)**
For a one-month Sprint, what is the maximum length of the Sprint Retrospective?
A. 1 hour
B. 3 hours
C. 4 hours
D. 8 hours

**Correct answer: B.**
**Why:** The Scrum Guide sets 3 hours for a one-month Sprint (4 hours for Review, 8 hours for Planning). Shorter Sprints normally have shorter events.
**Takeaway:** These are *maximums*, not required durations.

---

**Q170 | Agile Metrics (velocity) | Intermediate | Scenario (select 1)**
A team's last three velocities were 20, 22, and 18. A manager wants them to commit to 30 points next sprint. What is the best response?
A. Agree.
B. Explain that their recent average is about 20, plan around that range, and discuss what would have to change (scope, capacity, or impediments) to deliver more.
C. Commit to 30 and work overtime.
D. Double the story points.

**Correct answer: B.**
**Reasoning:** Velocity is a forecasting tool. The average is (20 + 22 + 18) ÷ 3 = **20**. Pushing the team beyond its capacity leads to unfinished work and quality problems.
**Why others are wrong:** A and C ignore the evidence. D inflates the numbers without changing the work.
**Takeaway:** Use velocity for planning, not pressure.

---

**Q171 | Agile Metrics (burndown) | Intermediate | Numerical (select 1)**
A 10-day sprint starts with 30 points. After day 4, 20 points remain. How does this compare with the ideal burndown?
A. 2 points behind
B. 2 points ahead
C. 10 points behind
D. Exactly on track

**Correct answer: A.**
**Calculation:** Ideal = 3 points per day, so 18 remain after day 4. Actual = 20. 20 − 18 = **2 points behind**.
**Why others are wrong:** B reverses the direction. C is the work done, not the gap. D ignores the difference.
**Takeaway:** Small gaps early are a prompt to talk, not to panic.

---

**Q172 | Backlogs (WSJF) | Advanced | Numerical (select 1)** **[Supplemental]**
Using WSJF = (business value + time criticality + risk reduction) ÷ job size, which item should be done first?
- Item A: value 8, time criticality 5, risk reduction 3, size 4
- Item B: value 6, time criticality 3, risk reduction 3, size 2
- Item C: value 10, time criticality 8, risk reduction 2, size 8

A. A
B. B
C. C
D. A and B tie

**Correct answer: B.**
**Calculation:** A = 16 ÷ 4 = **4.0**. B = 12 ÷ 2 = **6.0**. C = 20 ÷ 8 = **2.5**.
**Why others are wrong:** C has the highest raw score but the lowest ratio because of its size. A and B don't tie.
**Takeaway:** Small, valuable, time-critical items often come first. WSJF is one method, and the Product Owner makes the final call.

---

## Closure (Q173 to Q174)

**Q173 | Lessons learned | Intermediate | MCQ (select 1)**
When should lessons learned be collected?
A. Only after the project closes
B. Throughout the project (for example, after phases and in retrospectives), with a final session at closure
C. Only when the project fails
D. Never, since the team is busy

**Correct answer: B.**
**Why:** Early capture is more accurate and lets the current project benefit. **Why others are wrong:** A loses detail, C misses successes worth repeating, and D wastes the organization's biggest learning source.
**Takeaway:** Record lessons as you go, then review them at the end.

---

**Q174 | Procurement closure | Intermediate | Scenario (select 1)**
At closure, a hosting contract is still active in the project's name. What should you do?
A. Leave it and close the project.
B. Close it or transfer it to the operations owner, confirm final payments, record warranty and renewal terms, and document the handover.
C. Cancel it without telling operations.
D. Ask the vendor to bill the project forever.

**Correct answer: B.**
**Reasoning:** Open commitments with no owner create costs and risk after the team has gone.
**Why others are wrong:** A leaves it unowned. C could break the live service. D keeps charging a closed project.
**Takeaway:** Every contract ends or gets a new owner.

---

## Web Presence and Interviewing (Q175 to Q180)

**Q175 | Web Presence (LinkedIn) | Beginner | MCQ (select 1)**
Which LinkedIn headline best presents a software developer moving into project management?
A. "Unemployed and looking"
B. "Software Developer → Project Manager | Agile delivery, stakeholder communication, risk management | Google PM Certificate"
C. "Developer"
D. "Hard worker and team player"

**Correct answer: B.**
**Why:** It states the direction, relevant skills, and a factual credential. **Why others are wrong:** A is negative, C is generic, and D is a cliché with no keywords.
**Takeaway:** Show the value you offer, using the words recruiters search for.

---

**Q176 | Web Presence (confidentiality) | Intermediate | MCQ (select 1)**
You want to show results from a confidential client project in your portfolio. What is best?
A. Post the full client documents.
B. Describe the project generally ("a regional retail client") and use outcomes your employer has cleared, such as "reduced booking time by 30%," without internal documents or sensitive data.
C. Leave projects out altogether.
D. Make up impressive numbers.

**Correct answer: B.**
**Why:** It shows your achievements while protecting the client. **Why others are wrong:** A breaches confidentiality, C hides your experience, and D is dishonest.
**Takeaway:** If unsure, ask your employer or client what you can share.

---

**Q177 | Interviewing (STAR) | Beginner | Matching**
Match each STAR part to what it covers.
1. Situation
2. Task
3. Action
4. Result
a. What *you* did, step by step
b. The outcome, with numbers or what you learned
c. The context and background
d. Your responsibility or goal in that situation

**Correct answer: 1-c, 2-d, 3-a, 4-b.**
**Takeaway:** Spend most of the answer on Action and Result, and say "I," not only "we."

---

**Q178 | Interviewing (behavioral) | Intermediate | MCQ (select 1)**
An interviewer asks, "Tell me about a conflict on a team." Which answer is strongest?
A. "I've never had a conflict."
B. "Two engineers disagreed about the design. I met each separately, then led a session to agree the decision criteria. The tech lead chose, we kept the schedule, and the relationship recovered."
C. "My teammate was lazy, so I reported him."
D. "We just ignored it."

**Correct answer: B.**
**Why:** It shows the situation, your actions, and a result, with respect for both people. **Why others are wrong:** A is implausible, C blames, and D shows avoidance.
**Takeaway:** Choose real stories that show your process, and avoid blaming.

---

**Q179 | Resume writing (practical) | Intermediate | Short answer**
Rewrite the weak resume line "Worked on a booking app" as a stronger achievement bullet. Use clearly marked **example** numbers.

**Model answer (example numbers):** "Coordinated a 4-person team to deliver a customer booking app on schedule, using weekly risk reviews and a change log; online bookings reached 55% of total within two months (example figures)." A strong bullet has an action, scope, method, and a measurable result.
**Important:** On a real resume, use only true numbers.
**Takeaway:** Translate technical work into delivery, risk, stakeholder, and outcome language.

---

**Q180 | Career (credentials) | Intermediate | Scenario (select 1)**
You have completed the Google Project Management Certificate. How should you list it on your resume?
A. "PMP-certified Project Manager"
B. "Google Project Management Professional Certificate (Coursera), completed [month, year]"
C. "Certified by Google as a guaranteed project manager"
D. Leave it off, since it isn't a PMP.

**Correct answer: B.**
**Why:** It is accurate and verifiable. **Why others are wrong:** A is false, and a false credential can end a job offer. C overstates what a certificate guarantees. D hides genuine learning.
**Takeaway:** State exactly what you hold. A certificate may help, but it doesn't automatically qualify you for the PMP or guarantee a job.

---

## Part 8D Score Sheet

Give yourself 1 point per correct answer. For multiple-select and matching, count the question correct only if every part is right. For short-answer questions, count it correct if your answer covers the main points of the model answer.

| Topic | Questions | Your score |
|---|---|---|
| Foundations, initiation, scoping | Q141 to Q144 (4) | ___ |
| Planning and schedule | Q145 to Q148 (4) | ___ |
| Budget and earned value | Q149 to Q153 (5) | ___ |
| Risk | Q154 to Q156 (3) | ___ |
| Stakeholders and communication | Q157 to Q159 (3) | ___ |
| Teams and leadership | Q160 to Q162 (3) | ___ |
| Quality | Q163 to Q165 (3) | ___ |
| Change | Q166 to Q167 (2) | ___ |
| Agile and backlogs | Q168 to Q172 (5) | ___ |
| Closure | Q173 to Q174 (2) | ___ |
| Web presence and interviewing | Q175 to Q180 (6) | ___ |
| **Total** | **40** | ___ |

**Reading your result:** this isn't an official pass mark. Review any topic where you missed more than a third of the questions.

**Running total:** Q1 to Q180 are now done (Part 1: 20, 8A to 8D: 40 each).

## Part 8D Checkpoint

Without looking back:
1. In Q146, why is D's slack 1 and not 3?
2. When do you use AC + (BAC − EV) for EAC, and when BAC ÷ CPI?
3. What are the four parts of STAR, and which two deserve the most time in your answer?

---
# Part 8E: Practice Question Bank (Q181 to Q220)

**Note:** These are original practice questions, not official Google assessment content. They use the same 10-field format as 8A to 8D. This installment is weighted toward advanced scenarios, mixed numerical problems, and Agile, quality, and change cases. With Q220, the question bank passes the 200-question requirement.

---

## Foundations, Initiation, and Scoping (Q181 to Q185)

**Q181 | Foundations (triple constraint) | Advanced | Scenario (select 1)**
The sponsor insists on a fixed date (12 weeks), a fixed budget ($30,000), and the full scope. Your bottom-up plan shows 14 weeks and $38,000. What is the best response?
A. Agree and tell the team to work harder.
B. Show the gap with evidence, then offer options (cut or phase scope, extend the date, or add budget or resources, each with its risk) and ask the sponsor to choose.
C. Quietly cut quality to fit.
D. Refuse to start.

**Correct answer: B.**
**Reasoning:** Scope, schedule, and cost are linked, so all three cannot be fixed when the estimate does not fit. The sponsor owns the trade-off, and you owe the sponsor the facts and the choices.
**Why others are wrong:** A hides the problem. C hides a quality trade-off. D abandons the sponsor.
**Concept:** Triple constraint. **Takeaway:** Make trade-offs visible early, with numbers.

---

**Q182 | Initiation (assumptions) | Intermediate | MCQ (select 1)**
The charter assumes "the client will supply product data by week 2." What is the best action?
A. Leave it, since the client agreed in a meeting.
B. Record it in the assumption log, confirm it in writing with a date and owner, and add a risk with a trigger date in case it is late.
C. Delete it from the charter.
D. Wait and see.

**Correct answer: B.**
**Why correct:** Unverified assumptions can become risks or issues. Confirming them early and tracking a trigger gives you warning.
**Why others are wrong:** A relies on memory. C hides a dependency. D loses the early warning.
**Takeaway:** Validate assumptions early and write them down.

---

**Q183 | Scope (WBS naming) | Intermediate | Multiple-select (select 2)**
Which two are well-formed, deliverable-focused WBS elements?
A. Login page
B. Do the coding
C. Test report
D. Work on stuff

**Correct answer: A and C.**
**Why correct:** They name tangible, verifiable outputs.
**Why others are wrong:** B and D describe vague activity with no clear output.
**Concept:** WBS design. **Takeaway:** Name WBS elements as nouns (outputs), and use verbs later, when listing activities.

---

**Q184 | Scope (validation vs. quality control) | Intermediate | Matching**
Match each situation to the correct term.
1. The team tests the login page against its specification before the demo.
2. The sponsor reviews the finished app and signs acceptance.
3. A stakeholder asks for a new report after approval.
4. A developer adds an unrequested export feature.
a. Gold plating
b. Control quality (team verification)
c. Change request
d. Validate scope (customer acceptance)

**Correct answer: 1-b, 2-d, 3-c, 4-a.**
**Why:** Quality control is internal checking, and validation is customer acceptance. A post-approval request is a change, and unrequested extras are gold plating.
**Takeaway:** Quality control comes first, then validation.

---

**Q185 | Business case (ROI, payback) | Advanced | Numerical (select 1)**
A project costs $20,000 and is expected to produce $9,000 of net benefit per year for 3 years. What are the simple ROI and payback period?
A. ROI 35%; payback about 2.2 years
B. ROI 135%; payback 3 years
C. ROI 35%; payback 3 years
D. ROI 45%; payback about 2.2 years

**Correct answer: A.**
**Calculation:** Total benefit = 3 × 9,000 = 27,000. Net gain = 27,000 − 20,000 = 7,000. ROI = 7,000 ÷ 20,000 = **35%**. Payback = 20,000 ÷ 9,000 = **2.2 years**.
**Why others are wrong:** B treats total benefit as net gain. C uses the whole benefit period as payback. D has the wrong ROI.
**Plain English:** The project repays its cost in a little over two years and returns 35% on the money over three years. These are simple measures that ignore the time value of money **[Supplemental]**.
**Takeaway:** Show sponsors both ROI and payback.

---

## Planning and Schedule (Q186 to Q189)

**Q186 | Critical Path | Advanced | Numerical (select 1)**
A (2 days) is first. B (5 days) and C (3 days) follow A. D (4 days) follows B. E (6 days) follows C. F (2 days) follows both D and E. What is the project duration, and how many critical paths exist?
A. 13 days; one critical path
B. 13 days; two critical paths
C. 26 days; two critical paths
D. 15 days; one critical path

**Correct answer: B.**
**Calculation:** A-B-D-F = 2 + 5 + 4 + 2 = **13**. A-C-E-F = 2 + 3 + 6 + 2 = **13**. Both paths are equally long.
**Why others are wrong:** A misses the second path. C adds both paths together. D has no basis.
**Plain English:** Every task is critical, so a delay anywhere delays the project.
**Takeaway:** More than one critical path means higher schedule risk.

---

**Q187 | Schedule (float) | Intermediate | Numerical (select 1)**
A non-critical task has 4 days of total float and is delayed by 6 days. By how much does the project end date move?
A. 0 days
B. 2 days
C. 4 days
D. 6 days

**Correct answer: B.**
**Calculation:** 6 − 4 = **2 days** beyond the float.
**Why others are wrong:** A ignores the excess. C is the float, not the delay. D ignores the float.
**Takeaway:** A delay moves the end date only by the amount that exceeds the float.

---

**Q188 | Schedule compression (crashing) | Advanced | Numerical (select 1)**
You must save 3 days. A and B are on the only critical path. A can be crashed up to 2 days at $500 per day. B can be crashed up to 3 days at $300 per day. C is not critical (5 days of slack) and costs $100 per day to crash. What is the cheapest way to save 3 days?
A. Crash C for 3 days ($300)
B. Crash B for 3 days ($900)
C. Crash A for 2 days and B for 1 day ($1,300)
D. Crash A for 3 days ($1,500)

**Correct answer: B.**
**Why correct:** Only critical-path tasks shorten the project, and B is the cheapest critical task per day.
**Why others are wrong:** A crashes a non-critical task, which saves no time. C costs more. D exceeds A's 2-day limit.
**Takeaway:** Crash the cheapest critical task first, and recheck the critical path afterwards. Another path can become critical.

---

**Q189 | Procurement | Intermediate | Matching**
Match each document to its purpose.
1. RFI (request for information)
2. RFQ (request for quotation)
3. RFP (request for proposal)
4. SOW (statement of work)
a. Asks vendors to propose a solution and price for a problem
b. Describes the work the vendor will perform
c. Gathers general information about vendor capabilities
d. Requests prices for clearly defined items

**Correct answer: 1-c, 2-d, 3-a, 4-b.**
**Why:** RFI explores, RFQ prices defined items, RFP invites solutions, and SOW defines the work.
**Takeaway:** Choose the document by how well defined your need is.

---

## Budget and Earned Value (Q190 to Q195)

**Q190 | Earned Value | Advanced | Numerical (select 1)**
BAC = $150,000, PV = $75,000, EV = $60,000, AC = $80,000. What are CV, CPI, and SPI?
A. CV −$20,000; CPI 0.75; SPI 0.80
B. CV −$20,000; CPI 1.33; SPI 0.80
C. CV +$20,000; CPI 0.75; SPI 1.25
D. CV −$15,000; CPI 0.75; SPI 0.80

**Correct answer: A.**
**Calculation:** CV = 60,000 − 80,000 = **−20,000**. CPI = 60,000 ÷ 80,000 = **0.75**. SPI = 60,000 ÷ 75,000 = **0.80**.
**Why others are wrong:** B inverts CPI. C flips signs and ratios. D uses SV (−15,000) as CV.
**Plain English:** The project is over budget and behind plan. It earns 75 cents per dollar spent and runs at 80% of the planned pace.
**Takeaway:** EV is always the numerator.

---

**Q191 | Forecasting | Advanced | Numerical (select 1)**
Using Q190's figures, and assuming current cost performance continues, what are EAC and ETC?
A. EAC $200,000; ETC $120,000
B. EAC $170,000; ETC $90,000
C. EAC $200,000; ETC $200,000
D. EAC $150,000; ETC $70,000

**Correct answer: A.**
**Calculation:** EAC = BAC ÷ CPI = 150,000 ÷ 0.75 = **$200,000**. ETC = 200,000 − 80,000 = **$120,000**.
**Why others are wrong:** B uses the one-off formula, AC + (BAC − EV) = 170,000. C forgets to subtract AC. D assumes no overrun.
**Plain English:** At this rate the project finishes $50,000 over budget.
**Takeaway:** "Continues" means BAC ÷ CPI, and "one-off" means AC + (BAC − EV).

---

**Q192 | Earned Value (from task progress) | Intermediate | Numerical (select 1)**
Three tasks make up BAC = $60,000. Task 1 ($10,000 budget) is 100% complete. Task 2 ($20,000) is 50% complete. Task 3 ($30,000) has not started. AC = $22,000. What are EV, percent complete, and CPI?
A. EV $20,000; 33%; CPI 0.91
B. EV $30,000; 50%; CPI 1.36
C. EV $22,000; 37%; CPI 1.00
D. EV $60,000; 100%; CPI 2.73

**Correct answer: A.**
**Calculation:** EV = 10,000 + (0.5 × 20,000) + 0 = **$20,000**. Percent complete = 20,000 ÷ 60,000 = **33%**. CPI = 20,000 ÷ 22,000 = **0.91**.
**Why others are wrong:** C uses AC as EV. B and D give EV values the task progress does not support.
**Takeaway:** EV counts work completed, not money spent.

---

**Q193 | Forecasting | Intermediate | True/False**
"A CPI of 1.0 at 20% complete guarantees the project will finish on budget."

**Correct answer: False.**
**Why:** CPI describes performance to date. Later work can cost more or less, and risks can occur. EAC is a forecast, not a guarantee.
**Takeaway:** Update forecasts regularly and watch the trend.

---

**Q194 | Budget variance | Beginner | Numerical (select 1)**
A task's budget was $8,000 and its actual cost was $7,200. What is the budget variance?
A. −$800 (10% over)
B. +$800 (10% under)
C. +$800 (11% under)
D. +$7,200

**Correct answer: B.**
**Calculation:** 8,000 − 7,200 = **+800**. 800 ÷ 8,000 = **10%** under.
**Why others are wrong:** A has the wrong sign. C divides by actual cost. D is the actual cost.
**Takeaway:** Positive means under budget.

---

**Q195 | Monitoring (SV and the critical path) | Advanced | Scenario (select 1)**
SPI is 0.78 and SV is negative. All critical-path tasks are on time. The late tasks have 10 days of float. What is the best action?
A. Immediately add resources to everything.
B. Check which late tasks are on the critical path, confirm the float is real, keep monitoring, and avoid costly compression that the end date doesn't need.
C. Report the project as failed.
D. Ignore the schedule data.

**Correct answer: B.**
**Reasoning:** SV and SPI are measured in money and ignore the network logic. If the late tasks have float, the end date may be safe.
**Why others are wrong:** A spends money without need. C is an overreaction. D ignores a warning.
**Takeaway:** Pair earned value metrics with the critical path.

---

## Risk (Q196 to Q198)

**Q196 | Risk analysis | Intermediate | MCQ (select 1)**
Which technique is a **quantitative** risk analysis technique?
A. A probability-impact matrix with scores from 1 to 5
B. Calculating expected monetary value (EMV)
C. A brainstorming session
D. Reviewing the register for owners

**Correct answer: B.**
**Why:** EMV uses actual probabilities and money. **Why others are wrong:** A ranks with scales (qualitative), C identifies risks, and D is a review.
**Takeaway:** Qualitative ranks, and quantitative puts numbers on exposure.

---

**Q197 | Risk response | Advanced | Scenario (select 1)**
Risk: "The only developer who knows the payment code might leave" (probability 3, impact 5). Which response best **mitigates** it?
A. Accept and hope.
B. Cross-train a second developer and require written documentation.
C. Delete the risk from the register.
D. Ask the developer to promise not to leave.

**Correct answer: B.**
**Reasoning:** Cross-training and documentation reduce the impact if the developer leaves. The score is 3 × 5 = 15, which is high on the course scale.
**Why others are wrong:** A takes no action on a high risk. C erases it. D controls nothing.
**Takeaway:** Reduce single points of failure.

---

**Q198 | Risk (reserves) | Advanced | MCQ (select 1) [Supplemental]**
An **unidentified** risk occurs and needs funding. Under PMBOK terminology, where does the money come from?
A. Contingency reserve
B. Management reserve, released with management approval
C. The baseline tasks
D. Team overtime

**Correct answer: B.**
**Why:** Management reserve covers unknown risks and sits outside the cost baseline. Contingency reserve covers identified risks and sits inside it.
**Why others are wrong:** A is for known risks. C takes money from planned work. D is not a funding source.
**Takeaway:** Know where each reserve sits and who approves it.

---

## Stakeholders and Communication (Q199 to Q202)

**Q199 | Stakeholder analysis | Advanced | Scenario (select 1)**
A new executive joins mid-project and is skeptical. What should you do first?
A. Avoid them.
B. Add them to the stakeholder register, meet them to understand their expectations and concerns, and adjust the communication plan.
C. Send them the full project archive.
D. Wait until they raise objections.

**Correct answer: B.**
**Reasoning:** New, powerful stakeholders change the engagement picture. Early conversation turns uncertainty into information.
**Why others are wrong:** A and D leave concerns unaddressed. C overwhelms them.
**Takeaway:** Update the register when people change.

---

**Q200 | Communication (status report) | Intermediate | Multiple-select (select 3)**
Which three belong in a one-page sponsor status report?
A. Overall status (RAG) and forecast
B. Top risks
C. Decisions needed
D. Every developer's daily timesheet
E. The full source code

**Correct answer: A, B, C.**
**Why others are wrong:** D and E are too detailed for a sponsor update.
**Takeaway:** Executives need status, risks, and decisions.

---

**Q201 | Communication (practical message) | Advanced | Short answer**
Write a three-sentence message to the sponsor reporting a forecast overrun. The CPI is 0.90 and the forecast is $5,000 over.

**Model answer:** "Current forecast is $5,000 over budget because CPI is 0.90. I recommend deferring two low-priority features to close about $3,500 of the gap, and using contingency for the rest. Could you confirm by Friday so the team can plan next week?" Any version that gives the bottom line, the cause or metric, options or a recommendation, and a decision date is acceptable.
**Takeaway:** Lead with the forecast, then the plan and the ask.

---

**Q202 | Communication | Beginner | True/False**
"If nobody objects in a meeting, you can assume everyone agrees."

**Correct answer: False.**
**Why:** Silence can mean agreement, confusion, or reluctance to speak. Ask directly and confirm decisions in writing.
**Takeaway:** Check understanding explicitly.

---

## Teams and Leadership (Q203 to Q205)

**Q203 | Team leadership (situational) | Intermediate | MCQ (select 1) [Supplemental]**
A new team member is enthusiastic but inexperienced. Which leadership style fits best?
A. Hands-off, with full autonomy
B. Clear direction, examples, and regular check-ins, increasing autonomy as skill grows
C. Ignore them
D. Criticize mistakes publicly

**Correct answer: B.**
**Why:** Low skill with high motivation needs direction and support. **Why others are wrong:** A overwhelms them, C wastes motivation, and D damages trust.
**Takeaway:** Adjust your style to the person and the task.

---

**Q204 | Team management (workload) | Advanced | Scenario (select 1)**
The team has worked 60-hour weeks for a month, and defects are rising. What is the best action?
A. Keep going until the deadline.
B. Acknowledge the strain, then with the sponsor reduce load through scope, date, or resource options, rebalance work, and protect rest time.
C. Replace the entire team.
D. Hide the defect numbers.

**Correct answer: B.**
**Reasoning:** Chronic overtime reduces quality and raises the risk of turnover. The fix is a trade-off decision, not more effort.
**Why others are wrong:** A worsens the cause. C is disproportionate. D hides the evidence.
**Takeaway:** Sustainable pace protects quality.

---

**Q205 | Escalation | Intermediate | Multiple-select (select 3)**
Which three belong in an effective escalation message?
A. Facts and impact
B. What you have already tried
C. A specific ask and your recommendation
D. Blame for a named person
E. Waiting until the last possible moment

**Correct answer: A, B, C.**
**Why others are wrong:** D damages relationships. E removes options.
**Takeaway:** Escalate early, factually, and with a proposal.

---

## Quality (Q206 to Q209)

**Q206 | Root-cause analysis | Advanced | MCQ (select 1)**
Which order best describes a problem-solving cycle for a recurring defect?
A. Fix the symptom, close the issue, then investigate
B. Define the problem, gather data, find root causes, implement corrective or preventive action, verify the result
C. Find a person to blame, retrain them, move on
D. Implement a preventive action, then define the problem

**Correct answer: B.**
**Why:** Evidence comes before action, and verification confirms the action worked. **Why others are wrong:** A, C, and D skip or reverse key steps.
**Takeaway:** Verify that the fix removed the cause.

---

**Q207 | Quality metrics | Intermediate | Numerical (select 1)**
200 test cases were run and 188 passed. The target pass rate is 95%. What is the current rate, and how many more must pass?
A. 94%; 2 more
B. 94%; 5 more
C. 95%; 0 more
D. 88%; 12 more

**Correct answer: A.**
**Calculation:** 188 ÷ 200 = **94%**. 95% × 200 = 190, so **2 more** are needed.
**Why others are wrong:** B and D use wrong figures. C rounds the result up to the target.
**Takeaway:** Compare the exact figure with the target.

---

**Q208 | Cost of quality | Advanced | Numerical (select 1) [Supplemental]**
Costs: prevention $4,000, appraisal $6,000, internal failure $5,000, external failure $15,000. What is the total cost of quality, and what share is failure cost?
A. $30,000; about 67%
B. $30,000; about 33%
C. $20,000; 100%
D. $15,000; 50%

**Correct answer: A.**
**Calculation:** Total = 4,000 + 6,000 + 5,000 + 15,000 = **$30,000**. Failure = 5,000 + 15,000 = 20,000, and 20,000 ÷ 30,000 = **67%**.
**Why others are wrong:** B is the prevention and appraisal share. C and D use wrong totals.
**Plain English:** Two-thirds of the quality spend is paying for defects. Better prevention would likely cost less.
**Takeaway:** Shift spending toward prevention.

---

**Q209 | Quality assurance (terminology) | Advanced | Scenario (select 1)**
In an interview, you are asked about "QA." Your last company's "QA team" mainly ran tests. What is the best approach?
A. Assume the interviewer means testing.
B. Clarify the terms: in project management, QA is process-focused and preventive, and QC is product-focused testing. Then answer about both.
C. Say QA and QC are the same.
D. Avoid the question.

**Correct answer: B.**
**Reasoning:** The word is used differently in software companies and in PMBOK-style terminology, so state your definition and answer both.
**Why others are wrong:** A risks a mismatch. C is inaccurate. D loses the chance to show knowledge.
**Takeaway:** Define terms before answering.

---

## Change Management (Q210 to Q212)

**Q210 | Change control | Intermediate | MCQ (select 1)**
A change has been approved. What must happen next?
A. Nothing.
B. Update the schedule, budget, and other baselines, implement the change, and communicate the decision to everyone affected.
C. Archive the request.
D. Ask for a second approval.

**Correct answer: B.**
**Why:** An approved change is only effective if plans and people are updated. **Takeaway:** A decision is not done until the people doing the work know about it.

---

**Q211 | Change control (impact) | Advanced | Numerical (select 1)**
A change adds 4 days to a critical-path task and $2,400 of cost. The schedule has a 2-day buffer. The current budget is $30,000. If approved, what are the net schedule delay and the revised budget?
A. 2 days; $32,400
B. 4 days; $32,400
C. 2 days; $27,600
D. 6 days; $32,400

**Correct answer: A.**
**Calculation:** Net delay = 4 − 2 = **2 days**. Revised budget = 30,000 + 2,400 = **$32,400**.
**Why others are wrong:** B ignores the buffer. C subtracts the cost. D adds the buffer to the delay.
**Takeaway:** Contingency reserve is for risks, not scope changes. A change normally needs an approved budget adjustment.

---

**Q212 | Change management (ADKAR) | Intermediate | Scenario (select 1)**
Staff understand the need for the new tool, want it, and were trained. But the new workflow needs double data entry, so they cannot work efficiently. Which ADKAR element is weakest?
A. Awareness
B. Desire
C. Knowledge
D. Ability

**Correct answer: D.**
**Why:** Ability is being able to do it in practice. The workflow, not understanding, is the barrier. **Takeaway:** Remove practical obstacles, and give practice time and support.

---

## Agile, Scrum, and Kanban (Q213 to Q217)

**Q213 | Sprint Review | Intermediate | Multiple-select (select 3)**
Which three belong in a Sprint Review?
A. Demonstrating the Increment
B. Discussing progress toward the Product Goal and what to do next
C. Collecting stakeholder feedback
D. Assigning blame for missed items
E. Individual performance appraisals

**Correct answer: A, B, C.**
**Why others are wrong:** D and E do not belong in a Scrum event.
**Takeaway:** The review inspects the product, and the retrospective inspects the process.

---

**Q214 | Sprint scope | Advanced | Scenario (select 1)**
Mid-sprint, the Developers see they can finish 4 of 6 items, and the Sprint Goal is still achievable with 4. What should they do?
A. Cancel the sprint.
B. Talk with the Product Owner and renegotiate the scope under the Sprint Goal, moving the other items back to the backlog.
C. Change the Sprint Goal.
D. Work unpaid overtime.

**Correct answer: B.**
**Reasoning:** The Sprint Goal stays fixed, and scope under it is flexible by agreement with the PO.
**Why others are wrong:** A is only for an obsolete goal, and only the PO can do it. C breaks the commitment. D hides capacity limits.
**Takeaway:** Protect the goal, and negotiate the scope.

---

**Q215 | Agile Metrics (forecast range) | Advanced | Numerical (select 1)**
The last five sprint velocities were 18, 22, 20, 24, and 16. 120 points remain. What is a reasonable forecast range, and what does the average give?
A. 5 to 8 sprints; the average (20) gives 6 sprints
B. 5 to 6 sprints; the average gives 6 sprints
C. 6 to 8 sprints; the average gives 7 sprints
D. 4 to 7 sprints; the average gives 5 sprints

**Correct answer: A.**
**Calculation:** Best case: 120 ÷ 24 = **5**. Worst case: 120 ÷ 16 = 7.5, so **8**. Average = 100 ÷ 5 = 20, and 120 ÷ 20 = **6**.
**Plain English:** A range is more honest than one number, and you refresh it every sprint.
**Takeaway:** Forecast with a range and update it.

---

**Q216 | Agile Metrics (burndown) | Advanced | Numerical (select 1)**
A 10-day sprint starts with 50 points. After day 6, 28 points remain. How far behind the ideal line is the team, and what daily rate is needed to finish?
A. 8 points behind; 7 points per day
B. 8 points ahead; 7 points per day
C. 8 points behind; 5 points per day
D. 6 points behind; 7 points per day

**Correct answer: A.**
**Calculation:** Ideal after day 6 = 50 − 30 = 20 remaining. Actual = 28, so **8 behind**. Required rate = 28 ÷ 4 days = **7 per day**. The team has so far finished 22 points in 6 days, about 3.7 per day.
**Why others are wrong:** B reverses the direction. C uses the ideal rate. D has the wrong gap.
**Takeaway:** The required rate is nearly double the actual rate, so talk to the PO about scope under the Sprint Goal, not just "work faster."

---

**Q217 | Kanban (flow metrics) | Advanced | Numerical (select 1)**
A request arrives on day 0, work starts on day 4, and it is delivered on day 9. What are its lead time and cycle time?
A. Lead time 9 days; cycle time 5 days
B. Lead time 5 days; cycle time 9 days
C. Lead time 4 days; cycle time 9 days
D. Both 9 days

**Correct answer: A.**
**Why:** Lead time runs from request to delivery (9). Cycle time runs from work start to delivery (9 − 4 = 5).
**Why others are wrong:** B and C swap or misread the terms. D ignores the waiting time.
**Takeaway:** A long gap between the two means requests wait too long before work starts.

---

## Closure and Career (Q218 to Q220)

**Q218 | Project Closure (acceptance) | Advanced | Scenario (select 1)**
At acceptance, the sponsor finds three minor defects and says she won't sign. What is the best approach?
A. Argue that they are unimportant.
B. Classify the defects, agree which are fixed now and which are deferred, and record that in a signed acceptance with owners and warranty fix dates.
C. Close the project without her signature.
D. Restart testing from the beginning.

**Correct answer: B.**
**Reasoning:** Acceptance can record known exceptions, so minor defects do not have to block closure.
**Why others are wrong:** A dismisses her concerns. C removes formal acceptance. D is disproportionate.
**Takeaway:** Document exceptions instead of leaving them open and ownerless.

---

**Q219 | Project Closure (early closure) | Intermediate | MCQ (select 1)**
A project is cancelled at 60% because funding ended. Which action is **not** appropriate?
A. Document the status and reasons.
B. Release the team and tell their managers.
C. Delete all records and skip lessons learned.
D. Settle contracts and costs.

**Correct answer: C.**
**Why:** Records and lessons are the most valuable output of an early closure. **Why others are wrong:** A, B, and D are normal early-closure steps.
**Takeaway:** Early closure still needs proper closure.

---

**Q220 | Interviewing (STAR) | Advanced | Short answer (practical)**
Outline a STAR answer to "Tell me about a time you missed a deadline." Use clearly marked **example** details.

**Model answer (example, not real facts):**
*Situation:* A payment feature was due in week 6, and the vendor's sandbox arrived 8 days late.
*Task:* I was responsible for protecting the launch date and keeping the sponsor informed.
*Action:* I told the sponsor immediately with options, built a mock API so development continued, and re-sequenced non-critical work. I recorded the cause in the risk log.
*Result:* We missed the original feature date by two days but kept the launch date. We now get vendor dates in writing and build mocks early.
**Takeaway:** Own the miss, show what you did and what you learned, and use only true facts in a real interview.

---

## Part 8E Score Sheet

Give yourself 1 point per correct answer. For multiple-select and matching, count the question correct only if every part is right. For short-answer questions, count it correct if your answer covers the main points of the model answer.

| Topic | Questions | Your score |
|---|---|---|
| Foundations, initiation, scoping | Q181 to Q185 (5) | ___ |
| Planning and schedule | Q186 to Q189 (4) | ___ |
| Budget and earned value | Q190 to Q195 (6) | ___ |
| Risk | Q196 to Q198 (3) | ___ |
| Stakeholders and communication | Q199 to Q202 (4) | ___ |
| Teams and leadership | Q203 to Q205 (3) | ___ |
| Quality | Q206 to Q209 (4) | ___ |
| Change | Q210 to Q212 (3) | ___ |
| Agile, Scrum, Kanban | Q213 to Q217 (5) | ___ |
| Closure and career | Q218 to Q220 (3) | ___ |
| **Total** | **40** | ___ |

**Reading your result:** this isn't an official pass mark. Review any topic where you missed more than a third of the questions.

**Running total:** Q1 to Q220 are done (Part 1: 20, 8A to 8E: 40 each). The question bank now exceeds the 200-question requirement.

## Part 8E Checkpoint

Without looking back:
1. In Q186, why do all six tasks have zero slack?
2. If a non-critical task with 4 days of float slips 6 days, how far does the end date move?
3. What is the difference between lead time and cycle time?

**What next?** The four full-length mock tests are next. Each has 50 new questions, so none repeat Q1 to Q220. I suggest two messages per test, so the questions are shown first without answers, as you asked:
- **Message 1:** the 50 questions only
- **Message 2:** the answer key with explanations, a score sheet, and topic-wise analysis

---

