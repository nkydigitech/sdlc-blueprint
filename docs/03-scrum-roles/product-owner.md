# Product Owner: Decides WHAT

## Definition

**Product Owner** bridges the business and the team.

They decide **WHAT** should be built and **WHY**.

They do NOT decide **HOW**. (That's the team.)

---

## Main Responsibilities

### 1. Maintain Product Backlog

**What:** Prioritized list of everything that could be built

**For JobConnect:**
```
Must Build First:
- User registration
- Job search
- Apply to jobs

Build Next:
- Employer dashboard
- Notifications
- User profile

Build Later:
- Advanced filters
- Mobile app
- Analytics
```

**Why prioritize?** Limited time. Build what matters most first.

---

### 2. Define Requirements Clearly

**What:** Write stories so the team knows exactly what "done" looks like.

**Bad requirement:**
> "Build a login form."

**Good requirement:**
```
User Story: User Login

As a job seeker
I want to log in with email and password
So that I can access my saved jobs and applications

Acceptance Criteria:
✓ User can enter email
✓ User can enter password
✓ Email and password are validated
✓ Error messages appear if wrong
✓ User is logged in after successful entry
✓ Works on mobile
```

Now the team knows exactly what "done" means.

---

### 3. Accept Completed Work

**What:** When developers say "done," you verify it actually is.

**Sprint Review:**
```
Developer: "Registration is finished."
PO (Sarah): "Let me check against acceptance criteria."
  ✓ Email validates
  ✓ Password stores securely  
  ✓ Confirmation email sent
  ✓ User can log in after
  ✓ Mobile works
Sarah: "Perfect. Accepted. Ship it." ✓
```

If something's missing, it goes back to the team.

---

### 4. Engage with Stakeholders

**What:** Talk to real users and business people to understand what matters.

```
Sarah talks to employers:
"What's your biggest pain?"
"Bad applications. We post a job, get 500 terrible matches."

Sarah updates backlog:
Add "Screening questions" to Priority 1

Sarah talks to job seekers:
"What would make this easier?"
"Filter by salary, location, and experience level."

Sarah adds: "Advanced filters"
```

Feedback shapes the product.

---

### 5. Make Trade-Off Decisions

**What:** You have limited capacity. Say YES to some things, NO to others.

```
Team: "We can do 20 story points this sprint."
Sarah has:
- Registration (5 points)
- Dashboard (13 points)
- Notifications (8 points)
- Filters (14 points)

Sarah: "We'll do Registration, Dashboard, Notifications (26 points)."
Team: "That's 26. We said 20."
Sarah: "Try. If not, Filters goes to next sprint."
```

Trade-offs are normal and necessary.

---

## JobConnect's PO: Sarah

**Background:** Was a recruiter for 8 years. Knows the pain points.

**Strength:** Talks to real users. Understands what matters.

**Challenge:** 100 ideas but only 80 story points per sprint.

**Fear:** Building the wrong thing.

**Goal:** Deliver small, valuable features every sprint. Get feedback. Adapt.

---

## ❌ When PO Role Breaks

### PO is absent
```
Team: "Is this right?"
PO: "I don't know. I wasn't involved."

Result: Team builds the wrong thing.
Fix: PO in all ceremonies.
```

### PO keeps changing priorities
```
Monday: "Build feature A."
Wednesday: "Actually feature B."
Friday: "Wait, feature C."

Result: Team can't commit to anything.
Fix: Backlog is stable during a sprint. Adjust next sprint.
```

### PO micromanages HOW
```
PO: "Use React. PostgreSQL. Deploy to AWS."

Result: Team feels controlled. PO owns decisions they shouldn't.
Fix: PO decides WHAT. Team decides HOW.
```

---

## 📋 Checkpoint

Explain:

- [ ] What does PO decide?
- [ ] What does PO NOT decide?
- [ ] Why is the backlog prioritized?
- [ ] What's "acceptance criteria"?
- [ ] When does PO say "no"?

---

## 🎯 Challenge

**You're the PO for JobConnect.**

You have 30 story points per sprint.

Features:
- User Registration (5 pts)
- Job Search (8 pts)
- Apply to Job (5 pts)
- Employer Dashboard (13 pts)
- Notifications (8 pts)
- User Profile (3 pts)
- Advanced Filters (8 pts)
- Saved Jobs (2 pts)

**Task:**

1. Pick what goes in Sprint 1 (max 30 points)
2. Explain WHY those choices
3. What goes to Sprint 2?
4. Write ONE acceptance criterion for "User Registration"

---

## Next Step

**👉 [Read: Scrum Master](scrum-master.md)**
