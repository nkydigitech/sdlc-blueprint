# Development Team: Builds the Product

## Definition

**Development Team** builds the product.

Cross-functional: developers, QA, designers, anyone needed to deliver.

---

## Key Characteristics

### 1. Cross-Functional

**What:** Has all skills to complete work without waiting for outside people.

**Good:**
```
JobConnect Team:
✓ Alice (Frontend)
✓ Bob (Backend)
✓ Carol (QA)
✓ Dave (DevOps)
✓ Eve (Designer)

Can deliver registration end-to-end. No waiting.
```

**Bad:**
```
Team: Alice (Frontend), Bob (Backend)
No QA, no DevOps, no designer.

Wait 2 weeks for QA to test.
Wait 1 week for Ops to deploy.
Feature delayed 3 weeks.
```

---

### 2. Self-Organizing

**What:** Decides HOW to do the work. No micromanagement.

**Good:**
```
PO: "Build registration."
Team: "We'll pair on API, Alice codes UI solo, Carol tests."
PO: "Sounds good."
Team works without asking permission.
```

**Bad:**
```
Manager: "Alice, code UI. Bob, code API. Carol, test Friday."
Manager: "Done by 5 PM."
Team follows orders. Loses ownership.
```

---

### 3. Committed

**What:** Team commits to a sprint. Business respects that.

**Good:**
```
Sprint Planning:
Team: "We can do 15 points."
PO: "Great. I won't change mid-sprint."
Team commits. Focuses. Delivers.
```

**Bad:**
```
Team: "We can do 15 points."
PO: "OK, but I might ask for more."
(Wednesday) PO: "Drop everything. Do this urgent thing."
Team restarts. Fails at everything.
```

---

### 4. Accountable

**What:** Team owns results. No blame-shifting.

**Good:**
```
Sprint Review:
PO: "Is it done?"
Team: "No. We found bugs Friday.
Decided to fix properly instead of shipping broken."
PO: "I appreciate that. Let's improve."
```

**Bad:**
```
PO: "Why isn't it done?"
Bob: "I got busy."
Alice: "Carol delayed testing."
Carol: "Server was down."
(Everyone blames someone else)
```

---

## Size

```
1-2 people: Too small. Can't be cross-functional.
Waiting on external teams.

3-5 people: Sweet spot. Can deliver end-to-end.

5-9 people: Still good. More complex work.
Can parallelize.

10+ people: Too big. Communication breaks down.
Scrum doesn't scale.
```

---

## Composition

**JobConnect team (5 people):**
```
Alice - Frontend developer
Bob - Backend developer
Carol - QA engineer
Dave - DevOps engineer
Eve - Designer (part-time, 3 days/week)
```

**Key:** They have all skills needed. Don't depend on outsiders.

---

## Main Responsibilities

### 1. Estimate Work

**What:** Team decides how big each story is.

```
PO: "How many points for registration?"
Alice: "Frontend 1 point."
Bob: "API 5 points (database, validation, hashing)."
Carol: "Testing 2 points."
Team: "Total 8 points."
```

**Why the team?** QA and DevOps know complexity coders miss.

---

### 2. Execute the Sprint

**What:** Do the work. Finish what was committed.

```
Sprint 1:
Alice: Builds registration form
Bob: Builds registration API
Carol: Writes test cases
Dave: Sets up test environment
Eve: Designs UI improvements

Daily:
- Standup (15 min)
- Work on tasks
- Update status
- Unblock each other
```

---

### 3. Maintain Quality

**What:** Don't ship broken code.

```
Good:
✓ Code review before merging
✓ Test as you code
✓ Refactor messy code
✓ Document complex logic
✓ Leave code better than found

Bad:
✗ Ship code nobody reviewed
✗ Test only at the end
✗ "We'll refactor later" (never happens)
✗ No documentation
✗ Pile on technical debt
```

---

### 4. Collaborate

**What:** Talk to each other. Share knowledge.

```
Good:
Alice & Bob align on data format (30 min)
Bob shares code with Carol (explained)
Carol finds questions → Bob adds comments
Team finishes faster. Knowledge spreads.

Bad:
Everyone codes alone
No code review
Alice throws work at Bob
Bob doesn't understand it
Takes 3x longer
```

---

## ❌ When Team Role Breaks

### Team doesn't estimate
```
PO: "How long for registration?"
Bob: "I dunno. I'll try."

Result: Can't plan. No commitment.
Fix: Team estimates. Not perfect, but better than guessing.
```

### Team blames external people
```
Team: "We didn't finish because Ops didn't help."

Result: Not self-sufficient. Scrum breaks.
Fix: Make the external person part of the team.
```

### No code review
```
Alice: "Done. Shipping."
(Nobody else saw the code)

Result: Bugs. Technical debt.
Fix: Code review is part of done. Everyone reviews.
```

---

## 📋 Checkpoint

Explain:

- [ ] Why is team cross-functional?
- [ ] What does "self-organizing" mean?
- [ ] Why does team estimate, not just devs?
- [ ] What's the ideal size?
- [ ] Can someone be in two teams?

---

## 🎯 Challenge

**You join JobConnect as 6th team member (full-stack developer).**

Q1: Who do you work with daily? Why?

Q2: You get stuck on a technical problem. Who do you ask?

Q3: PO asks to add a feature mid-sprint. What do you do?

Q4: Carol finds a bug in your code. How should she tell you?

Q5: At retro, you think Alice is too slow. How do you bring it up?

Write your answers.

---

## Next Step

**👉 [Read: Scrum Ceremonies](../04-scrum-ceremonies/README.md)**
