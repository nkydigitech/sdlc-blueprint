# Sprint, Backlog, Stories, Tasks — How They Connect

## The Hierarchy (Big Picture)

```
Product Backlog (Everything that could be built)
│
├─ Epic 1: User Authentication
│  ├─ Story 1: User Registration
│  │  ├─ Task 1: Create registration form
│  │  ├─ Task 2: Validate email
│  │  └─ Task 3: Store password securely
│  │
│  └─ Story 2: User Login
│     ├─ Task 1: Create login form
│     ├─ Task 2: Validate credentials
│     └─ Task 3: Create session token
│
└─ Epic 2: Blog Posts
   ├─ Story 1: Create Posts
   ├─ Story 2: Edit Posts
   └─ Story 3: Delete Posts

Sprint Backlog (What we're doing THIS sprint)
│
├─ Story: User Registration (Epic: Authentication)
│  ├─ Task: Create registration form
│  ├─ Task: Validate email
│  └─ Task: Store password securely
│
└─ Story: User Login (Epic: Authentication)
   ├─ Task: Create login form
   ├─ Task: Validate credentials
   └─ Task: Create session token
```

---

## Definitions and Examples

### **Epic** (The Big Feature)

An **Epic** is a large feature that's too big to complete in one sprint.

**Examples:**
- "User Authentication" (registration, login, password reset, 2FA)
- "Blog Post Management" (create, edit, delete, publish)
- "Search and Discovery" (search, filters, recommendations)

**Why split into stories?** An Epic might take 4 sprints. A story takes 1.

---

### **User Story** (One Feature)

A **User Story** is one small, complete feature that delivers value to the user.

**Format:**
```
As a [user type]
I want to [action]
So that [benefit]
```

**Acceptance Criteria:**
```
✓ User can enter email and password
✓ Email is validated (must be real email format)
✓ Password is at least 8 characters
✓ Account is created in database
✓ User can log in immediately after
✓ Error messages are clear if validation fails
```

**Example Story:**
```
Story: User Registration

As a new blogger
I want to create an account with email and password
So that I can start publishing posts

Acceptance Criteria:
✓ Registration form is visible and functional
✓ Email must be valid format
✓ Password must be 8+ characters
✓ Account created in database
✓ User can log in immediately
✓ Clear error messages
✓ Works on mobile

Estimate: 5 story points
Sprint: Sprint 1
```

**Why "User Story"?** It keeps the focus on user value, not technical implementation.

Wrong: "Create a user table in PostgreSQL"
Right: "As a blogger, I want to register so I can publish"

---

### **Task** (The Technical Work)

A **Task** is one specific piece of work to implement a story.

**For the "User Registration" story, tasks might be:**

```
Task 1: Design registration form mockup (Designer)
Task 2: Create registration form HTML/CSS (Frontend dev)
Task 3: Build registration API endpoint (Backend dev)
Task 4: Add email validation (Backend dev)
Task 5: Add password strength validation (Backend dev)
Task 6: Test registration flow (QA)
Task 7: Test error messages (QA)
Task 8: Test mobile responsiveness (QA)
```

**Who creates tasks?** The developer, once they understand the story.

**How detailed?** Detailed enough that someone can start working on it immediately without asking "what do I do?"

---

## How They Connect: The Sprint

### **Before Sprint Starts: Product Backlog**

```
Product Owner has prioritized 50 stories:
1. User Registration (5 points)
2. User Login (5 points)
3. Create Posts (8 points)
4. Edit Posts (5 points)
5. Delete Posts (3 points)
6. Search Posts (8 points)
... and 44 more items
```

### **Sprint Planning: Create Sprint Backlog**

Team meeting on Monday:

```
PO: "Here are the top stories. Should we do them?"
Team: "Let's estimate."

Story: User Registration (5 points)
Team: "Yep, 5 points."

Story: User Login (5 points)  
Team: "Yep, 5 points."

Story: Create Posts (8 points)
Team: "That's too big. Let's split it. Maybe just 'Create and publish' is 5 points."

Team decides: "We can do 15 points. So: Registration, Login, and Create Posts."

Sprint Backlog created:
✓ User Registration (5 points)
✓ User Login (5 points)  
✓ Create Posts (5 points)
```

### **During Sprint: Work on Tasks**

Developers take stories and create tasks:

```
Alice works on: User Registration story
  → Task 1: Build registration form (In Progress)
  → Task 2: Add email validation (To Do)
  → Task 3: Store password (To Do)

Bob works on: User Login story
  → Task 1: Build login form (In Progress)
  → Task 2: Validate credentials (To Do)
  → Task 3: Create session (Blocked - waiting for database schema)

Carol works on: Create Posts story
  → Task 1: Build post form (In Progress)
  → Task 2: Save to database (To Do)
  → Task 3: Publish (To Do)
```

### **End of Sprint: Tasks → Stories → Done**

```
Friday (End of Sprint):

User Registration story:
  ✓ Task 1: Form - DONE
  ✓ Task 2: Email validation - DONE
  ✓ Task 3: Password storage - DONE
  → Story STATUS: DONE ✓

User Login story:
  ✓ Task 1: Form - DONE
  ✓ Task 2: Validate - DONE
  ✓ Task 3: Session - DONE
  → Story STATUS: DONE ✓

Create Posts story:
  ✓ Task 1: Form - DONE
  ✓ Task 2: Database - DONE
  ✓ Task 3: Publish - DONE
  → Story STATUS: DONE ✓

Sprint Result: 3 stories completed ✓
```

---

## The Status of Work: Kanban Board

Scrum teams use a **Kanban board** to visualize work:

```
┌────────────────┬────────────────┬────────────────┬────────────────┐
│    TO DO       │  IN PROGRESS   │    REVIEW      │      DONE      │
├────────────────┼────────────────┼────────────────┼────────────────┤
│                │                │                │                │
│ Registration   │  Login Form    │  Registration  │  Search Posts  │
│ (5 pts)        │  (5 pts)       │  (5 pts)       │  (8 pts)       │
│                │                │                │                │
│ Edit Posts     │  Post Form     │  Delete Modal  │  Post Delete   │
│ (5 pts)        │  (5 pts)       │  (3 pts)       │  (3 pts)       │
│                │                │                │                │
│ Password Reset │                │                │  User Profile  │
│ (3 pts)        │                │                │  (3 pts)       │
│                │                │                │                │
└────────────────┴────────────────┴────────────────┴────────────────┘

Reading the board:
- TO DO: Tasks not started yet (20 points of work)
- IN PROGRESS: Team is working on these right now (10 points)
- REVIEW: Built, waiting for testing/approval (8 points)
- DONE: Completed and tested (14 points)
```

---

## Real Workflow Example: Blog Platform Sprint 1

### Monday 9 AM: Sprint Planning

```
PO: "Here are the most important stories."

Story 1: User Registration
  "As a blogger, I want to create an account so I can publish posts"
  Acceptance Criteria:
  ✓ Email validation
  ✓ Password 8+ chars
  ✓ Account created in DB
  ✓ User can log in after
  Estimate: 5 points

Story 2: User Login
  "As a user, I want to log in so I can access my account"
  Acceptance Criteria:
  ✓ Enter email/password
  ✓ Validate against database
  ✓ Create session
  ✓ Remember login (cookie)
  Estimate: 5 points

Story 3: Create Blog Post
  "As a blogger, I want to create and publish posts"
  Acceptance Criteria:
  ✓ Write post title
  ✓ Write post content
  ✓ Publish to blog
  ✓ Post visible publicly
  Estimate: 5 points

Team: "We can do these 3. That's 15 points. We're in!"
```

### Monday 10 AM: Break Stories into Tasks

Developers now break each story:

**Story: User Registration**
```
Task 1 (Frontend): Build registration form
Task 2 (Backend): Create user table in database  
Task 3 (Backend): Build signup API endpoint
Task 4 (Backend): Add email validation
Task 5 (Backend): Hash and store password
Task 6 (QA): Test valid registration
Task 7 (QA): Test invalid inputs (short password, bad email)
```

**Story: User Login**
```
Task 1 (Frontend): Build login form
Task 2 (Backend): Build login API endpoint
Task 3 (Backend): Validate email/password vs database
Task 4 (Backend): Create session token
Task 5 (Frontend): Set session cookie
Task 6 (Frontend): Store login state
Task 7 (QA): Test valid login
Task 8 (QA): Test invalid password
```

**Story: Create Blog Post**
```
Task 1 (Frontend): Build post creation form
Task 2 (Backend): Create posts table
Task 3 (Backend): Build post creation API
Task 4 (Backend): Build publish API
Task 5 (Frontend): Add publish button
Task 6 (Backend): Make published posts public
Task 7 (QA): Test post creation
Task 8 (QA): Test post visibility
```

### Tuesday-Thursday: Daily Work

```
Tuesday 9 AM Standup:
Alice (Frontend): "Yesterday I built the registration form. Today I'll build the login form."
Bob (Backend): "I created the user table and started the signup API. Today I'll finish it and start login API."
Carol (QA): "I tested registration but found an issue with email validation. Bob, can we talk after standup?"

Wednesday 9 AM Standup:
Alice: "Login form done. Today I'll work on the post creation form."
Bob: "Email validation fixed. I finished login API. Today I'll start post creation backend."
Carol: "Registration tests passed ✓. I'll start testing login today."

Thursday 9 AM Standup:
Alice: "Post form done. Ready for testing."
Bob: "Post creation and publish API done. We can deploy today."
Carol: "Login tests passed ✓. Starting post creation tests today."
```

### Friday 3 PM: Sprint Review

```
Team demos to Product Owner:

Demo 1: "You can now register"
  - Open site
  - Enter email and password
  - Click register
  - Account created! ✓
  PO: "Perfect!"

Demo 2: "You can log in"
  - Log out
  - Log in with those credentials
  - Works! ✓
  PO: "Great!"

Demo 3: "You can create and publish posts"
  - Log in
  - Create a post
  - Publish
  - Post shows on the blog ✓
  PO: "Excellent!"

PO: "This is perfect! Next sprint, let's add:
- Post editing
- Post deletion
- Comments"
```

### Friday 4 PM: Retrospective

```
Team discussion:

"What went well?"
  - We finished everything we committed to
  - Bob's code was clean and well-tested
  - Carol found issues early
  - Communication was great

"What didn't go well?"
  - We didn't have enough time to test mobile
  - One API endpoint had a bug we found Friday afternoon
  - Task estimates were off by ~20%

"What will we do differently?"
  - Next sprint, add 4 hours for mobile testing
  - Test APIs earlier (by Wednesday, not Friday)
  - Be more conservative with estimates
```

---

## 📋 Checkpoint

Before moving to Jira/Azure DevOps, you should:

- [ ] Understand the hierarchy: Epic → Story → Task
- [ ] Be able to write a User Story in the correct format
- [ ] Know what goes in a Sprint Backlog
- [ ] Understand how work moves from To Do → In Progress → Done
- [ ] See how a sprint flows: Planning → Daily Work → Review → Retrospective

---

## 🎯 Challenge

**For a "Blog Platform" project, create:**

1. **One Epic:** "User Account Management"
2. **Three Stories** under that Epic (use the format)
3. **For each story, list 3-5 Tasks**
4. **Estimate each story** with story points (1, 2, 3, 5, 8)
5. **Decide:** "If this is Sprint 1, which stories should we include? Why?"

Example:
```
Epic: User Account Management

Story 1: User Registration
As a new blogger, I want to create an account
So that I can start publishing posts
Estimate: 5 points

Tasks:
- Build registration form
- Add email validation
- Store password securely
- Test registration
- Test error messages
```

---

## Next Step

**👉 [Read: Scrum Roles & Ceremonies](../03-roles-ceremonies/README.md)**

Or jump straight to hands-on:
**👉 [Set Up Jira](../04-jira/setup-free-jira.md)** or **[Set Up Azure DevOps](../05-azure-devops/setup-azure-devops.md)**
