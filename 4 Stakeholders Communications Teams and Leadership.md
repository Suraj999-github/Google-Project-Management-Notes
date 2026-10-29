# Part 4: Stakeholders, Communications, Teams, and Leadership

**Source note:** As publicly described, Google's courses cover communication planning in *Project Planning*, and team leadership, conflict resolution, and stakeholder management mainly in *Project Execution* and the *Foundations* course. I haven't re-checked Coursera live, so confirm the current contents there. **[Supplemental]** marks my additions (Tuckman stages, role comparisons, negotiation frameworks). Templates, dialogues, and questions are my original material, not official Google content.

Stakeholder analysis (Skill 4) was covered in Part 2. This part builds on it with Skills 7, 13, and 14.

---

## 1. Learning Objectives

By the end of Part 4 you should be able to:
- Build a communication plan and tailor messages to different audiences
- Build, motivate, and delegate to a team
- Resolve conflicts and give constructive feedback
- Facilitate effective meetings, including remote ones
- Negotiate priorities, handle resistance, and escalate appropriately
- Explain how a project manager differs from a product manager, Scrum Master, technical lead, and people manager

**Running example:** BrightCuts Online Booking App. Team: you (PM), Dev (developer), Priya (UI designer), Sam (QA contractor). Sponsor: Maria Lopez. Receptionist: Tom.

---

## 2. How the Pieces Connect

```
Stakeholder register → Communication plan → Status reports, meetings
          ↓                                        ↓
   Engagement strategy                  Team alignment and decisions
          ↓                                        ↓
   Trust and support  ←──  Leadership + team management
```

The stakeholder register says *who* needs *what*. The communication plan turns that into a schedule of messages. Leadership and team management determine whether the people doing the work stay aligned and motivated. A communication breakdown often shows up first as a team conflict or a surprised sponsor.

---

## 3. Skill 7: Stakeholder Communications

**Definition:** Planning, creating, delivering, and checking the information exchange between the project and its stakeholders so the right people get the right information at the right time in a form they can use.

**Why it matters:** Most project managers spend a large share of their time communicating. Poor communication is a frequent root cause of missed expectations, duplicated work, and late surprises.

**When to use:** Plan it in the Planning phase, then run and adjust it throughout.

### Communication basics

| Concept | Meaning |
|---|---|
| **Sender, message, receiver, feedback** | Communication is only complete when the receiver understands. Check understanding. |
| **Push** | You send it (email, report) |
| **Pull** | They retrieve it (shared dashboard, wiki) |
| **Interactive** | Two-way (meetings, calls) |
| **Synchronous / asynchronous** | Real time (call) vs. delayed (email, chat) |
| **Formal / informal** | Documented (status report) vs. casual (hallway check-in) |

**Channels:** use a call or meeting for sensitive, complex, or emotional topics. Use writing for decisions, commitments, and anything that needs a record.

**Step-by-step process**
1. Start from the **stakeholder register**.
2. For each group, decide **what** they need, **how often**, **by what channel**, and **who** sends it.
3. Choose the right **level of detail** (executives: outcomes and decisions; team: tasks and blockers).
4. Write the **communication plan** and get it agreed.
5. **Deliver**, then **ask for feedback**.
6. **Review** monthly and after major changes.

### Template: Communication Plan (completed)

| Audience | Information | Frequency | Channel | Owner | Purpose |
|---|---|---|---|---|---|
| Maria (Sponsor) | Status report: progress, risks, decisions needed | Weekly (1 page) + monthly review call | Email + 30-min call | PM | Keep informed, get decisions |
| Project team | Tasks, blockers, priorities | Daily 15-min stand-up | Video call | PM | Coordinate work |
| Tom (Receptionist) and stylists | Demo, changes affecting daily work | Every 2 weeks | In-person demo | PM | Gather feedback, prepare for adoption |
| Customers (sample) | Short usability survey | Once, in UAT | Online form | PM | Validate usability |
| Payment provider | Delivery dates, API questions | Weekly until delivered | Email to account manager | Dev | Track dependency |
| Change requests | Impact summary and decision | As needed | Email + change log | PM | Controlled decisions |

**Rule of thumb:** if a stakeholder is surprised by news, the plan failed. Surprises should come from the world, not from the project.

### Writing for your audience

| Audience | Lead with | Avoid |
|---|---|---|
| Executive / sponsor | Status, forecast, the decision needed | Technical detail, long history |
| Customer / client | Benefits, dates, what you need from them | Internal jargon |
| Team | What, who, by when, why | Vague instructions |
| Technical stakeholders | Specifics, dependencies | Over-simplified claims |

**Good message structure:** *Bottom line first, then context, then options, then the ask.*

### Sample Messages

**Weekly status email to the sponsor**
> **Subject:** BrightCuts App, Week 6 Status: Amber
> **Summary:** We are one week behind on the critical path (booking flow). Launch is still achievable with a scope adjustment.
> **Done:** Requirements and design approved; admin dashboard 60% complete.
> **Next:** Booking flow completion; start system testing on finished modules.
> **Risks:** Payment API delay (High). Mock API in place.
> **Decision needed by Friday:** Defer SMS reminders to phase 2 (saves ~$2,000 and 3 days), or move launch by one week?

**Escalation message**
> Maria, I need your help with one item. The payment provider has not delivered the sandbox access promised for week 4. This puts our launch date at risk. I've emailed their account manager twice. Could you contact the provider's owner this week? Without access by next Wednesday, we'll use the mock API and plan a 2-day delay.

### Common challenges and solutions

| Challenge | Solution |
|---|---|
| Too many emails, nobody reads them | Short, structured updates; one place for status |
| Conflicting messages to different groups | One source of truth; PM approves outward messages |
| Information overload for executives | One page, top 3 risks, decisions highlighted |
| Remote team misses context | Written notes after every meeting; shared decision log |
| Different time zones | Rotate meeting times; rely on async updates |

**Relationships:** The communication plan is driven by the **stakeholder register**, delivers **risk** and **change** information, and is checked during **quality** reviews. Poor communication is a root cause of **scope** disputes and **conflict**.

---

## 4. Skill 13: Team Management

**Definition:** Organizing, coordinating, and supporting the people doing the work so tasks are assigned clearly, workloads are sustainable, and performance is tracked and improved.

**Why it matters:** Plans don't deliver themselves. People do, and misaligned or overloaded teams produce rework and burnout.

### Building a team: Tuckman's stages **[Supplemental]**

| Stage | What you see | Your action |
|---|---|---|
| **Forming** | Polite, unsure of roles | Clarify goals, roles, ways of working |
| **Storming** | Disagreements, friction | Facilitate, don't suppress. Agree on decision rules |
| **Norming** | Cooperation, shared norms | Reinforce good habits |
| **Performing** | Efficient, self-driven | Remove obstacles, delegate more |
| **Adjourning** | Project ending | Recognize contributions, capture lessons |

Storming is normal and not a sign you failed.

### Team management process
1. **Set up:** kickoff meeting, shared goals, roles (RACI), team agreements (working hours, how to raise problems, definition of done).
2. **Assign work** based on skills, availability, and development goals.
3. **Delegate** (see below).
4. **Track** progress and workload (stand-ups, task board).
5. **Support:** remove blockers, provide tools and training.
6. **Give feedback** regularly.
7. **Recognize** good work.
8. **Resolve** problems early.

### Delegating well

| Step | Example |
|---|---|
| Choose the right person | Dev has payment API experience |
| Explain the **outcome** and why it matters | "Customers must be able to pay at booking" |
| Define constraints and success criteria | "Done = card payment works in test, under $400 in fees, by Friday week 7" |
| Agree on checkpoints | "Show me the sandbox test on Tuesday" |
| Give authority and resources | Access to sandbox, decision rights on library choice |
| Follow up, don't micromanage | Ask for progress, offer help |

**Delegating is not dumping.** You stay accountable for the result.

### Motivating a team
- Give **purpose** (connect tasks to business value).
- Give **autonomy** (let people choose *how*).
- Support **growth** (stretch assignments, learning time).
- Recognize **specific** contributions, publicly when appropriate.
- Protect people from **overload** and constant context-switching.
- Different people are motivated differently, so ask them.

### Template: Team Agreement (completed)
| Topic | Agreement |
|---|---|
| Working hours | Core hours 10:00 to 15:00 for overlap |
| Communication | Urgent: call. Questions: team chat. Decisions: written in decision log |
| Raising problems | Raise blockers the same day, no blame |
| Meetings | Agenda in advance, notes within 24 hours |
| Done means | Reviewed, tested, merged, documented |

### Conflict resolution

Conflict is normal. Unmanaged conflict hurts a project, while well-managed disagreement can improve decisions.

| Approach | Meaning | Best when |
|---|---|---|
| **Collaborate / problem-solve** | Work to a solution that meets both needs | Important issue, time available |
| **Compromise** | Each gives something up | Time is short, moderate stakes |
| **Accommodate** | Give way | Issue matters more to the other party |
| **Compete / force** | One side wins | Emergencies, safety, unpopular but necessary decisions |
| **Avoid / withdraw** | Postpone | Cooling-off needed, or trivial issue |

*(These are adapted from the Thomas-Kilmann conflict modes, a widely used framework. The names vary by source.)* **[Supplemental]**

**Process:**
1. Talk to each person **privately** first to understand their view.
2. Separate **facts** from interpretations, and **issues** from personalities.
3. Bring them together, focus on **shared goals**.
4. Agree on **specific actions**.
5. **Follow up**.
6. Escalate only if the people can't resolve it or if behavior breaches policy. Involve HR or the people manager for behavior concerns.

### Giving constructive feedback
Use a simple structure such as **SBI: Situation, Behavior, Impact**, then ask for their view and agree on a next step.

> "In yesterday's review (situation), the test report arrived after the demo started (behavior). That meant Maria saw unverified results and asked questions we couldn't answer (impact). What got in the way, and how can we make sure it's ready 30 minutes before the next demo?"

**Tips:** be timely, specific, private for corrective feedback, and balanced. Ask questions before concluding. Recognize good work with the same specificity.

### Handling a team member who is not meeting expectations
1. **Clarify expectations.** Were they clear and documented?
2. **Gather facts** (missed dates, quality issues).
3. **Meet privately**, ask open questions to find root causes (skills gap, unclear task, overload, personal issues, motivation).
4. **Agree a plan:** support, training, clearer tasks, checkpoints, timeline.
5. **Follow up** and document.
6. **Involve the people manager** if no improvement. As PM you may not have formal authority over performance reviews.

### Facilitating meetings

| Before | During | After |
|---|---|---|
| Clear purpose, agenda, invite only needed people | Start on time, assign note-taker, timebox, keep to agenda, draw out quiet voices, park off-topic items | Send notes with **decisions, actions, owners, dates** within 24 hours |

**Test for a meeting:** can this be an email or a shared doc? If yes, skip the meeting.

### Remote and cross-functional teams
- Over-communicate in writing; document decisions.
- Define overlap hours and response expectations.
- Use video for relationship-building and sensitive topics.
- Don't assume silence means agreement. Ask directly.
- Include remote people first in discussions.
- With cross-functional teams (design, engineering, QA, business), agree on a **shared goal and vocabulary**, since each function has different priorities and terms.

**Relationships:** Team management uses the **RACI**, **schedule**, and **communication plan**. It supports **quality** (clear definitions of done), and **risk** (single points of failure, overload).

---

## 5. Skill 14: Team Leadership

**Definition:** Guiding and influencing people toward a shared goal, setting direction, building trust, and helping the team make good decisions, especially when you don't control their careers.

**Management vs. leadership:** Management handles *how* (plans, tracking, process). Leadership handles *where and why* (vision, motivation, influence). Project managers need both.

**Why it matters:** Many project managers lead without formal authority. Influence, trust, and clarity do the work that a title cannot.

### Core leadership behaviors

| Behavior | In practice |
|---|---|
| **Set direction** | Explain the goal and why it matters, repeatedly |
| **Build trust** | Keep promises, admit mistakes, give credit |
| **Empower** | Delegate decisions to those with the best information |
| **Serve** | Remove blockers, shield from noise |
| **Communicate honestly** | Share bad news early with a plan |
| **Adapt** | Vary your style to the person and situation |
| **Model** | Show the behavior you expect (punctuality, respect, accountability) |

**Situational leadership [Supplemental]:** Match your style to the person's skill and motivation. A new, enthusiastic team member needs clear direction. An experienced, capable one needs autonomy and recognition. A skilled but demotivated one needs listening and encouragement.

### Making decisions with incomplete information
1. Decide **what must be decided now** and what can wait.
2. Gather the **most important facts quickly** (timebox it).
3. List **options** and what you'd lose if you're wrong.
4. Prefer **reversible** decisions made quickly. Slow down for irreversible ones.
5. State your **assumptions** and the trigger for revisiting.
6. **Decide, communicate, and review.**

> "We don't know if the vendor will deliver by week 4. I'm deciding to build the mock now, because it costs two days and protects the launch. If the sandbox arrives, we switch with little loss."

### Negotiating priorities
1. Understand each party's **interests** (needs), not just **positions** (demands).
2. Share the **facts** (impact on schedule, cost).
3. Offer **options** with trade-offs.
4. Look for **win-win** (phasing, partial delivery).
5. Agree and **document**.

> **Maria:** "I need the loyalty feature before launch."
> **PM:** "Tell me more about what you want it to achieve."
> **Maria:** "I want repeat customers."
> **PM:** "That's a great goal. Building loyalty points adds about three weeks and $4,500. Another option is a first-booking discount, which takes two days and also encourages return visits. We could add full loyalty in phase 2 once we see usage. Which do you prefer?"

### Managing resistance to change
Resistance usually has a reason: fear of losing control, extra work, unclear benefits, past bad experiences.

1. **Listen** to understand the concern.
2. **Explain** the why and what's in it for them.
3. **Involve** them in design and testing.
4. **Train and support.**
5. **Show early wins**, and use champions.
6. **Follow up** after launch.

(Formal change management for organizational change, including frameworks like ADKAR, appears in Part 5.) **[Supplemental]**

### Dealing with difficult stakeholders

| Situation | Approach |
|---|---|
| Demanding and constantly changing requests | Quantify the cost of changes; batch changes; weekly decision meeting |
| Silent / unresponsive | Offer shorter, specific asks; find out preferred channel; ask the sponsor for support |
| Hostile | Stay calm, listen, acknowledge the concern, focus on facts, take it offline |
| Overly technical | Translate to outcomes, bring a technical lead |
| Skeptical senior stakeholder | Show evidence, small proof, and regular updates |

### Communicating with executives vs. customers

| | Executive | Customer |
|---|---|---|
| Wants | Outcomes, risks, decisions, money | Value, usability, dates |
| Format | One page, headline first | Demos, plain language |
| Tone | Concise, confident, honest | Collaborative, reassuring |

### Escalating appropriately
Escalate when: a problem is **beyond your authority** or the team's ability, it threatens the **baseline** (scope, schedule, cost, quality), or the people involved can't agree.

**How to escalate:**
1. Try to resolve at the lowest level first (unless there's urgent risk).
2. State **facts**, impact, what you've tried, and the **specific help** needed.
3. Offer a **recommendation**.
4. Escalate **early**, not at the last moment.
5. Stay professional and don't blame.

Escalation is not failure. Hiding problems is.

### Dialogue Example: addressing missed deadlines

> **PM:** "Dev, I wanted to check in. The booking flow task was due Tuesday and is still open. I'd like to understand what's happening."
> **Dev:** "Honestly, the payment rules are more complicated than I expected, and I've been pulled into support questions too."
> **PM:** "Thanks for telling me. What would help most: clearer rules, fewer interruptions, or more time?"
> **Dev:** "Fewer interruptions, and a decision on partial payments."
> **PM:** "I'll block support questions to me until Friday, and I'll get Maria's decision on partial payments by tomorrow. Can we check in again Thursday?"

### Dialogue Example: resolving a conflict between team members

> **PM** (to Priya and Dev separately, then together): "I've heard both views. Priya, you need designs approved before development changes them. Dev, you need freedom to adjust things that aren't feasible. Do we agree the goal is a design that works and is built once?"
> **Both:** "Yes."
> **PM:** "Then let's agree: Dev flags feasibility issues within one day of receiving a design. Priya updates the design or explains why not. Maria arbitrates if you can't agree in two days. Does that work?"

### Role Comparison [Supplemental]

| Role | Main focus | Typical responsibility | Typical authority |
|---|---|---|---|
| **Project manager** | Delivering a defined project on time, cost, scope, quality | Plan, track, risk, communication, change control | Varies; often influence-based |
| **Product manager** | The product's value and strategy over time | What to build and why; roadmap; customer needs | Product vision and priorities |
| **Scrum Master** | Scrum process and team effectiveness | Coach the team, facilitate events, remove impediments | Authority over the process, not the people or content |
| **Product Owner (Scrum)** | Maximizing product value | Own and order the product backlog | Backlog decisions |
| **Technical lead** | Technical quality and design | Architecture, code standards, mentoring on technical matters | Technical decisions |
| **People manager** | Individuals' performance and growth | Reviews, hiring, career development, welfare | Formal authority over team members |

**Notes:** Titles and duties vary by company. In Agile teams, there may be no dedicated project manager, and some of the project manager's duties are shared among the Product Owner, Scrum Master, and team. In small teams, one person may wear several hats.

---

## 6. Common Mistakes

| Mistake | How to avoid |
|---|---|
| Communicating only when there's bad news (or only good news) | Regular rhythm, honest status |
| One-size-fits-all messages | Tailor to audience |
| Avoiding conflict | Address early, in private |
| Public criticism | Give corrective feedback privately |
| Micromanaging | Agree on outcomes and checkpoints |
| Hero PM doing everyone's work | Delegate and trust |
| Assuming silence means agreement | Ask directly |
| Escalating too late, or with no recommendation | Escalate early with facts and a proposal |
| Ignoring workload | Check capacity weekly |

---

## 7. Module Summary and Revision Notes

- The communication plan answers: who, what, how often, which channel, who sends.
- Lead with the bottom line and any decision needed.
- Tuckman: forming, storming, norming, performing, adjourning. Storming is normal.
- Delegate outcomes with clear criteria and checkpoints. You remain accountable.
- Conflict: talk privately first, focus on interests and facts, agree actions, escalate when needed.
- SBI feedback: Situation, Behavior, Impact.
- Negotiate interests, not positions; offer options with trade-offs.
- Escalate early, with facts, what you tried, and a recommendation.
- PM, product manager, Scrum Master, tech lead, and people manager have different focuses.

---

## 8. Skill-by-Skill Question Sets

*Brief explanations are included. The full 10-field format appears in the numbered bank in Part 8.*

### Skill 7: Stakeholder Communications

**Beginner**
1. **What is a communication plan?** A document that sets out who gets what information, how often, by which channel, and from whom.
2. **What source document do you use to build it?** The stakeholder register.
3. **Push vs. pull communication?** Push is sent to the audience (email). Pull is retrieved by them (a shared dashboard).
4. **True or false: communication is complete once the message is sent.** False. It's complete when the receiver understands.
5. **Which channel suits a sensitive conversation?** A live conversation (call or in person).

**Intermediate**
1. **How should you write an update for an executive?** Short, outcome-focused, with the decision needed first.
2. **Why document decisions in writing?** To avoid disputes and ensure shared understanding.
3. **What should meeting notes include?** Decisions, action items, owners, and dates.
4. **Why review the communication plan regularly?** Stakeholders, risks, and the project change.
5. **Formal vs. informal communication?** Formal is documented and official. Informal is casual and builds relationships. Both are needed.

**Scenario**
1. **Maria says she wasn't told about a delay.** Check the plan: was she on the distribution? Apologize for the gap, share the facts, adjust frequency, and confirm what she wants. *Reasoning:* fix the process, not just the symptom.
2. **Remote team members miss decisions made in a hallway chat.** Record all decisions in a shared log and send summaries. *Reasoning:* decisions that aren't written aren't shared.
3. **A stakeholder replies "OK" but then objects later.** Confirm understanding explicitly ("To confirm, you approve X by Friday?") and follow up in writing.
4. **A rumor spreads that the project is cancelled.** Respond quickly with a clear factual message from the PM or sponsor, then increase update frequency.
5. **The team receives conflicting instructions from two managers.** Clarify priorities with both managers together and document the agreed direction.

**Interview**
1. **How do you plan communication on a project?** *Sample:* "I begin with the stakeholder register, decide what each group needs and how often, choose the channel, and agree on it in a communication plan. I review it monthly."
2. **Tell me about a communication problem you fixed.** *Sample (STAR):* "A sponsor felt uninformed. I asked what format she preferred, switched to a one-page weekly status with a decision section, and her confidence improved."
3. **How do you communicate bad news?** "Early, factually, with the impact, the options, and my recommendation."
4. **How do you tailor communication for executives vs. engineers?** "Executives get outcomes, risks, and decisions. Engineers get specifics, dependencies, and context."
5. **How do you keep a remote team aligned?** "Written decisions, a shared task board, short stand-ups, and clear overlap hours."

### Skill 13: Team Management

**Beginner**
1. **What are Tuckman's five stages?** Forming, storming, norming, performing, adjourning.
2. **What is delegation?** Assigning responsibility for a task or outcome to someone else while remaining accountable for the overall result.
3. **What does SBI stand for?** Situation, Behavior, Impact.
4. **What should a kickoff meeting do?** Align on goals, roles, and ways of working.
5. **True or false: conflict is always bad.** False. Managed disagreement can improve decisions.

**Intermediate**
1. **Why is storming normal?** People are testing roles and working styles, so friction is expected.
2. **Name three conflict-handling approaches.** Collaborate, compromise, accommodate, compete, avoid (any three).
3. **When is "compete/force" appropriate?** In emergencies or when a quick unpopular decision is essential.
4. **What is a team agreement?** A short set of working rules the team defines together.
5. **Why delegate outcomes rather than steps?** It encourages ownership and uses people's expertise.

**Scenario**
1. **A team member is consistently late with tasks.** Meet privately, find the root cause, agree on a plan with checkpoints, and escalate to their manager if it doesn't improve. *Reasoning:* understand before judging.
2. **Two members disagree on the technical approach.** Hear both, focus on goals and criteria, involve the technical lead, and decide with documented reasons.
3. **A key developer is overloaded.** Review workloads, reprioritize, move non-critical work, and consider help. *Reasoning:* overload hurts quality and retention.
4. **A high performer is dominating meetings.** Use facilitation (round-robin, ask quiet people first) and give private feedback.
5. **Morale is low after a schedule crunch.** Acknowledge the effort, reduce pressure where possible, recognize contributions, and discuss lessons.

**Interview**
1. **How do you motivate a team?** *Sample:* "I link work to purpose, give autonomy, recognize specific contributions, and protect people from overload. I ask each person what motivates them."
2. **Tell me about a team conflict you resolved.** *Sample (STAR):* "Two engineers disagreed on architecture. I met them separately, then together, we agreed decision criteria, and the tech lead made the call. The project stayed on schedule and the working relationship recovered."
3. **How do you handle underperformance?** "I clarify expectations, find the cause, agree a support plan, follow up, and involve their manager if needed."
4. **How do you delegate?** "I explain the outcome and why it matters, set criteria and checkpoints, give authority and resources, then follow up without micromanaging."
5. **How do you run an effective meeting?** "Clear purpose, agenda, right attendees, timeboxing, and notes with owners and dates after."

### Skill 14: Team Leadership

**Beginner**
1. **Management vs. leadership?** Management handles how (planning, tracking). Leadership handles direction and influence.
2. **What does a servant leader do?** Removes obstacles and supports the team's work.
3. **Why is trust important?** People share problems and take ownership when they trust the leader.
4. **When should you escalate?** When an issue exceeds your authority, threatens the baseline, or can't be resolved at the team level.
5. **True or false: a PM always has formal authority over team members.** False. Often influence-based.

**Intermediate**
1. **Interests vs. positions in negotiation?** Positions are what people demand. Interests are why they want it. Solutions come from interests.
2. **How do you decide with incomplete information?** Timebox research, weigh reversibility, state assumptions, decide, and review.
3. **Why do people resist change?** Fear of loss of control, extra work, unclear benefit, past experience.
4. **What makes an escalation effective?** Facts, impact, what's been tried, specific ask, and a recommendation.
5. **How does a Scrum Master differ from a PM?** A Scrum Master focuses on Scrum process and team effectiveness, while a PM is accountable for delivering the project plan, though duties vary by organization.

**Scenario**
1. **A senior stakeholder publicly criticizes the project.** Stay calm, acknowledge the concern, then meet privately to understand and address it. *Reasoning:* de-escalate in public and resolve in private.
2. **The sponsor and a team lead give opposing priorities.** Bring both together, show the trade-offs, and ask the sponsor (higher authority) to decide and document.
3. **You must decide today but lack data.** Choose a reversible option, state assumptions, and set a review point.
4. **Tom the receptionist says the new app will "make my job harder".** Ask what worries him, involve him in design and testing, and provide training.
5. **A deadline can't be met.** Tell the sponsor early with options and a recommendation.

**Interview**
1. **How do you lead without authority?** *Sample:* "I build trust, make goals clear, connect work to what each person cares about, and use data and shared decisions rather than orders."
2. **Describe a time you managed resistance to change.** *Sample (STAR):* "Staff resisted a new tool. I listened, involved them in testing, adjusted the workflow, and trained them. Adoption reached 85% in a month."
3. **How do you handle a difficult stakeholder?** "I listen for the underlying concern, share facts, offer options, and keep communication frequent and written."
4. **When do you escalate?** "When the issue is beyond my authority or threatens the baseline, and early, with a recommendation."
5. **How is a PM different from a Scrum Master?** "The Scrum Master facilitates the Scrum process and team effectiveness. A PM manages the overall plan, risk, stakeholders, and delivery. In many Agile teams, these responsibilities are shared."

### Revision Checklist
- [ ] I can build a communication plan from a stakeholder register
- [ ] I can write a one-page status update
- [ ] I can recall Tuckman's stages and conflict approaches
- [ ] I can give SBI feedback and delegate outcomes
- [ ] I can negotiate using interests and trade-offs
- [ ] I can explain when and how to escalate
- [ ] I can distinguish PM, product manager, Scrum Master, tech lead, and people manager

---

## 9. Case Studies (3 more of the 15)

### Case 5: A team member who is not meeting expectations

| Element | Detail |
|---|---|
| Situation | Sam (QA contractor) has missed two test-report deadlines, and one report had errors. |
| Main problem | Testing is on the critical path (system testing, week 8 to 10). |
| Root cause | Unclear test scope and a second client taking his time (found in conversation) |
| Options | (a) Replace Sam, (b) clarify and support, (c) share the testing among the team |
| Recommended | (b), with a short checkpoint cycle. Keep (a) as contingency |
| Resolution steps | Meet privately, ask open questions, agree a test plan and priorities, set 2-day checkpoints, review in one week, raise with the contract owner if no improvement |
| Documentation | Test plan, task assignments, notes of the conversation |
| Communication | Sam: supportive and specific. Maria: heads-up on the risk to testing and mitigation |
| Outcome | Reports arrive on time after scope is clarified; quality improves |
| Lessons | Underperformance is often a clarity or capacity problem first |
| Possible exam question | "What should the PM do first when a team member misses deadlines?" Answer: meet privately to understand the cause |

### Case 6: A conflict between two team members

| Element | Detail |
|---|---|
| Situation | Priya (designer) and Dev argue about changes to approved screens. |
| Main problem | Rework, tension, slowed handoffs |
| Root cause | No agreed process for feasibility feedback and design changes |
| Options | Ignore, impose a winner, or facilitate a process agreement |
| Recommended | Facilitate: separate conversations, then a joint session to agree the process |
| Resolution steps | Listen separately, restate shared goals, agree: Dev flags issues within 1 day, Priya responds within 1 day, sponsor arbitrates after 2 days, record in team agreement |
| Documentation | Updated team agreement; design change log |
| Communication | Brief note to the team on the new process (no blame) |
| Outcome | Fewer reworks; handoffs speed up |
| Lessons | Fix the process, not just the people |
| Possible exam question | "Two team members disagree. What do you do first?" Answer: speak to each privately to understand their views |

### Case 13: A communication breakdown between stakeholders

| Element | Detail |
|---|---|
| Situation | Stylists believe the app will let customers pick any stylist at any time. Maria planned "first available" only. A week before UAT, stylists are upset. |
| Main problem | Mismatched expectations about a key feature |
| Root cause | Stylists were "informed" but never "consulted". Requirements were gathered only from Maria |
| Options | Change scope, explain and hold, or phase the feature |
| Recommended | Meet both groups, clarify the business rule, estimate the effort for stylist selection, and decide through change control |
| Resolution steps | Joint workshop, document requirements, impact estimate (+3 days), Maria approves a simplified version, update scope, schedule, and user stories |
| Documentation | Updated stakeholder register and RACI (stylists to Consulted), change log, communication plan |
| Communication | Acknowledge the gap, explain the decision and reason, confirm in writing |
| Outcome | Stylists feel heard; UAT goes ahead with aligned expectations |
| Lessons | Consult affected users early, and confirm understanding in writing |
| Possible exam question | "Which document helps prevent stakeholders being left out of decisions?" Answer: stakeholder register and RACI |

---

## Part 4 Checkpoint Quiz

Try these **without looking back**:

1. What does a communication plan contain, and which document do you build it from?
2. A team is arguing heavily in the second week. Which Tuckman stage is likely, and what should you do?
3. Write one SBI sentence about a missed deadline.
4. The sponsor demands a feature that would delay launch by three weeks. Describe how you would negotiate.
5. When should you escalate, and what should an escalation include?
6. Name one difference between a project manager and a Scrum Master.
