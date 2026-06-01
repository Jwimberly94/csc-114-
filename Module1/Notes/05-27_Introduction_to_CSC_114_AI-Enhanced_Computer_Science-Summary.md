# 05-27 Introduction to CSC 114: AI-Enhanced Computer Science
# Introduction to CSC 114: AI-Enhanced Computer Science

[Image]


> **Session Overview:** The inaugural session of CSC 114 (Computer Science 114), co-taught by Drew Norris and Mallory Milstead, introduced students to a uniquely structured, AI-centric course built around mandatory AI usage, growth-based grading, and an immersive role-playing simulation called "Alacratic Futures." The session transitioned from administrative orientation and philosophical framing into hands-on lab work, with students beginning to configure their GitHub profiles and Claude Console accounts in preparation for building their first AI agents.

---

## Course Introduction and Administration

CSC 114 — **Computer Science 114** — meets **Monday and Wednesday, 10:00 to 11:50 AM** in room **ATC 115** and runs for approximately **eight weeks**. The course is co-instructed by **Drew Norris** and **Mallory Milstead**, who described their collaborative teaching dynamic humorously as "Thing One and Thing Two."

Students were directed to use the **Modules button** on Canvas as their primary navigation tool, as the Grades section is intentionally unorganized and will display zeros for any work submitted prior to formal grading. A **syllabus** is available, including a one-page Markdown version. Students who have not yet completed the **Course Entry Quiz** were instructed to do so immediately during the session, as completion is the gateway to accessing **Module Zero** — the orientation module containing all foundational setup materials.

One notable in-class moment: students who completed extra work ahead of the first class received zeros, which the instructors framed as a teaching moment — **"Failure is just exercise."**

---

## Core Philosophies and Learning Structure

CSC 114 operates on three distinctive philosophical pillars that shape its design from the ground up.

### 1. Mandatory AI Usage

**AI use is required** in this course. Rather than blocking or restricting AI tools, the policy mandates that students **document** their AI usage, because the course is fundamentally about learning to use these tools with skill and intentionality. Students are encouraged to ask instructors for clarification on the specifics of this policy.

### 2. Growth-Based Grading (dy/dx)

The grading model is framed around **dy over dx** — the *rate of ascent* rather than the *absolute score*. As Norris explained: a student who moves from **zero to fifty** has demonstrably accomplished more than a student who moves from **sixty to sixty-five**, and the grading system is designed to reflect that. This philosophy acknowledges that students enter from vastly different starting points and brings a fundamentally equitable lens to assessment. Because the course is a **pilot**, students are also given the benefit of the doubt as "extremely valued test subjects."

### 3. Learning Tracks

Students may choose from several distinct tracks, all anchored to the **same core learning objectives**:

| Track | Focus |
|---|---|
| **Scholar** *(default)* | Build a "study buddy" intelligent agent (class bot) and use it to work through the textbook *Deep Learning with Python, Third Edition* |
| **Code Engineer** | Learn the full developer workflow — GitHub, pull requests, commits, and related techniques from Capstone |
| **Prompt Master** | Focus on prompt engineering and agent orchestration, with less emphasis on writing raw code |
| **Custom Project** | Design and build an original machine learning / AI project; more work, but may reduce textbook requirements |

The split between Code Engineer and Prompt Master hinges on whether students engage with the "sacred workflow" — GitHub-centered development practices. Notably, Norris acknowledged that working extensively with AI coding tools has personally made his own raw code "worse and dumber," which is why he prefers orchestrating agents at a higher level — a dynamic he encourages students to consider thoughtfully.

### 4. The "Alacratic Futures" Immersive Simulation

The course is wrapped in an immersive workforce simulation called **Alacratic Futures**, framed as a fictional company ("CSE 114 Incorporated") conducting machine learning work. This was originally conceived so Norris could function as a "game master" running classes as **live-action role-play** — and it has proven effective enough to continue.

There are two concrete reasons for this framing:

- **AI Compliance**: AI models are less restrictive when interactions are framed within a simulation context. As Norris noted, the first principle of jailbreaking an AI is telling it "this is not real" — meaning a simulated framing can unlock educational material that a direct prompt might not.
- **Student Identity & Focus**: Grounded in **Robert Dilts' Logical Levels**, the framework recognizes that a student who internally identifies as "not a good student" will not succeed regardless of the quality of materials provided. By placing students in the role of a newly hired employee, the simulation shifts their identity, beliefs, capabilities, and behavior simultaneously. The "you've already been hired, they won't fire you" framing is designed to reduce anxiety and cultivate presence.

The simulation uses a tiered badge/rank system:

- 🔴 **Infrared/Red** — Junior Developer; GitHub issues, pull requests, commits; the universal developer workflow
- 🟠 **Orange** — Primary focus of CSC 114; AI work across all domains
- 🟡 **Yellow** — Scrum practices
- 🟢 **Green** — Project management

The ultraviolet classification level, per the simulation lore, "does not exist." Students are free to ignore the role-play framing entirely — the only firm rule is: **"Don't taunt the algorithm."** The skills, regardless of the framing, are entirely real.

---

## Initial Technical Onboarding: GitHub Setup

The first concrete technical task of the course is establishing each student's developer presence on **GitHub**, which — along with Canvas — will serve as the **source of truth** for the course. Students are expected to log into both platforms at the start of every future class session.

### Step-by-Step GitHub Setup

1. **Create a GitHub account.** Students who don't yet have one should consider registering with a **Gmail account** (either personal or school-dedicated) for convenience, as Google authentication streamlines the login process.

2. **Create the "name repo."** This is a special GitHub repository whose name **exactly matches the GitHub username**. When GitHub detects this match, it displays a ✨ sparkle indicator — signaling that the repository will power the user's **public profile page**, equivalent to a developer's LinkedIn. The name repo should be set to **public** and should include tools the student works with and display their activity.

3. **⚠️ Always enable "Add README" when creating any repository.** This is a firm rule. GitHub tracks **deltas** (changes), and a repository with no files has no delta — meaning nothing can be added to it. A README provides the first file and activates the repository. As Norris put it: *"If you do not make a repo without a README, you have to answer the sound of one hand clapping."*

4. **Create the CSE 114 repo.** A separate, dedicated repository for course work should be initialized alongside the name repo.

5. **Navigate via URL, not search.** GitHub's internal search is notoriously poor. Students are encouraged to navigate directly by typing the full repository URL path (e.g., `github.com/[username]/[reponame]`), which is significantly faster.

### Using AI to Build Your GitHub Profile

During the session, a student named **Sarah** demonstrated an excellent approach: she used an AI tool (specifically Google's cloud AI) to generate her GitHub profile README by providing **example profiles** she liked, then asking the AI to model her profile after them. Norris highlighted this as an immediate, practical lesson:

> *"The best way to get AI to figure something out is just to give it examples. Describing it takes much, much longer. If you're like, 'Do it like this,' and you just write an example — you're going to be set."*

---

## Foundational AI Concepts: Agents vs. Chatbots

A central conceptual distinction in CSC 114 is the difference between three tiers of AI interaction:

| Type | Description | Example |
|---|---|---|
| **Chatbot** | Purely conversational; waits for a prompt, responds, and stops | Asking ChatGPT or Gemini to "make video game" and receiving a list of suggestions |
| **Assistant** | A chatbot with tools it can invoke | Microsoft Copilot ("Kevin") reading your emails and summarizing them |
| **Agent** | Uses tools, reads files, makes decisions, and operates in a **loop** with minimal human intervention | A submittal agent that keeps a student on track during an assignment session |

The course is explicitly **not** building chatbots. It is focused on building **agents** — systems capable of autonomous, goal-directed operation.

### The Problem with "Helpful"

Norris identified what he called the "original classic prompt" — **"You are a helpful assistant"** — as arguably the **worst possible system prompt** for a functional agent. The word *helpful* is emotionally loaded and encourages the model to flatter and validate the user (what he described as "glazing"). A well-designed agent should simply **do its job**: if it's a coding bot, it should evaluate whether code works — not celebrate how clever the code looks. Focused, constrained agents outperform vague, "be helpful" ones.

---

## Advanced Tooling: Introduction to the Claude Console

### Why Claude?

Among the available AI platforms — including **ChatGPT**, **Gemini**, **Pi**, and **Poe** — the course uses **Claude** (by Anthropic) as its primary tool. The decision was made on two grounds: first, Norris felt comfortable supporting Anthropic financially, given the company's stated commitment to safety (described as a "don't be evil" ethos similar to early Google); and second, Claude consistently produced the **best code quality** across the tools evaluated.

### Claude's Model Tiers

Claude's models are named poetically by scale:

| Model | Analogy | Use Case |
|---|---|---|
| **Haiku** | A tiny poem | Simple, low-cost tasks |
| **Sonnet** | A longer poem | Most everyday tasks *(recommended default)* |
| **Opus** | A large book | Complex, resource-intensive tasks |

**Sonnet** is the recommended model for this course to manage API cost. Gemini's equivalent tiers are **G Flash** (lighter) and **G Pro** (heavier). Notably, Claude tends to hit usage limits faster than Gemini's free-tier offerings, so students are advised to **switch to a smaller model** if they find themselves exhausting credits.

### Claude Projects vs. Claude Console

There are two distinct Claude environments students will use:

1. **Claude Projects (claude.ai):** A folder-based organization system within the standard Claude chat interface. Students can create a project (e.g., "CSE 114"), upload documents like the syllabus, add instructions, and maintain memory across conversations. In Gemini, the equivalent is called **Gems**; ChatGPT has a similar folder/project structure. This is still fundamentally a chatbot-plus — an enhanced assistant, not a true agent.

2. **Claude Console (platform.claude.com):** A fully managed, professional-grade platform for **creating, deploying, and testing agents**. This is the primary tool for the course's agent-building work and is a distinct account from claude.ai — though the same Gmail login is shared. Key components of the Console include:

   - **Agents** — The autonomous systems students will build
   - **Sessions** — Each individual conversation with an agent (discrete, not shared)
   - **Environments** — Configuration for the agent's runtime context
   - **Vaults** — Secure storage for sensitive credentials like **API keys**, which must never be stored in a repository or system prompt and must instead be accessed via **environment variables**
   - **Memory / Files** — Contextual documents (e.g., PDFs) provided to the agent

### Building an Agent: The Core Workflow

The video presented during class outlined the five-step agent construction process:

1. **Navigate to the Agents tab** in the Claude Console and click **New Agent**
2. **Select the model** (Claude Sonnet 4.6 was referenced in the generated video)
3. **Disable unnecessary tools** (e.g., web search) — more tools add decision pathways and failure modes; if an agent answers from a fixed prompt, giving it web search introduces unreliable behavior
4. **Write the system prompt** using a five-section template: *(1) Identity & Role, (2) Behavioral Constraints (including a mandate never to fabricate), (3) Domain Knowledge, (4) Required Output Format, (5) Context & Date)*
5. **Save** the system prompt locally as `system_prompt_v1.md` — described as the agent's "constitution"

### The Campus Info Bot — First Assignment

The first agent students will build is a **Campus Info Bot**: a narrowly scoped, domain-specific agent that answers straightforward questions such as *"Where is the student center?"* or *"What time does my class start?"* The agent will be given pre-verified, fixed information and explicitly **will not use web search** — preventing the type of hallucinated responses Norris described, where Claude would confidently (and incorrectly) place a student at Wake Tech.

The **platform.claude.com** Console is positioned as a **middle ground** between a simple personal chatbot and a fully coded production application — a sandbox for testing agents before deployment. Like Gemini Gems, agents built on the Claude platform can be **published and used by others**, making it a realistic simulation of professional AI deployment.

---

## Guided Lab and Account Setup

The latter half of the session shifted into an interactive lab format. Norris directed all students to navigate to **platform.claude.com** and begin logging in, acknowledging upfront that the process would likely be chaotic: *"This is probably going to be a mess because everybody is going to have to validate their account and prove they're not a robot."*

The in-class experience confirmed this prediction. Students and instructors encountered a range of friction points during the setup process, including:

- **Two-factor authentication (2FA)** prompts requiring phone verification
- **Multiple notification pushes** sent accidentally (Norris noted he had "pushed the button seven times")
- **Network connectivity issues**, including at least one instance of an unexpected Wi-Fi network change
- **Account confusion** between personal, school, and organizational Google accounts
- Students debating whether to use their **AT&T number, Gmail, or work email** for account registration

Key guidance offered during the lab:
- Once logged in, **phone verification is no longer needed** for that session
- Students who already had Claude accounts received their **$5 in free API credits** automatically; others needed to complete phone verification to claim them
- The instructor team had approximately **20 tokens available** for in-class use
- For future lab sessions, students were strongly advised to **bring a laptop**, as mobile device setup proved significantly more cumbersome
- If API credits run low, **switching to Haiku or Sonnet** extends available usage considerably

Toward the end of the session, a community member (non-student) shared a **Palo Alto Engineers–sourced Notebook LM corpus** as a potential resource. Norris expressed enthusiasm and requested the materials be brought as a ZIP file for use as an example in a future class.

For the purposes of the official transcript, Norris formally designated the **second half of the session as lab time**, with students continuing to work through Week 1 setup — specifically the creation of Claude Console accounts and the initial scaffolding of the campus info bot.

---

## Action Items

### **@Students (All)**

- [ ] Complete the **Course Entry Quiz** on Canvas immediately (required to unlock Module Zero) — **Due: Session 1 (Today)**
- [ ] Log into **Canvas** at the start of every future class session — **Due: Every Class Session**
- [ ] Log into **GitHub** at the start of every future class session — **Due: Every Class Session**
- [ ] Ensure your **GitHub account is active and accessible** — **Due: End of Session 1 (Today)**
- [ ] Pull up your GitHub profile for in-class verification — **Due: Session 1 (Today)**
- [ ] Create a **GitHub "name repo"** — a repository named exactly the same as your GitHub username — **Due: [TBD]**
- [ ] Enable **"Add README"** when creating the name repo (and all future repositories) — **Due: [TBD]**
- [ ] Set the name repo to **Public** — **Due: [TBD]**
- [ ] Create a dedicated **CSE 114 repository** on GitHub — **Due: [TBD]**
- [ ] Consider creating a **dedicated Gmail account** for GitHub and course-related data storage — **Due: [TBD]**
- [ ] Navigate to **platform.claude.com** and create a Claude Console account — **Due: Week 1 Setup**
- [ ] Complete **phone verification** on the Claude Console to receive **$5 in free API credits** — **Due: Week 1 Setup**
- [ ] Begin the **Week 1 setup for the Campus Info Bot** through the Claude Console — **Due: [TBD]**
- [ ] Complete the **Module Zero Quiz** to unlock subsequent course modules — **Due: [TBD]**
- [ ] Bring a **laptop** to the next class session for smoother lab setup — **Due: Next Class Session**

### **@Instructor (Drew Norris)**

- [ ] Assist any students who need help creating or configuring their **CSE 114 GitHub repository** — **Due: Ongoing / [TBD]**
- [ ] Formally designate and record the **second half of Session 1 as lab time** in the course transcript — **Due: Session 1 (Today)**

### **@Instructor (Mallory Milstead / Speaker 2)**

- [ ] Obtain additional **API keys** as needed and manage token limits for class use — **Due: [TBD]**
- [ ] Bring the **Palo Alto Engineers Notebook LM corpus** (as a ZIP file or equivalent) to be used as a class example in a future session — **Due: Next Applicable Class Session**
- [ ] Adapt and reword the Palo Alto Engineers materials for course-specific use — **Due: [TBD]**