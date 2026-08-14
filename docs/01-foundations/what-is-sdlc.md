# What is SDLC? The Recipe for Building Software

## Definition

**Software Development Life Cycle (SDLC)** is a structured process that guides how teams plan, design, build, test, and release software.

It answers:
- **What** will we build?
- **How** will we build it?
- **Who** will build it?
- **When** should it be ready?
- **How** do we know it works?

---

## Without SDLC (The Chaos Story)

Imagine you're asked to build a "blog platform":

**Monday morning:**
- You start coding without understanding what a "blog platform" actually means
- Are we building WordPress? Medium? A personal blog? Nobody is clear.

**Wednesday:**
- You've built the backend, but the designer says the UI should be completely different
- You rebuild. Wasted 2 days.

**Friday:**
- You deploy to production. The code crashes because you never tested edge cases.
- Customers are angry. You're fixing bugs at 11 PM.

**Next week:**
- Nobody knows who's working on what
- Features conflict with each other
- The project is 3 months behind and nobody knows why

---

## With SDLC (The Organized Story)

**Monday morning:**
- **Plan:** Team agrees on what "blog platform" means (requirements document)
- **Design:** Architect describes the system (who builds what, technical decisions)
- **Assign:** Tasks are assigned to specific people with deadlines

**Tuesday-Thursday:**
- **Build:** Developers code based on clear requirements
- **Test:** QA tests each feature as it's built
- **Communicate:** Daily standups keep everyone aligned

**Friday:**
- **Deploy:** Code goes to production because it's been tested
- **Monitor:** You watch for issues, but there are none because requirements were clear

**Next week:**
- The project is on track. Features are delivered predictably. The team is happy.

---

## The Five Phases of SDLC

Every SDLC model follows these phases (though they might be called different names):

### 1. **Requirements** (Planning & Analysis)

*"What are we building?"*

- Gather what the customer/business wants
- Document the requirements clearly
- Estimate how long it will take
- Identify risks

**Real example:**
> "The blog platform needs:
> - User registration and login
> - Ability to write, edit, delete posts
> - Comments on posts
> - Mobile-friendly design"

---

### 2. **Design** (Architecture & Planning)

*"How will we build it?"*

- Architects design the system
- Decide on technology stack (Python? Go? Node.js?)
- Plan the database structure
- Outline the user interface

**Real example:**
> "We'll use:
> - Frontend: React
> - Backend: Node.js + Express
> - Database: PostgreSQL
> - Authentication: JWT tokens"

---

### 3. **Development** (Coding)

*"Build it."*

- Developers write the code
- Follow the design from phase 2
- Follow coding standards
- Commit code to version control (GitHub)

**Real example:**
> Developers write the login feature, post creation, comments, etc.

---

### 4. **Testing** (Quality Assurance)

*"Does it work? Will it break?"*

- QA tests the features against the requirements
- Find bugs, report them
- Developers fix bugs
- Test again until it's stable

**Real example:**
> "I clicked Register, but the password validation didn't work."
> Developer fixes it.
> QA tests again. ✅ Works.

---

### 5. **Deployment & Maintenance** (Release & Support)

*"Let customers use it."*

- Deploy to production (the live servers)
- Monitor for issues
- Fix bugs users find
- Release updates

**Real example:**
> The blog platform goes live.
> A user finds a bug with comment notifications.
> The team fixes it and releases an update.

---

## Different SDLC Models (Brief Overview)

Different teams organize these phases differently. Here are the main approaches:

### **1. Waterfall** (The Old Way)

```
Requirements → Design → Development → Testing → Deployment
```

**How it works:**
- Do phase 1 completely, then move to phase 2
- No going back
- All requirements upfront
- All testing at the end

**Pros:**
- Clear structure
- Good for big, stable projects (like NASA rockets)

**Cons:**
- If requirements were wrong, you find out too late
- Hard to adapt to changes
- Testing finds bugs at the end (expensive to fix)
- Takes forever to deliver anything

---

### **2. Agile** (The Modern Way)

```
Sprint 1:           Sprint 2:           Sprint 3:
Plan → Build →      Plan → Build →      Plan → Build →
Test → Deploy       Test → Deploy       Test → Deploy
(2 weeks)           (2 weeks)           (2 weeks)
```

**How it works:**
- Break work into small "sprints" (usually 1-2 weeks)
- Plan a little, build a little, test a little, release a little
- Get feedback from users quickly
- Adapt based on feedback

**Pros:**
- Adapt to changes quickly
- Find bugs early (cheaper to fix)
- Deliver working software every sprint
- User feedback shapes the product

**Cons:**
- Requires more communication
- Harder to predict exactly when you're done
- Needs disciplined teams

---

### **3. DevOps** (The Continuous Way)

```
Code → Build → Test → Deploy → Monitor → Repeat (every day, or every hour)
```

**How it works:**
- Automation does most of the work
- Deploy changes to production continuously (multiple times per day)
- Monitor in real-time
- Fix issues immediately

**Pros:**
- Fastest feedback loop
- Bugs fixed within hours, not weeks
- Most efficient for cloud-native apps

**Cons:**
- Requires heavy automation
- Needs mature team
- Monitoring is critical

---

## Why Did Agile Win?

In the 1990s-2000s, Waterfall was standard. But teams realized:

1. **Requirements change** — Customers don't know what they want until they see it
2. **Feedback is gold** — Getting feedback early saves months of wasted work
3. **Teams are smarter together** — Daily communication beats big documentation
4. **Speed matters** — Shipping in 2 weeks beats shipping in 6 months

So in 2001, a group of developers wrote the **Agile Manifesto** — a better way to build software.

**The Agile Manifesto (simplified):**
- **Individuals and interactions** over processes and tools
- **Working software** over comprehensive documentation
- **Customer collaboration** over contract negotiation
- **Responding to change** over following a plan

**Translation:**
- Talk to your team instead of just following process
- Ship working code early and often
- Keep the customer involved
- Be ready to pivot when things change

---

## How This Connects to Agile & Scrum

Now you understand **why** Agile exists.

Next, we'll look at **Scrum** — the most popular way to do Agile. Scrum is how teams organize their sprints, communicate, and deliver.

---

## 📋 Checkpoint

Before continuing, you should be able to explain (in your own words):

- [ ] What is SDLC?
- [ ] What are the five phases of SDLC?
- [ ] What's the main difference between Waterfall and Agile?
- [ ] Why did Agile become popular?
- [ ] Can you give an example of a project that would be Waterfall vs Agile?

**If you can answer these, you're ready for the next section.**

---

## 🎯 Challenge

**Your turn:**

Think about a project you know (building a house, organizing an event, developing an app).

1. What would the **five SDLC phases** look like for that project?
2. Would you use **Waterfall** or **Agile**? Why?
3. What could go wrong if you used the wrong approach?

Write your answers down. You'll reference them later.

---

## Next Step

**👉 [Read: What is Agile?](../02-agile-scrum/what-is-agile.md)**

We're about to connect SDLC to Agile and see how real teams actually work.
