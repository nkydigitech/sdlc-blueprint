# What is Scrum? The Framework That Makes Agile Work

## Definition

**Scrum** is a framework for implementing Agile principles.

Agile is the mindset ("work in small pieces, get feedback, adapt"). Scrum is the structure that makes it happen.

---

## The Scrum Framework at a Glance

```
┌─────────────────────────────────────────────────────────┐
│ SPRINT (2 weeks)                                        │
│                                                         │
│ Day 1: Sprint Planning → Days 2-9: Build → Day 10: Done │
│                                                         │
│ Daily:                                                  │
│ - 15-min standup: "What did I do? What will I do?"     │
│ - Work on Sprint Tasks                                  │
│ - Update ticket status                                  │
│                                                         │
│ End of Sprint:                                          │
│ - Sprint Review: Show what was built                    │
│ - Retrospective: What went well? What needs fixing?     │
│                                                         │
│ Then repeat for Sprint 2, 3, 4...                       │
└────────���────────────────────────────────────────────────┘
```

---

## The Core Concepts

### 1. **Sprint** (Time Box)

A Sprint is a **fixed 2-week period** where the team commits to building specific features.

**Why 2 weeks?**
- Short enough to get feedback quickly
- Long enough to build something meaningful
- Easy to plan
- Not exhausting

**What happens in a Sprint:**

| Day | Event | What You Do |
|-----|-------|-------------|
| Day 1 (Mon) | **Sprint Planning** | Team meets. "What are we building this sprint?" Pick stories from backlog. |
| Days 2-9 (Tue-Wed) | **Daily Work** | Developers build. QA tests. Daily standup at 9 AM. |
| Day 10 (Fri) | **Sprint Review** | Show the customer what you built. Get feedback. |
| Day 10 (Fri) | **Retrospective** | Team talks: "What went well? What didn't? How do we improve?" |
| Day 11 (Mon) | **New Sprint Starts** | Do it all again |

---

### 2. **Product Backlog** (The Master To-Do List)

The **Product Backlog** is a prioritized list of everything that needs to be built.

**Example for a Blog Platform:**

```
Priority 1 (Build First):
- User registration and login
- Create and publish posts
- Edit and delete posts

Priority 2 (Build Next):
- Comments on posts
- Search for posts
- Like/favorite posts

Priority 3 (Build Later):
- Share on social media
- Analytics dashboard
- Mobile app
```

**Who maintains it?** The **Product Owner** (more on that later).

**Why prioritize?** You might not have time to build everything. At least build what matters most.

---

### 3. **Sprint Backlog** (This Sprint's Work)

The **Sprint Backlog** is the **subset of the Product Backlog** that you commit to finishing in this sprint.

**Example:**

```
Product Backlog (big list of everything):
├── User registration
├── User login
├── Create posts
├── Edit posts
├── Delete posts
├── Comments
├── Search
└── ... (100 more items)

Sprint Backlog (what we're doing THIS sprint):
├── User registration
└── User login

"We picked these 2 items. We'll finish them in 2 weeks."
```

---

### 4. **User Story** (The Building Block)

A **User Story** is one feature written from the **user's perspective**.

**Format:**
```
As a [type of user]
I want to [action]
So that [benefit]
```

**Real examples:**

```
As a blog reader
I want to search for posts by title
So that I can find content quickly

As a blogger
I want to edit my posts after publishing
So that I can fix mistakes

As a user
I want to reset my password
So that I can regain access if I forget it
```

**Why this format?** It forces you to think about **why** you're building it, not just **what** you're building.

---

### 5. **Task** (The Technical Work)

Each **User Story** is broken down into **Tasks** — the actual work developers do.

**Example Story:**
```
As a user, I want to reset my password so I can regain access.
```

**Tasks for this story:**
```
- Create password reset form
- Add email validation
- Generate reset token
- Send email with reset link
- Create reset landing page
- Update password in database
- Test with invalid tokens
- Test email delivery
```

---

### 6. **Story Points** (How Big Is the Work?)

**Story Points** estimate how much work a story requires.

Instead of saying "2 days", Agile teams say "5 story points".

**Why?** Because estimates in days are often wrong. But relative sizing is reliable.

**Common scale:**
```
1 point:  Tiny, easy work (1-2 hours)
2 points: Small work (half day)
3 points: Medium work (1 day)
5 points: Medium-large work (1-2 days)
8 points: Large work (2-3 days)
13 points: Very large (3+ days, maybe split it?)
```

**In practice:**
```
Story A: "Add a button to the UI" → 1 point
Story B: "Integrate with payment API" → 8 points
Story C: "Write login feature" → 5 points
```

**Team capacity:** "We usually complete 20 story points per sprint."
So they pick stories adding up to ~20 points.

---

## The Scrum Roles

Every Scrum team has 3 key roles:

### 1. **Product Owner (PO)**

**Responsibility:** Decide what to build.

**What they do:**
- Maintain the Product Backlog (prioritize items)
- Answer questions: "Why are we building this?"
- Accept or reject finished work
- Talk to stakeholders/customers
- Adjust priorities based on feedback

**Who is this?** Usually a business person, product manager, or senior developer with business sense.

### 2. **Scrum Master**

**Responsibility:** Make sure the team follows Scrum and removes roadblocks.

**What they do:**
- Run standups, sprint planning, retros
- Remove blockers ("I'm stuck on X, can someone help?")
- Protect the team from distractions
- Coach the team on Scrum practices
- **NOT** a manager. They don't tell people what to do.

**Who is this?** Could be anyone, but usually someone who's trained in Scrum.

### 3. **Development Team**

**Responsibility:** Build the product.

**What they do:**
- Estimate stories
- Commit to completing sprint work
- Code, test, deploy
- Participate in standups and ceremonies
- Help each other

**Who is this?** Developers, QA, designers, anyone who builds the product.
**Size:** Typically 3-9 people.

---

## The Scrum Ceremonies (Meetings)

Scrum has 4 official meetings per sprint:

### 1. **Sprint Planning** (2 hours)

**When:** Start of sprint (Monday morning)

**Who:** Whole team + Product Owner

**What happens:**
1. PO presents the top prioritized stories from the backlog
2. Team asks questions: "What does this mean? How big is it?"
3. Team estimates: "I think that's 3 points"
4. Team picks stories: "We can do stories A, B, and C this sprint (total 15 points)"
5. Team breaks stories into tasks
6. Sprint Backlog is created

**Output:** "This is what we're building. Here are the tasks. We commit to finishing."

---

### 2. **Daily Standup** (15 minutes)

**When:** Every day at 9 AM (or start of workday)

**Who:** Whole team

**What happens:** Each person answers 3 questions:
1. What did I complete yesterday?
2. What will I work on today?
3. Am I blocked on anything?

**Example:**
```
Alice: "Yesterday I finished the login form. Today I'll add password validation. Not blocked."

Bob: "Yesterday I finished the API endpoint. Today I'll add error handling. I need help with JWT tokens."

Carol: "Yesterday I tested login. Found 2 bugs. Today I'll retest after Bob fixes them. Not blocked."

Dave (Scrum Master): "Bob, let's find someone to help with JWT after standup."
```

**Note:** Standup is NOT a status report to the manager. It's the team syncing up with each other.

---

### 3. **Sprint Review** (1-2 hours)

**When:** End of sprint (Friday afternoon)

**Who:** Team + Product Owner + Stakeholders (sometimes customers)

**What happens:**
1. Team shows what they built (live demo, not slides)
2. Stakeholders/PO give feedback
3. Discuss: "Is this what you wanted?"
4. Update backlog based on feedback

**Example:**
```
Team: "Here's the working login feature. You can register and log in."
PO: "Perfect! I have one question: can users reset their password?"
Team: "Not yet. That's on the backlog for next sprint."
PO: "Good. Let's prioritize that."
```

---

### 4. **Retrospective** (1 hour)

**When:** End of sprint (Friday afternoon, after review)

**Who:** Only the team (no PO, no stakeholders)

**What happens:** Team discusses openly:
1. What went well this sprint?
2. What didn't go well?
3. What will we do differently next sprint?

**Example discussion:**
```
What went well:
- We finished everything we committed to
- The daily standups kept us aligned
- Bob's code was really clean

What didn't go well:
- We had 2 production bugs after launch
- Our meetings ran over time
- We didn't have enough testing

What we'll do differently:
- Add 2 hours for QA testing next sprint
- Set time limits on meetings
- Do more peer code review
```

**Important:** This is a **safe space**. People should be honest, not blame each other.

---

## The Full Sprint Cycle

```
Monday 9 AM:         Sprint Planning
                     ↓
Monday 9:15 - Friday 5 PM:
                     Daily work + Daily Standup (9 AM)
                     ↓
Friday 3 PM:         Sprint Review (show what was built)
                     ↓
Friday 4 PM:         Retrospective (discuss improvement)
                     ↓
Next Monday 9 AM:    New Sprint Planning
                     (repeat)
```

---

## 📋 Checkpoint

Before continuing, you should be able to explain:

- [ ] What is a Sprint?
- [ ] What's the difference between Product Backlog and Sprint Backlog?
- [ ] What is a User Story? (Give an example)
- [ ] What are the 3 Scrum roles?
- [ ] What's the difference between Sprint Review and Retrospective?
- [ ] Why do we estimate with Story Points?

**If you can answer these, you're ready to see how this works in real tools.**

---

## 🎯 Challenge

For a blog platform project:

1. Write 3 User Stories (using the "As a... I want... So that..." format)
2. For one story, break it into 5 Tasks
3. Estimate each story with story points
4. Explain: "Which story should be in Sprint 1 and why?"

---

## Next Step

**👉 [Read: Sprint, Backlog, Stories, Tasks](sprint-backlog-stories.md)**

Then we'll set up your first Jira or Azure DevOps project.
