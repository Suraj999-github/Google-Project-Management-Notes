# Part 7: Project Closure and Practical Templates

**Source note:** As publicly described, Google's *Project Execution* course ends with closing a project: confirming deliverables, capturing lessons learned, and recognizing the team. I haven't re-checked Coursera live, so confirm the current contents there. **[Supplemental]** marks my additions (PMBOK terms, benefits realization, premature closure). The templates, numbers, and questions are my original material, not official Google content.

This part covers **Skill 18 (Project Closure)**. It also supplies the two templates not yet built, the **lessons-learned register** and the **project closure report**, and shows how every document evolves across the life cycle. Skills 19 and 20 (web presence and interviewing) come in Part 9.

---

## 1. Learning Objectives

By the end of Part 7 you should be able to:
- Verify deliverables against acceptance criteria and obtain formal sign-off
- Complete administrative, contract, and financial closure
- Hand deliverables over to the people who will operate them
- Release the team, recognize their work, and capture lessons learned
- Measure results against the original goals and write a closure report
- Decide what to do when a project must close early or with incomplete deliverables
- Trace each project document from initiation to closure

**Running example:** BrightCuts Online Booking App (the predictive version), at the end of week 12.

---

## 2. How the Pieces Connect

```
Charter goals + acceptance criteria (Part 2)
              ↓
   Verify deliverables (UAT, test report) → Customer acceptance
              ↓
 Close contracts and money → Hand over to operations → Release team
              ↓
   Lessons learned → Archive → Measure outcomes → Closure report
```

Closure is where the **charter** (goals), **scope statement** (acceptance criteria), **quality plan** (evidence), **budget and schedule** (final numbers), **risk and issue logs** (open items), and **stakeholder register** (who must sign off) all come back together. A project with weak documents in earlier phases has a hard time proving it succeeded.

---

## 3. Skill 18: Project Closure

**Definition:** Formally finishing a project or phase: confirming the work is complete and accepted, settling contracts and finances, transferring the results to the people who will use or support them, releasing resources, recording lessons, and reporting results against the original goals.

**Why it matters:**
- Unclosed projects leave open contracts, unpaid invoices, unclear ownership, and team members still assigned.
- Without acceptance, "done" is an opinion and disputes follow.
- Lessons learned are the main way an organization improves, and they are easily lost if you skip them.
- A clear closure report is evidence of your results for your sponsor, your organization, and your own portfolio.

**When to use it:** at the end of the project, and at the end of each major phase **[Supplemental]**. PMBOK calls this process "Close Project or Phase."

### Normal vs. early closure

| Type | When | Main difference |
|---|---|---|
| **Normal closure** | Objectives met and deliverables accepted | Full verification and handover |
| **Early / premature closure [Supplemental]** | Sponsor cancels, funding ends, strategy changes, or the project is no longer viable | Document what was done and why it stopped, protect reusable work, settle commitments |

Ending a project early is **not** a failure of closure. Failing to close it properly is.

### Step-by-step closure process

1. **Confirm completion.** Check every deliverable against its acceptance criteria and the scope statement.
2. **Get formal acceptance.** The sponsor or customer signs. Verbal "looks good" is not enough.
3. **Resolve open items.** Close or transfer open issues, defects, change requests, and risks. Each remaining item needs a named owner.
4. **Complete administrative closure.** Final status report, financial reconciliation, timesheets, and document updates.
5. **Close contracts and procurements.** Confirm vendors delivered, pay final invoices, return or cancel access, and record any warranty terms.
6. **Hand over to operations.** Transfer deliverables, credentials, documentation, training, and support arrangements.
7. **Release the team.** Return people to their managers or next assignments, and tell their managers how they performed.
8. **Run a lessons-learned session.** Capture what worked, what didn't, and what to do differently.
9. **Archive project documents.** Store them where they can be found, with version control and access rules.
10. **Measure results.** Compare outcomes with the charter's SMART goals, and set a date for measuring any benefits that appear only after launch.
11. **Report and celebrate.** Issue the closure report and recognize the team.

### Two ideas often confused

| Term | Meaning | Owner |
|---|---|---|
| **Scope validation (acceptance)** | The customer formally accepts deliverables | Sponsor / customer |
| **Quality control** | The team checks deliverables against requirements before presenting them | Team |

Quality control happens first, then validation. A deliverable can pass quality control and still be rejected if it doesn't meet the customer's real need, which is why acceptance criteria must be written at scoping.

### Project closure in Agile

| Topic | Agile practice |
|---|---|
| Delivery | Increments are released throughout. There is no single "go-live moment" unless you plan one |
| Acceptance | The Product Owner accepts items against acceptance criteria and the Definition of Done |
| End of work | The team stops when the Product Goal is reached, funding ends, or value no longer justifies the cost |
| Lessons | The Sprint Retrospective runs every sprint, and a final project retrospective is common practice |
| Handover | Release notes, operational documentation, support arrangements |
| Remaining backlog | Archived or handed to the product's ongoing owner |

A *product* may continue for years after a *project* closes.

### Template: Acceptance Verification (completed)

| Acceptance criterion (from the scope statement and quality plan) | Target | Result | Evidence | Met? |
|---|---|---|---|---|
| Customer completes a booking | Under 3 minutes | Average 2 min 10 s (5 UAT users) | UAT report | Yes |
| Page load time | Under 2 s for 95% of requests | 95% under 1.8 s | Performance test | Yes |
| System test pass rate | At least 95% | 97.5% (39 of 40) | Test report | Yes |
| Critical defects open | Zero | Zero | Defect log | Yes |
| High-severity defects open | Zero | Zero | Defect log | Yes |
| Low-severity defects | Deferred only with approval | 1 deferred (misaligned icon), approved by Maria | Change and defect log | Yes |
| Staff trained | All users | Tom and 4 stylists trained | Training sign-in sheet | Yes |
| Admin dashboard, reminders (email), cancellation, payment at booking | Delivered | Delivered | Demo and sign-off | Yes |
| SMS reminders | Deferred | Deferred via CR-003 | Change log | Approved scope change |

### Template: Formal Acceptance Sign-off (completed)

| Field | Content |
|---|---|
| Project | BrightCuts Online Booking App |
| Deliverables accepted | Customer booking app, admin dashboard, email reminders, training guide |
| Approved scope changes | CR-003 (SMS deferred), CR-004 (payment API migration) |
| Known open items | 1 low-severity defect (D-18); SMS reminders and loyalty points in phase 2 |
| Statement | "The deliverables listed meet the agreed acceptance criteria, with the exceptions recorded above." |
| Accepted by / date | Maria Lopez, Sponsor, Week 12 |

### Template: Project Closure Checklist (completed)

| # | Task | Owner | Done? |
|---|---|---|---|
| 1 | All deliverables verified against acceptance criteria | PM | ✔ |
| 2 | Formal acceptance signed | Maria | ✔ |
| 3 | Open issues: closed or assigned to an owner | PM | ✔ |
| 4 | Open risks: closed, or transferred to operations (e.g., payment provider changes) | PM | ✔ |
| 5 | Final invoices paid (designer, QA contractor, hosting) | PM / Maria | ✔ |
| 6 | Vendor contracts closed or moved to operations (payment provider, hosting) | PM | ✔ |
| 7 | Project cost reconciled with the finance records | PM | ✔ |
| 8 | Source code, credentials, and documents transferred to Maria's account | Dev | ✔ |
| 9 | Admin and user training completed and guide delivered | PM / Tom | ✔ |
| 10 | Support plan agreed (30-day warranty for defect fixes, then ongoing support contract) | PM / Maria | ✔ |
| 11 | Team released and managers informed | PM | ✔ |
| 12 | Lessons-learned session held and register completed | PM | ✔ |
| 13 | Project documents archived | PM | ✔ |
| 14 | 30- and 90-day benefit reviews scheduled | Maria / PM | ✔ |
| 15 | Closure report issued | PM | ✔ |
| 16 | Team and contributors thanked | PM / Maria | ✔ |

### Template: Handover Plan (completed)

| Item | From | To | How | Date |
|---|---|---|---|---|
| Live app and admin access | Dev | Maria and Tom | Credentials transferred, ownership changed to Maria's accounts | Wk 12 |
| Source code and technical documentation | Dev | Maria (stored in her repository) | Handover session, written guide | Wk 12 |
| User guide and training videos | PM | Tom and stylists | Hands-on session and shared folder | Wk 11 to 12 |
| Support process | PM | Dev (support contract, $150/month) | Email address, response times, defect-reporting steps | Wk 12 |
| Open vendor relationships | PM | Maria | Introduction to the payment provider's account manager | Wk 12 |
| Open risks (e.g., API version changes) | PM | Maria and Dev | Recorded in an operations risk list | Wk 12 |
| Phase 2 backlog (SMS, loyalty points, reports) | PM | Maria | Prioritized list | Wk 12 |

**Handover rule:** the receiving person confirms they can operate the product. Sending the documents is not the same as completing the handover.

### Template: Lessons-Learned Register (completed)

Run the session soon after delivery, while memories are fresh. Include the whole team and key stakeholders, focus on **process and facts, not blame**, and record actions with owners.

| ID | Area | What happened | Impact | Lesson / recommendation | Owner | Applies to |
|---|---|---|---|---|---|---|
| L-01 | Scope | Stylists' needs were gathered only through Maria | Late expectation gap (week 11 stylists' workshop) | Consult every affected user group at requirements stage | PM | All projects |
| L-02 | Risk | Payment provider's sandbox arrived 8 days late | 2 days lost, protected by mock API | Get vendor dates in writing, build mocks early, set trigger dates | PM / Dev | Vendor-dependent projects |
| L-03 | Quality | Double-booking defect found only in system test | Rework and risk to the launch date | Add scenario reviews for concurrency to requirements checklist | Dev / Sam | Software projects |
| L-04 | Change | Weekly informal changes from sponsor early in the project | Rework before the change process existed | Set up change control and weekly decision meeting at kickoff | PM | All projects |
| L-05 | Communication | One-page weekly status with a "decision needed" section | Faster decisions, no surprises | Keep the format; use it as a template | PM | All projects |
| L-06 | Team | Design handoff process agreed after Priya and Dev conflict | Short-term rework | Agree a design-feasibility feedback rule in the team agreement at the start | PM | Cross-functional teams |
| L-07 | Estimating | Payment integration underestimated | Overran by about $1,300 in dev labor | Use three-point estimates for integrations; add a spike for unknown APIs | Dev | All estimates |
| L-08 | Monitoring | "Done but untested" tasks reported as green | Delayed discovery of risk | Add "built, not verified" as a status | PM | All projects |

**Good practice:** lessons that stay in a spreadsheet nobody opens help nobody. Share them, store them where the next project team will look, and turn the best ones into checklist items.

### Template: Project Closure Report (completed)

| Section | Content |
|---|---|
| **1. Summary** | BrightCuts Online Booking App went live on schedule at the end of week 12. All Must and Should features were delivered except SMS reminders, which were deferred by an approved change. Final cost was within the revised approved budget. |
| **2. Goals vs. results** | See the table below |
| **3. Deliverables** | Customer booking app, admin dashboard, email reminders, payment at booking, training guide. All accepted by the sponsor |
| **4. Schedule** | Planned 12 weeks. Actual 12 weeks. Critical-path slips (booking flow, payment API) were absorbed with buffer and scope trimming |
| **5. Budget** | See the table below |
| **6. Scope changes** | CR-001 loyalty points (deferred to phase 2), CR-002 color-coded calendar (approved), CR-003 SMS deferred, CR-004 payment API migration |
| **7. Quality** | 97.5% test pass rate, zero critical or high defects open, UAT passed by 5 users, performance targets met |
| **8. Risks and issues** | Payment API delay occurred and was mitigated. Remaining risk (provider API changes) transferred to operations |
| **9. Stakeholder feedback** | Maria satisfied. Tom and stylists confident after training. Customer survey planned at 30 days |
| **10. Lessons learned** | Summary of register (L-01 to L-08). Full register attached |
| **11. Handover** | Completed (see handover plan). Support: 30-day warranty, then support contract |
| **12. Outstanding items and recommendations** | Phase 2 backlog (SMS, loyalty points, reports). Benefit reviews at 30 and 90 days. Renewal date for the payment provider contract |
| **13. Recognition** | Dev for the mock-API approach, Priya for the redesign under time pressure, Sam for the regression test suite, Tom for early feedback |
| **14. Approval** | Maria Lopez, Sponsor, date |

**Goals vs. results**

| Goal (from the charter) | Target | Result at closure | How and when it will be confirmed |
|---|---|---|---|
| Launch the booking app | Within 12 weeks | Live at week 12 | Achieved |
| Online share of bookings | 60% within 3 months of launch | Not measurable yet | Maria reviews booking data at 30 and 90 days |
| Reduce no-shows | 12% to 6% | Not measurable yet | Compare at 90 days |
| Reduce staff phone time | About 10 hours per week saved | Not measurable yet | Tom's time log at 90 days |
| Staff trained | All users | All trained | Achieved |

**Output vs. outcome:** at closure you can usually prove **outputs** (what was delivered). **Outcomes** (business results) often appear later. Name who will measure them and when, so they don't vanish. A closure report that claims benefits nobody has measured is a weak report.

**Final budget and performance**

| Item | Amount |
|---|---|
| Original baseline (including $3,000 contingency) | $30,000 |
| CR-003: SMS reminders deferred | −$2,000 |
| CR-004: payment API migration | +$1,500 |
| Approved budget increase (week 7) | +$1,000 |
| **Revised approved budget (final BAC)** | **$30,500** |
| **Actual cost at closure (AC)** | **$30,400** |
| Budget variance (budget − actual) | **+$100** (about 0.3% under) |
| Contingency used | $2,400 of $3,000 |

**Final earned value check (all scope complete):** EV = revised BAC = $30,500, PV = $30,500, AC = $30,400.
- CV = 30,500 − 30,400 = **+$100**, and CPI = 30,500 ÷ 30,400 ≈ **1.00**
- SV = 30,500 − 30,500 = **$0**, and SPI = **1.00**

**Plain English:** the project finished on schedule and about $100 under the revised budget. Note it finished *over the original $30,000 baseline* because the sponsor approved changes. Report both numbers honestly and explain the approved changes, so nobody misreads the result.

### Sample messages

**Closure announcement to stakeholders**
> **Subject:** BrightCuts Booking App: project complete
> The online booking app went live on schedule at the end of week 12, and Maria has accepted the deliverables. Staff are trained and the support arrangements are in place. SMS reminders and loyalty points are planned for phase 2. Business results (online booking share and no-show rate) will be reviewed at 30 and 90 days. The full closure report is attached. Thank you to everyone who contributed.

**Team recognition**
> Dev, your decision to build the mock API early saved us two weeks of delay when the payment sandbox arrived late. Priya, the redesign under time pressure kept our launch date. Sam, the regression suite caught the double-booking defect before customers did. Tom, your early feedback shaped the staff experience. Thank you all.

**Message to the people manager of a released team member**
> Sam completed testing on the BrightCuts project on 12 Dec. His regression suite caught a critical defect before launch, and his reports improved steadily after we clarified scope. He is available for reassignment from Monday.

---

## 4. How Documents Evolve Across the Life Cycle

| Document | Initiating | Planning | Executing | Closing |
|---|---|---|---|---|
| **Business case** | Created: problem, options, benefits | Referenced to justify budget | Revisited if the case changes | Compared with actual results |
| **Charter** | Created and signed | Source for scope and plans | Resolves disputes about authority | Basis for the goals-vs-results table |
| **SMART goals** | Defined | Drive scope and metrics | Tracked | Measured; outcomes scheduled |
| **Scope statement** | Created | Basis for WBS | Controlled through change log | Acceptance criteria verified |
| **Stakeholder register** | Created | Feeds the communication plan | Updated as attitudes change | Used for sign-off and thank-yous |
| **RACI** | Drafted | Finalized with the plan | Updated for role changes | Confirms who accepts and who hands over |
| **WBS / schedule / Gantt** | n/a | Created, baselined | Tracked, updated by approved changes | Final dates compared with baseline |
| **Budget** | High-level estimate | Detailed baseline | Tracked with CV, CPI | Final cost reconciled |
| **Risk register** | Early risks | Full analysis and responses | Reviewed weekly | Open risks closed or handed over |
| **Issue log** | n/a | n/a | Created and used daily | Closed or transferred |
| **Change request log** | n/a | Process defined | Used for every change | Full history in report |
| **Communication plan** | n/a | Created | Followed and adjusted | Closure communications |
| **Quality plan and checklists** | Quality needs noted | Created | QA and QC run | Test evidence supports acceptance |
| **Status reports** | n/a | n/a | Weekly | Final report feeds closure report |
| **Lessons learned** | Review past projects | Apply earlier lessons | Capture as you go | Final session and register |
| **Closure report** | n/a | n/a | n/a | Created |

**Agile projects:** the **product backlog, sprint plans, reviews, retrospectives, and burndown** evolve in the same way. The backlog replaces the WBS and scope statement, and retrospective notes feed the lessons-learned register.

### Template index (where each template appears)

| Template | Part |
|---|---|
| Business case, charter, scope statement, SMART goals, stakeholder register, power-interest matrix, RACI, change request log | 2 |
| WBS, schedule, Gantt, milestone plan, budget, probability-impact matrix, risk register | 3 |
| Communication plan, team agreement | 4 |
| Issue log, decision log, status report, defect log, quality management plan, QA/QC checklist, change request form, change management plan | 5 |
| Product backlog, user story, sprint planning, review and retrospective, burndown | 6 |
| Acceptance verification, closure checklist, handover plan, lessons-learned register, closure report | 7 |

---

## 5. Common Challenges and Solutions

| Challenge | Solution |
|---|---|
| Team moves on before closure is done | Make closure tasks part of the plan and budget, with owners and dates |
| Sponsor won't sign acceptance | Show results against the acceptance criteria, resolve specific objections, and record any agreed exceptions |
| Endless "small fixes" after delivery | Agree a warranty period and route later requests to a support process or phase 2 |
| Lessons learned turn into blame | Focus on process, use facts, and ask "what would we do differently?" |
| Nobody reads the lessons | Share a one-page summary and add key items to templates and checklists |
| Benefits can't be measured at closure | Name an owner and review dates, and report outputs and outcomes separately |
| Final invoices arrive after closure | Keep a short financial close-out window, with an owner |
| Documents scattered | Archive in one location with a clear index |
| Early closure feels awkward | Treat it as a professional decision: document, protect reusable work, settle commitments |

---

## 6. Common Mistakes

| Mistake | How to avoid |
|---|---|
| Treating closure as optional once the product is live | Include closure tasks in the plan |
| Accepting verbally | Get a signed acceptance with known exceptions listed |
| Leaving risks and issues "open" with nobody responsible | Close them or assign operational owners |
| Skipping handover training | Confirm the receiver can operate the product |
| Forgetting contracts and access | Use a checklist for vendors, accounts, and credentials |
| Reporting only the good news | State results honestly, including variances and approved changes |
| Claiming outcomes you haven't measured | Report outputs now and schedule outcome reviews |
| Not releasing the team formally | Notify their managers and provide feedback |
| Not archiving | Store documents so a future PM can find them |
| Forgetting to thank people | Recognize specific contributions |

---

## 7. Module Summary and Revision Notes

- Closure: **verify, accept, resolve open items, close contracts and money, hand over, release team, learn, archive, measure, report**.
- **Acceptance** is formal and written. Exceptions are recorded.
- **Handover** is complete only when the receiver can operate the product.
- **Outputs** (what you delivered) are proven at closure. **Outcomes** (business results) may need later reviews.
- A **lessons-learned session** focuses on process, not blame, and produces actions with owners.
- **Early closure** needs the same care: document status, protect reusable work, settle contracts, and capture lessons.
- Report final cost against both the **original baseline** and the **approved revised budget**.
- Agile products continue after the project ends. Retrospectives and release notes support closure.
- **Validate scope** (customer acceptance) is not the same as **control quality** (team checking).

---

## 8. Skill 18: Question Sets

*Brief explanations are included. The full 10-field format appears in the numbered bank in Part 8.*

### Beginner

1. **What is project closure?** The formal end of a project or phase, including acceptance, handover, release of resources, lessons learned, and reporting.
2. **Why do you obtain formal acceptance?** It proves the customer agrees the deliverables meet the criteria and prevents later disputes.
3. **What is a lessons-learned session?** A meeting where the team and stakeholders record what worked, what didn't, and what to improve.
4. **True or false: a project closes only when everything went perfectly.** False. Projects can close early or with exceptions, but still must be closed properly.
5. **Name two things to do with project documents at closure.** Archive them and make them findable for future projects.

### Intermediate

1. **Output vs. outcome?** An output is what the project delivers (the app). An outcome is the business result (60% online bookings).
2. **What does a handover plan include?** What is transferred, from whom to whom, how, when, plus training and support arrangements.
3. **What is procurement (contract) closure?** Confirming vendors delivered, paying final invoices, closing or transferring contracts, and recording warranties.
4. **Why measure results against the charter?** The charter holds the agreed goals, so it is the fair basis for judging success.
5. **Why is a warranty or support period useful?** It sets a clear boundary for fixing defects without reopening the project.

### Scenario

1. **The sponsor says "It looks fine" but won't sign.** Ask which acceptance criteria concern them, show the evidence, fix real gaps, and record any agreed exceptions in a signed statement. *Reasoning:* convert vague approval into documented acceptance.
2. **Two open defects remain at closure.** Rank them. If low severity, ask the sponsor to approve deferral and assign them to the support owner. *Reasoning:* nothing stays open without an owner and a decision.
3. **The team starts a new project before the lessons session.** Schedule a short session now, before memories fade. Ask managers to release people for 90 minutes and gather written input from anyone who can't attend.
4. **The sponsor asks for new features after acceptance.** Explain that the project is closing, log the requests in the phase 2 backlog, or open a new change or project with its own budget.
5. **The final invoice arrives after the project is closed.** Keep a defined close-out window and a named owner for late costs, and report the final figure in an addendum.

### Interview

1. **How do you close a project?** *Sample:* "I verify deliverables against the acceptance criteria, get written sign-off, resolve open items, close contracts, hand over to operations, release the team, hold a lessons-learned session, archive the documents, and report results against the charter."
2. **Tell me about a lessons-learned session you ran.** *Sample (STAR):* "A software launch had a late vendor delay. I ran a blame-free session with a simple 'what worked, what didn't, what next' structure. We recorded eight lessons with owners, and the vendor-date and mock-system practices went into our project template."
3. **How do you measure success at closure?** "I compare results with the SMART goals in the charter, report outputs now, and schedule reviews for outcomes that need time, with a named owner."
4. **What do you do when a project is cancelled?** "I document what was completed and why it stopped, protect reusable work, settle contracts and costs, release the team with feedback, and capture lessons."
5. **How do you ensure a smooth handover?** "I agree the plan with the receiving team, provide training and documentation, confirm they can operate the product, and set a support period for questions."

### Revision checklist
- [ ] I can list the closure steps in order
- [ ] I can complete an acceptance verification table
- [ ] I can write a handover plan and a lessons-learned register
- [ ] I can write a closure report with goals vs. results
- [ ] I can distinguish outputs from outcomes
- [ ] I can explain how to close a project early
- [ ] I can say how Agile closure differs from predictive closure

---

## 9. Case Studies (the final 2 of the 15)

### Case 14: A project that must be closed despite incomplete deliverables

| Element | Detail |
|---|---|
| Situation | In week 9, Maria tells you the salon's landlord is ending the lease, and the business must relocate. She cancels the project and will use an off-the-shelf booking tool at the new location. About 70% of the work is complete. |
| Main problem | The project must stop with deliverables unfinished, and commitments remain |
| Root cause | A business change outside the project's control (the sponsor's circumstances changed) |
| Options | (a) Stop immediately and walk away, (b) pause the project, (c) close it formally: document, protect reusable work, settle commitments |
| Recommended | (c). A pause makes sense only if work will resume, and Maria has said it won't |
| Step-by-step resolution | 1) Confirm the decision in writing with the sponsor. 2) Freeze work and assess what is complete, partial, and not started. 3) Check which deliverables have value (requirements, design, data model) and package them. 4) Review contracts: end Sam's contract, notify hosting and the payment provider, check cancellation terms and fees. 5) Reconcile costs and pay valid invoices (work done to date). 6) Release the team with feedback and tell their managers. 7) Run a short lessons-learned session. 8) Archive documents. 9) Write the closure report. |
| Relevant documentation | Written cancellation decision, status of deliverables, contract close-out notes, financial reconciliation, lessons-learned register, closure report |
| Stakeholder communication | Message below. Brief the team honestly and respectfully. Inform vendors in writing |
| Expected outcome | Clean ending, no hidden liabilities, reusable designs and requirements handed to Maria for her new setup, and clear records |
| Lessons | Early closure is a legitimate result. Protect the sponsor's investment by saving what has value |
| Possible exam question | "A sponsor cancels a project at 70% complete. What should the PM do?" Answer: formally close it by documenting status, handing over useful work, settling contracts, releasing the team, and recording lessons |

> **Message to sponsor:** "Maria, thank you for letting us know early. To close the project properly, I will confirm what's done and what isn't, package the requirements and designs so you can use them with the new booking tool, and settle our contracts with the contractor, hosting, and payment provider. I'll share a closure summary with costs to date by Friday. Is there anything you'd like me to prioritize in the handover?"

### Case 15: A project that has met its goals and requires formal closure

| Element | Detail |
|---|---|
| Situation | Week 12: the BrightCuts app is live and UAT passed. The team is already thinking about other work. Maria says "We're done, thanks." |
| Main problem | Without formal closure, acceptance, handover, financial close-out, lessons, and benefit tracking would be lost |
| Root cause | Success creates a feeling of completion, so formal steps feel unnecessary |
| Options | (a) Informal thanks and move on, (b) close formally with the checklist |
| Recommended | (b), kept lightweight (about one week of effort, planned in the schedule) |
| Step-by-step resolution | 1) Run the acceptance verification table and get Maria's signed acceptance. 2) Resolve or reassign open items (D-18, risk on API changes). 3) Reconcile costs: $30,400 against a revised budget of $30,500. 4) Close contracts (designer, QA contractor), move hosting and the payment provider to Maria's accounts. 5) Hand over code, credentials, guides, and support arrangements. 6) Release the team with feedback to their managers. 7) Hold the lessons session and complete the register. 8) Archive documents. 9) Schedule 30- and 90-day benefit reviews. 10) Issue the closure report and thank the team. |
| Relevant documentation | Acceptance verification, sign-off, closure checklist, handover plan, lessons-learned register, closure report |
| Stakeholder communication | Closure announcement and team recognition (samples above) |
| Expected outcome | Documented proof of delivery, clear ownership, a team that feels recognized, and a plan to measure the business results |
| Lessons | Success still needs closure. The benefits are only proven when someone measures them |
| Possible exam question | "The project has met its goals and the sponsor is happy. What is the PM's next step?" Answer: obtain formal acceptance and complete the closure activities (handover, contracts, lessons learned, archive, report) |

---

## Part 7 Checkpoint Quiz

Try these **without looking back**:

1. List five closure activities in a sensible order.
2. A project finished with CPI = 1.00 and SPI = 1.00 but costs more than the original baseline. How can that be, and how should you report it?
3. What is the difference between an output and an outcome? Give a BrightCuts example of each.
4. A sponsor cancels a project halfway through. List four closure actions you would still take.
5. Name three items in a handover plan.
6. Why should a lessons-learned session avoid blame, and what should it produce?
7. What is the difference between validating scope and controlling quality?
