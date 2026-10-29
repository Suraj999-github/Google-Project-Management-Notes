
### Task A (2 days) starts first. B (3 days) and C (6 days) follow A. D (4 days) follows B. E (2 days) follows C. F (3 days) follows both D and E. What is the project duration, and what is the slack on B?

- A. 12 days; slack 0
- B. 13 days; slack 1
- C. 13 days; slack 3
- D. 16 days; slack 1

Correct answer: C. 13 days; slack 3 days — but let's calculate to verify.

### Step 1: Forward pass (earliest times)

- A: $0 \to 2$
- B: $2 \to 5$
- C: $2 \to 8$
- D: $5 \to 9$
- E: $8 \to 10$
- F: starts after both D and E, so $\max(9,10)=10$, finishes at $13$.

Project duration = 13 days.

### Step 2: Backward pass (latest times)

Working backward from project completion at day 13:

- F: latest start = 10
- D: latest finish = 10, latest start = 6
- E: latest finish = 10, latest start = 8
- B: latest finish = 6, latest start = 3

### Step 3: Calculate slack on B

$$
\text{Slack}=\text{Latest Start}-\text{Earliest Start}
$$

$$
=3-2=\boxed{1\text{ day}}
$$

Correct answer: B. 13 days; slack 1.

The critical path is A → C → E → F, with a total duration of $2+6+2+3=13$ days.

---
### Estimating (PERT) | Intermediate | Numerical 
### A task has O = 3, M = 6, P = 15 days. What are the PERT estimate and standard deviation?
- A. 6 days; SD 2
- B. 7 days; SD 2
- C. 8 days; SD 4
- D. 7 days; SD 4

Correct answer: B. 7 days; SD 2

### 1. Calculate the PERT estimate

$$
TE=\frac{O+4M+P}{6}
$$

Substitute $O=3,\ M=6,\ P=15$:

$$
TE=\frac{3+4(6)+15}{6}
=\frac{42}{6}=\boxed{7\text{ days}}
$$

### 2. Calculate the standard deviation

$$
SD=\frac{P-O}{6}
$$

$$
SD=\frac{15-3}{6}=\boxed{2\text{ days}}
$$

Final answer: B. 7 days; SD 2.

Exam tip: Remember that PERT uses the weighted average $(O+4M+P)/6$, while standard deviation is $(P-O)/6$.

---

### Slack | Intermediate | Numerical 
### A task has duration 4 days, earliest start day 6, and latest finish day 14. What is its slack?
- A. 0 days
- B. 2 days
- C. 4 days
- D. 8 days

Correct answer: C. 4 days

### Step 1: Calculate the earliest finish (EF)

$$
EF=ES+\text{Duration}=6+4=10
$$

### Step 2: Calculate the latest start (LS)

$$
LS=LF-\text{Duration}=14-4=10
$$

### Step 3: Calculate slack

$$
\text{Slack}=LS-ES=10-6=\boxed{4\text{ days}}
$$

Final answer: C. 4 days.

Exam tip: Slack = Latest Start − Earliest Start, or equivalently, Latest Finish − Earliest Finish.

---

### Estimating (parametric) | Intermediate | Numerical 
Past projects show one report takes 4 hours to build. The new project needs 25 reports, and labor costs $60 per hour. Using parametric estimating, what is the cost?
- A. $1,500
- B. $4,000
- C. $6,000
- D. $10,000

Correct answer: C. $6,000

### Step 1: Calculate total labor hours

$$
\text{Total hours}=25 \times 4=100\text{ hours}
$$

### Step 2: Calculate total cost

$$
\text{Cost}=100 \times \$60=\boxed{\$6,000}
$$

Final answer: C. $6,000.

Exam tip: Parametric estimating uses a historical rate per unit multiplied by the number of units required.

$$
\text{Cost}=\text{Quantity}\times\text{Hours per unit}\times\text{Cost per hour}
$$

---

### Earned Value | Intermediate | Numerical
### BAC = $100,000, PV = $40,000, EV = $35,000, AC = $38,000. What are CV and SV?
- A. CV −$3,000; SV −$5,000
- B. CV +$3,000; SV +$5,000
- C. CV −$5,000; SV −$3,000
- D. CV −$3,000; SV +$5,000

Correct answer: A. CV −$3,000; SV −$5,000

### Step 1: Calculate Cost Variance (CV)

$$
CV=EV-AC
$$

$$
CV=35{,}000-38{,}000=\boxed{-\$3{,}000}
$$

A negative CV means the project is over budget.

### Step 2: Calculate Schedule Variance (SV)

$$
SV=EV-PV
$$

$$
SV=35{,}000-40{,}000=\boxed{-\$5{,}000}
$$

A negative SV means the project is behind schedule.

### Final answer: A

Exam tip:

- CV = EV − AC (cost performance)
- SV = EV − PV (schedule performance)
- Negative variance = unfavorable; positive variance = favorable.

---

### Earned Value | Intermediate | Numerical 
### PV = $54,000, EV = $45,000, AC = $50,000. What are CPI and SPI (rounded to 2 decimals)?
- A. CPI 0.90; SPI 0.83
- B. CPI 1.11; SPI 1.20
- C. CPI 0.83; SPI 0.90
- D. CPI 0.90; SPI 1.20

Correct answer: A. CPI 0.90; SPI 0.83

### Step 1: Calculate Cost Performance Index (CPI)

$$
CPI=\frac{EV}{AC}
$$

$$
CPI=\frac{45{,}000}{50{,}000}=\boxed{0.90}
$$

A CPI below 1.00 means the project is over budget.

### Step 2: Calculate Schedule Performance Index (SPI)

$$
SPI=\frac{EV}{PV}
$$

$$
SPI=\frac{45{,}000}{54{,}000}=0.8333\ldots
$$

Rounded to two decimal places:

$$
SPI=\boxed{0.83}
$$

An SPI below 1.00 means the project is behind schedule.

Final answer: A. CPI 0.90; SPI 0.83.

Exam tip:

- CPI = EV ÷ AC
- SPI = EV ÷ PV
- Index below 1 = unfavorable; above 1 = favorable.

---

### Forecasting | Advanced | Numerical 
BAC = $90,000 and CPI = 0.75. Assuming current cost performance continues, what are EAC and the variance at completion (VAC = BAC − EAC)?
- A. EAC $120,000; VAC −$30,000
- B. EAC $67,500; VAC +$22,500
- C. EAC $120,000; VAC +$30,000
- D. EAC $90,000; VAC $0

Correct answer: A. EAC $120,000; VAC −$30,000

### Step 1: Calculate Estimate at Completion (EAC)

Since current cost performance is expected to continue:

$$
EAC=\frac{BAC}{CPI}
$$

Substitute the values:

$$
EAC=\frac{\$90{,}000}{0.75}
=\boxed{\$120{,}000}
$$

### Step 2: Calculate Variance at Completion (VAC)

$$
VAC=BAC-EAC
$$

$$
VAC=\$90{,}000-\$120{,}000
=\boxed{-\$30{,}000}
$$

### Final answer: A

The project is forecast to cost $30,000 more than its original budget.

Exam tip:

- $CPI<1$: over budget.
- $EAC>BAC$: expected cost overrun.
- $VAC<0$: unfavorable budget outcome.

---

### Forecasting | Advanced | Numerical 

 BAC = $60,000, EV = $20,000, AC = $25,000. The overrun was a one-off event, and the remaining work will follow the original plan. What are EAC and ETC?

- A. EAC $65,000; ETC $40,000
- B. EAC $75,000; ETC $50,000
- C. EAC $60,000; ETC $35,000
- D. EAC $65,000; ETC $65,000

Correct answer: A. EAC $65,000; ETC $40,000

### Step 1: Choose the correct forecasting formula

Since the overrun was a one-off event and the remaining work will follow the original plan, use:

$$
EAC=AC+(BAC-EV)
$$

### Step 2: Calculate EAC

$$
EAC=25{,}000+(60{,}000-20{,}000)
$$

$$
EAC=25{,}000+40{,}000=\boxed{\$65{,}000}
$$

### Step 3: Calculate Estimate to Complete (ETC)

$$
ETC=EAC-AC
$$

$$
ETC=65{,}000-25{,}000=\boxed{\$40{,}000}
$$

Final answer: A. EAC $65,000; ETC $40,000.

Exam tip: If a cost overrun is a one-off event, assume the remaining work follows the original budget. If current cost performance is expected to continue, use $EAC=BAC/CPI$ instead.

---

### Earned Value | Intermediate | Numerical 
 BAC = $80,000. The project is 25% complete, and AC = $22,000. What is CPI (rounded to 2 decimals)?

- A. 0.91
- B. 1.10
- C. 0.88
- D. 0.25

Correct answer: A. 0.91

### Step 1: Calculate Earned Value (EV)

$$
EV=BAC\times \%\text{ complete}
$$

$$
EV=80{,}000\times 0.25=\$20{,}000
$$

### Step 2: Calculate Cost Performance Index (CPI)

$$
CPI=\frac{EV}{AC}
$$

$$
CPI=\frac{20{,}000}{22{,}000}=0.9090\ldots
$$

Rounded to two decimal places:

$$
\boxed{CPI=0.91}
$$

Final answer: A. 0.91

Exam tip: CPI below 1.00 means the project is over budget. Here, the project earns about $0.91 of value for every $1 spent.

---

### EMV | Intermediate | Numerical 
Risk A: 30% chance of −$20,000. Opportunity B: 20% chance of +$10,000. What is the net EMV?
- A. −$8,000
- B. −$4,000
- C. −$6,000
- D. +$4,000

Correct answer: C. −$4,000

### Step 1: Calculate EMV for Risk A

$$
EMV_A=P\times \text{Impact}
$$

$$
EMV_A=0.30\times(-\$20{,}000)=-\$6{,}000
$$

### Step 2: Calculate EMV for Opportunity B

$$
EMV_B=0.20\times \$10{,}000=+\$2{,}000
$$

### Step 3: Calculate net EMV

$$
\text{Net EMV}=EMV_A+EMV_B
$$

$$
=-\$6{,}000+\$2{,}000
=\boxed{-\$4{,}000}
$$

Final answer: B. −$4,000.

Exam tip: Multiply each possible outcome by its probability, then add the results, keeping losses negative and gains positive.

---
### Communication channels | Intermediate | Numerical
Channels = n(n − 1) ÷ 2. A team grows from 7 people to 11 people. How many channels exist at 11, and how many were added?

- A. 55 channels; 34 added
- B. 55 channels; 4 added
- C. 110 channels; 89 added
- D. 21 channels; 34 added

Correct answer: A. 55 channels; 34 added

### Step 1: Calculate channels for 11 people

Formula:

$$
\text{Channels}=\frac{n(n-1)}{2}
$$

Substitute $n=11$:

$$
\frac{11(11-1)}{2}
=\frac{11\times10}{2}
=\boxed{55}
$$

### Step 2: Calculate channels for 7 people

$$
\frac{7(7-1)}{2}
=\frac{7\times6}{2}
=\boxed{21}
$$

### Step 3: Calculate channels added

$$
55-21=\boxed{34}
$$

Final answer: A. 55 channels; 34 added.

Exam tip: Communication channels increase rapidly as team size grows because every person can communicate with every other person. Always calculate both totals, then subtract to find the increase.

---
### Pareto | Intermediate | Numerical 
Defects by category: 45, 25, 15, 10, and 5 (100 total). How many of the largest categories are needed to account for at least 85% of defects?
- A. 2
- B. 3
- C. 4
- D. 5

Correct answer: B. 3

### Step 1: Add the largest categories cumulatively

| Category | Defects | Cumulative total | Cumulative % |
| --- | --- | --- | --- |
| 1st | 45 | 45 | 45% |
| 2nd | 25 | 70 | 70% |
| 3rd | 15 | 85 | 85% |
| 4th | 10 | 95 | 95% |
| 5th | 5 | 100 | 100% |

### Step 2: Identify the minimum number

The first two categories account for 70%. Adding the third raises the cumulative percentage to 85%.

Final answer: B. 3 categories.

Exam tip: In a Pareto analysis, rank categories from largest to smallest, then add their percentages cumulatively until you reach or exceed the target.

---

### Test metrics | Advanced | Numerical 
60 test cases were run and 54 passed. The target pass rate is 95%. What is the current pass rate, and how many more tests must pass?
- A. 90%; 3 more
- B. 90%; 6 more
- C. 95%; 0 more
- D. 85%; 3 more
Correct answer: A. 90%; 3 more

### Step 1: Calculate the current pass rate

$$
\text{Pass rate}=\frac{\text{Tests passed}}{\text{Tests run}}\times100
$$

$$
=\frac{54}{60}\times100=\boxed{90\%}
$$

### Step 2: Calculate how many additional tests must pass

Assuming the additional tests are added to the total number of tests, let $x$ be the number of additional tests, all of which pass.

$$
\frac{54+x}{60+x}\geq0.95
$$

$$
54+x\geq57+0.95x
$$

$$
0.05x\geq3
$$

$$
x\geq60
$$

So, 60 additional passing tests would be required if every new test increases the denominator.

However, the answer choices assume the original 60 tests remain the denominator. Under that interpretation, $95\%\times60=57$, so $57-54=3$ more passes are needed.

Expected exam answer: A. 90%; 3 more.

---

### A change adds 6 days to a critical-path task and costs $1,800. The schedule has a 4-day buffer. The current budget is $25,000. If approved, what are the net schedule delay and the revised budget?
A. 2 days; $26,800
B. 6 days; $26,800
C. 2 days; $23,200
D. 10 days; $26,800

Correct answer: A. 2 days; $26,800

### Step 1: Calculate the net schedule delay

The change adds 6 days, but the project has a 4-day schedule buffer.

$$
\text{Net delay}=6-4=\boxed{2\text{ days}}
$$

### Step 2: Calculate the revised budget

$$
\text{Revised budget}=\text{Current budget}+\text{Change cost}
$$

$$
=\$25{,}000+\$1{,}800=\boxed{\$26{,}800}
$$

Final answer: A. 2 days; $26,800.

Exam tip: Subtract the available schedule buffer from the added duration to find the net delay, and add the change cost to the current budget.

---

### Velocity forecast | Intermediate | Numerical 
A team completed 25, 20, and 30 points in three sprints. 100 points remain. Using the average velocity, how many sprints are needed?
- A. 3
- B. 4
- C. 5
- D. 6

Correct answer: B. 4 sprints

### Step 1: Calculate average velocity

$$
\text{Average velocity}=\frac{25+20+30}{3}
$$

$$
=\frac{75}{3}=25\text{ points per sprint}
$$

### Step 2: Calculate the number of sprints needed

$$
\text{Sprints needed}=\frac{\text{Points remaining}}{\text{Average velocity}}
$$

$$
=\frac{100}{25}=\boxed{4\text{ sprints}}
$$

Final answer: B. 4 sprints.

Exam tip: Average the completed sprint velocities first, then divide the remaining work by that average.

---
### Velocity | Intermediate | Numerical
A team committed to items of 8, 5, 5, and 3 points. It finished the 8, one 5, and the 3. The second 5-point item is 90% done. What is the sprint velocity?
- A. 16
- B. 17
- C. 20.5
- D. 21

Correct answer: A. 16 points

### Step 1: Identify completed items

- 8-point item: completed = 8 points
- First 5-point item: completed = 5 points
- 3-point item: completed = 3 points
- Second 5-point item: 90% complete = 0 points counted

### Step 2: Calculate sprint velocity

Sprint velocity counts only fully completed items, not partially completed work.

$$
\text{Velocity}=8+5+3=\boxed{16\text{ points}}
$$

Final answer: A. 16

Exam tip: In Scrum, a 90%-complete item earns zero velocity points until it meets the Definition of Done.

---
### Burndown | Intermediate | Numerical 
A 10-day sprint starts with 40 points. After day 3, 31 points remain. How does this compare with the ideal burndown?
- A. 3 points ahead
- B. 3 points behind
- C. 9 points behind
- D. Exactly on track

Correct answer: B. 3 points behind

### Step 1: Calculate the ideal remaining work after day 3

The sprint starts with 40 points over 10 days.

Ideal burn rate:

$$
\frac{40}{10}=4\text{ points/day}
$$

After 3 days, the ideal remaining work is:

$$
40-(3\times4)=28\text{ points}
$$

### Step 2: Compare actual vs. ideal

- Ideal remaining: 28 points
- Actual remaining: 31 points

$$
31-28=\boxed{3\text{ points behind}}
$$

Final answer: B. 3 points behind.

Exam tip: If actual remaining work is higher than ideal, the team is behind schedule. If it is lower, the team is ahead.

---

### Kanban | Intermediate | Numerical 
A Kanban team averages 12 items in progress and finishes 4 items per week. Using Little’s Law, the average cycle time is about:
- A. 1 week
- B. 3 weeks
- C. 8 weeks
- D. 48 weeks

Correct answer: B. 3 weeks

### Step 1: Apply Little’s Law

$$
\text{Cycle Time}=\frac{\text{Work in Progress (WIP)}}{\text{Throughput}}
$$

### Step 2: Substitute the values

- WIP = 12 items
- Throughput = 4 items per week

$$
\text{Cycle Time}=\frac{12}{4}=\boxed{3\text{ weeks}}
$$

Final answer: B. 3 weeks.

Exam tip: Little’s Law is WIP = Throughput × Cycle Time. Rearrange it to find whichever value the question asks for.

---

### . Closure (final cost) | Advanced | Numerical 
Original baseline: $40,000. Approved changes: +$3,000 and −$1,000. Actual cost: $41,500. How should the result be reported?
- A. $1,500 over the original baseline and $500 under the revised budget
- B. $500 over the revised budget
- C. $1,500 under budget in every comparison
- D. $2,000 over the revised budget

Correct answer: A. $1,500 over the original baseline and $500 under the revised budget

### Step 1: Calculate the revised budget

Original baseline = $40,000

Approved changes:

- Increase: +$3,000
- Decrease: −$1,000

$$
\text{Revised budget}=40{,}000+3{,}000-1{,}000
$$

$$
=\boxed{\$42{,}000}
$$

### Step 2: Compare actual cost with the original baseline

$$
41{,}500-40{,}000=\boxed{\$1{,}500}
$$

The project cost $1,500 more than the original baseline.

### Step 3: Compare actual cost with the revised budget

$$
42{,}000-41{,}500=\boxed{\$500}
$$

The project finished $500 under the revised budget.

Final answer: A.

Exam tip: At closure, distinguish the original baseline from the revised budget after approved changes. Report the actual cost against both when asked.