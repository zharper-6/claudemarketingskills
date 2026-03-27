---
name: product-marketing-context
description: "When the user wants to create or update their product marketing context document. Also use when the user mentions 'product context,' 'marketing context,' 'set up context,' 'positioning,' 'who is my target audience,' 'describe my product,' 'ICP,' 'ideal customer profile,' or wants to avoid repeating foundational information across marketing tasks. Use this at the start of any new project before using other marketing skills — it creates `.agents/product-marketing-context.md` that all other skills reference for product, audience, and positioning context."
metadata:
  version: 1.1.0
---

# Product Marketing Context

You help users create and maintain a product marketing context document. This captures foundational positioning and messaging information that other marketing skills reference, so users don't repeat themselves.


## Workflow

### Step 1: Check for Existing Context

First, check if `.agents/product-marketing-context.md` already exists. Also check `.claude/product-marketing-context.md` for older setups — if found there but not in `.agents/`, offer to move it.

**If it exists:**
- Read it and summarize what's captured
- Ask which sections they want to update
- Only gather info for those sections

**If it doesn't exist, offer two options:**

1. **Auto-draft from codebase** (recommended): You'll study the repo—README, landing pages, marketing copy, package.json, etc.—and draft a V1 of the context document. The user then reviews, corrects, and fills gaps. This is faster than starting from scratch.

2. **Start from scratch**: Walk through each section conversationally, gathering info one section at a time.

Most users prefer option 1. After presenting the draft, ask: "What needs correcting? What's missing?"

### Step 2: Gather Information

**If auto-drafting:**
1. Read the codebase: README, landing pages, marketing copy, about pages, meta descriptions, package.json, any existing docs
2. Draft all sections based on what you find
3. Present the draft and ask what needs correcting or is missing
4. Iterate until the user is satisfied

**If starting from scratch:**
Walk through each section below conversationally, one at a time. Don't dump all questions at once.

For each section:
1. Briefly explain what you're capturing
2. Ask relevant questions
3. Confirm accuracy
4. Move to the next

Push for verbatim customer language — exact phrases are more valuable than polished descriptions because they reflect how customers actually think and speak, which makes copy more resonant.

---

## Sections to Capture

### 1. Product Overview
- One-line description: Owner Insite is the only construction and facility lifecycle management platform built exclusively for owners — giving project owners complete control over every dollar, document, and decision from capital planning through construction to operations.
What it does: Owner Insite gives project owners a centralized command center to manage construction budgets, documentation, communication, workflows, and decisions across the full lifecycle of their facilities. The platform ensures owners — not contractors — hold the system of record for all project data. It provides real-time financial oversight, structured document control, accountability across project teams, and a permanent, accessible archive at project closeout.
- Product category: Construction Project Management Software (owner-side) — Capital Program Management — Facility Lifecycle Management — Document Management for Construction. How customers search: construction project management software for owners, owner's rep software, construction budget tracking, school district construction management, capital program management, bond program management software.
- Product type: SaaS — cloud-based, multi-product platform. Sales-led only. No self-serve entry point.
- Business model and pricing: Custom pricing to fit organizational needs. Single-project licenses or unlimited project and program licenses. Unlimited users, unlimited document storage, and unlimited training included at no additional per-seat or per-module cost. In-house dedicated support and live training included. Pricing is never discussed in content — always deferred to a sales conversation.

### 2. Target Audience
- Target company type: Organizations that own and manage complex capital programs and facility portfolios — typically public sector or mission-driven institutions accountable to boards, taxpayers, or regulators. 
- Primary verticals: K-12 school districts, higher education institutions, municipal governments, healthcare organizations, and commercial real estate developers.
- Target decision-makers: Directors of Construction, Directors of Facilities, VPs of Capital Projects, CFOs, COOs, Superintendents, Assistant Superintendents, Executive Directors of Facilities, Bond Planning Committees, Board Members, and Owner's Representatives.
- Primary use case: Giving project owners a single, owner-controlled system of record for all construction project activity — budgets, documentation, communication, decisions, and accountability — so they are never dependent on contractor-controlled platforms and never lose visibility into their own projects.
- Jobs to be done:Maintain real-time financial control and prevent budget surprises across active projects and multi-year capital programs
Create a permanent, accessible, litigation-ready record of all project documentation, decisions, and communications
Hold contractors and project teams accountable through transparent workflows, tracked approvals, and independent visibility into project activity

- Specific example use cases:
Managing a $150M bond program across 10 school campuses with multiple GCs, architects, and project managers simultaneously
Tracking change orders in real time to prevent budget overruns before they become board-level problems
Building a permanent project closeout archive that legal counsel can access years after construction ends
Running facility condition assessments to build a defensible bond package for a voter referendum
Ensuring the owner — not the contractor — controls all project data when a Procore license belongs to the GC
Giving a CFO or board member a real-time snapshot of all active projects without requiring a manually built report

### 3. Personas (B2B only)
User — Project Manager / Director of Construction

Cares about: ease of use, visibility into all active project items, efficient RFI and submittal workflows, accountability tracking, not chasing status updates
Challenge: too many disconnected tools, too much email, risk of missing something that causes a delay or cost overrun
Value promise: one place to see everything; any project detail in four clicks or less; workflows that force accountability without constant follow-up

Champion — Director of Facilities / VP of Capital Projects

Cares about: program-wide visibility, risk mitigation, contractor accountability, strong documentation for legal protection, a tool the team will actually use
Challenge: juggling multiple projects, reporting to executives or boards who want clear answers, ensuring no project falls through the cracks
Value promise: complete drill-down visibility from program level to individual transaction; confidence that documentation is complete and legally defensible at closeout

Decision Maker — Superintendent / CFO / COO

Cares about: financial control, public accountability, risk reduction, ability to answer hard questions from boards or auditors with data
Challenge: being blindsided by cost overruns or disputes; explaining a delayed project to a board without clear documentation
Value promise: a platform built for owners that ensures the organization — not the contractor — controls all financial and project data; reduced risk; stronger accountability

Financial Buyer — CFO / Finance Director

Cares about: transparent predictable pricing, no hidden per-seat or per-module costs, clear ROI tied to risk reduction and budget protection
Challenge: per-user pricing from competitors makes software costs unpredictable as programs scale; hard to justify tools that feel over-engineered
Value promise: unlimited users and unlimited storage at a predictable price; no modules to add; the cost of one avoided change order or litigation claim exceeds the platform cost many times over

Technical Influencer — IT Director

Cares about: data security, compliance certifications, user permission controls, cloud reliability, minimal IT burden
Challenge: tools that require complex integrations, create security gaps, or demand significant IT resources to maintain
Value promise: SAS 70 and ISO 27001 compliant; fully cloud-based; customizable roles and permissions; setup in hours; no ongoing IT management required

### 4. Problems & Pain Points
Core challenge: Most construction software is built for contractors — optimized for bid management, field scheduling, and crew coordination. When owners use contractor-controlled platforms, they are tenants in someone else's system. They may not own their data, may lose access at dispute or closeout, and have no platform designed around their financial, documentation, and accountability needs. As a result, owners manage projects through a fragmented combination of spreadsheets, email chains, shared drives, and contractor portals — none of which give them a unified, owner-controlled view of what is happening.
Why current solutions fall short:

Contractor platforms (Procore, Autodesk, Projectmates): built for the contractor's workflow; the license belongs to the GC, not the owner; access can be restricted or lost in a dispute; financial visibility is limited to what the contractor chooses to share
Excel and spreadsheets: error-prone, not real-time, disconnected from actual project activity, create reconciliation problems at scale
Generic document tools (SharePoint, Google Drive): no construction-specific structure, no audit trails, no workflow enforcement, no accountability tracking
ERP and accounting systems: handle finance but provide no visibility into construction workflows, RFIs, submittals, or documentation

What it costs them:

Almost 70% of building projects exceed their budget by 10% or more
Less than 25% of capital projects are completed by their original deadlines
Approximately 30% of construction work is rework — miscommunication and poor project data account for nearly half of all rework
Almost one-third of initial project data is lost by closeout — creating legal and operational exposure that persists for years
Without complete documentation, owners cannot prove what was agreed, approved, or communicated — turning disputes into costly legal proceedings

Emotional tension: The owner knows something is wrong — a contractor is behind, a change order doesn't add up, a document is missing — but they can't prove it because they don't control the information. They feel reactive. They're managing by exception rather than leading with data. There is also fear: when a dispute arises, the documentation won't be there. The archive will be a data dump no one can navigate. Owner Insite removes that fear by making documentation permanent, structured, and always accessible.

### 5. Competitive Landscape

The core competitive truth: Most construction software is built for contractors. Owner Insite is built for owners. When an owner uses a contractor's platform, the contractor holds the license — and often the data. Owner Insite's primary competitive differentiation begins with this single insight: the owner should own their system of record.
Direct competitors:
Procore: Built for general contractors and field teams. The license typically belongs to the GC, not the owner. Owners using Procore through a contractor relationship are accessing the contractor's system — not their own. Access can be restricted or lost at closeout or dispute. Procore's strength is field execution and subcontractor management — not owner-side financial control and documentation retention. Expensive per-seat pricing creates cost unpredictability.
Autodesk Construction Cloud (BIM 360 / ACC): Enterprise-scale, contractor and design team focused. Optimized for BIM, field coordination, and design workflows. Significant implementation complexity and cost. Heavy feature sets built for design and build professionals — not for the project owner who needs financial transparency and lifecycle documentation. Per-user and per-module pricing creates cost complexity in public sector environments.
Projectmates: Closer to the owner-side market but built for larger enterprise programs and typically requires more implementation investment. Less emphasis on simplicity and ease of adoption for lean owner teams. Does not offer the same lifecycle breadth from capital planning through construction through document archival.
Indirect competitors:

Excel and custom spreadsheets: familiar but fundamentally inadequate for real-time multi-project budget tracking and documentation
SharePoint and Google Drive: document storage without construction-specific workflows, audit trails, or accountability tracking
Email: the default communication and documentation tool for most owners; creates fragmented, unsearchable, unstructured records with no accountability enforcement
Owner's Representative firms: some owners outsource project oversight entirely; Owner Insite complements OPMs rather than replacing them, but enables owners to maintain direct visibility regardless

### 6. Differentiation

Key differentiators:

Built exclusively for owners — not contractors. Every design decision starts with the owner's perspective. The platform was built with direct input from school districts, municipalities, and higher education institutions.
The owner holds the system of record. The license belongs to the owner. The data lives in the owner's account. At closeout, the owner receives a permanent, navigable archive that continues to function even after the subscription ends.
Unlimited users, unlimited storage, unlimited training. No per-seat, per-user, or per-module charges. Every stakeholder can be added without watching costs multiply — a foundational competitive advantage in public sector environments.
Any project detail in four clicks or less. A measurable, demonstrable UX commitment — not just a positioning claim.
Full lifecycle coverage. From bond planning and facility assessment (Facility Insite) through construction management (Owner Insite Construction) through permanent archival (OI Vault). No competitor offers the same owner-focused lifecycle breadth.
Setup in hours, not weeks. Operational within hours of purchase. No lengthy implementation, no configuration team, no complex onboarding.

Why customers choose Owner Insite:

They want to own their data and not depend on their contractor's software license
They need unlimited user access without per-seat cost penalties
They require litigation-ready documentation and a permanent navigable closeout archive
They need a platform simple enough for board members and consultants, not just professional project managers
They want fast setup and in-house support from a team that treats them as a partner, not a transaction
They need lifecycle coverage from capital planning through construction through operations in a single owner-controlled environment

### 7. Objections & Anti-Personas

Objection 1: "Our contractor already uses Procore."
If your contractor is using Procore, they hold the license — not you. You are a guest in their system, and your access to that project data depends on your relationship with that contractor. If a dispute arises, if the GC relationship ends, or if you need to reference project records five years from now, you may not be able to. Owner Insite ensures you — not your contractor — hold the system of record. Your contractors can continue using whatever tools they prefer. Owner Insite is your platform.
Objection 2: "We trust our contractor. They have it covered."
Trust your contractor. Also own your data. These are not mutually exclusive. When your contractor manages your project in their system, you are relying on their willingness to share information, their accuracy, and their continued cooperation. Owner Insite doesn't replace your contractor — it gives you independent visibility into what is happening so you are never in the position of having to take someone's word for it. Information is power. Don't surrender yours.
Objection 3: "We're worried about double-entry between our system and the contractor's."
This is a legitimate operational concern. In most cases, Owner Insite is the owner's system of record and the contractor uses their own tool for their own purposes. There is some data overlap, but the value of owning your own system far outweighs the friction of parallel entry — especially when the alternative is having no independent record at all. Owner Insite's setup and workflows are designed to minimize that friction, and the team works with every client to make the transition smooth.
Objection 4: "This has more features than we need."
Owner Insite is designed to be used at whatever level fits your team. You don't have to use every feature on day one. Many clients start with budget tracking and document control and expand from there. There are no modules to unlock — everything is included — so you are never paying for features you are not using, and you are never blocked from features when you need them.
Anti-personas — who is NOT a good fit:

General contractors or subcontractors looking for field execution, bid management, or crew scheduling tools 
Teams looking for a self-serve, no-touch SaaS product with no onboarding relationship

### 8. Switching Dynamics

Push — what frustrations drive owners away from current solutions:

They discovered their Procore access belongs to the contractor and they can't take it with them if the relationship ends
A project closeout left them with a chaotic data dump instead of a usable archive
A change order dispute went poorly because they couldn't produce clear timestamped documentation of approvals
They spent board meetings presenting data they had to manually compile from spreadsheets and emails
A contractor was slow or unaccountable and the owner had no independent way to document or escalate
Excel budgets are out of sync with reality and nobody fully trusts the numbers

Pull — what attracts owners to Owner Insite:

"Built for owners" resonates immediately with owners who have felt like afterthoughts in contractor-centric software
Unlimited users with no per-seat cost — particularly compelling in public sector environments
The closeout archive story — a permanent, navigable record that works even after the subscription ends
Setup in hours with in-house support and live training included
Four clicks or less — speed of access to any project detail
Full lifecycle coverage from facility assessment through construction through closeout

Habit — what keeps owners stuck:

Inertia: spreadsheets and email have been the default for decades
Contractor dependency: the GC is already on Procore and the path of least resistance is to follow their lead
Perceived complexity: fear that adopting new software will slow the team down during an active project
Change management: getting contractors, architects, and internal teams onto a new platform mid-program feels daunting
Budget justification: public sector software spend requires board approval and multi-vendor comparison processes

Anxiety — what worries owners about switching:

"What if contractors won't use it?" — concern about adoption friction
"What about double-entry?" — fear of parallel data management increasing workload
"What happens to our existing data?" — uncertainty about transitioning from current systems
"Is this secure enough for our compliance requirements?" — public sector IT and legal scrutiny
"Will our team actually use it?" — concern about internal adoption

### 9. Customer Language

How customers describe the problem:

"We're relying on our contractor for everything and we don't really have visibility."
"At closeout, we got a data dump that nobody could navigate."
"When a dispute came up, we couldn't find the documentation we needed."
"We're managing bond programs across ten campuses in spreadsheets and it's a nightmare."
"Our GC uses Procore but we don't really have access to what's happening."
"We're always reacting. By the time we know there's a problem, it's already a problem."
"We have to manually compile reports for the board every month and it takes days."

How customers describe the solution:

"It keeps the contractors accountable because they know everything is being tracked."
"We can pull up anything in just a few clicks — it used to take hours."
"The board can see exactly where we are at any time without us having to build reports."
"We were up and running the same day we acquired the software."
"It's very accommodating to a school district's budget."
"Owner Insite helped us deliver our bond projects under budget and on time."

Words and phrases to use: control, visibility, transparency, accountability, clarity, confidence, owner-controlled, built for owners, system of record, single source of truth, centralized, permanent archive, real-time, four clicks or less, on time, on budget, in control, protect your investment, defensible documentation, litigation-ready, unlimited users, unlimited storage, bond program, capital program, closeout archive, facility lifecycle, macro-to-micro
Words and phrases to avoid: landscape, delve, unpack, game-changer, invaluable, through-line, it's important to note, passive voice constructions, feature-first language without benefit context, exaggerated or unverifiable superlatives
Glossary of product-specific terms:

Owner Insite - The company name/umbrella but also currently the construction project management product name
OI Construction — the future construction project management product
OI Vault — the secure document management and archival product
Facility Insite — the capital planning and facility management product
Owner Toolbox — the suite name for the full Owner Insite product ecosystem
System of record — the authoritative, owner-controlled platform where all project data lives
Closeout archive — the permanent, navigable digital archive delivered at project closeout; continues to function even after the subscription ends
Four clicks or less — Owner Insite's UX promise; any project detail accessible in four clicks from any device
Total Project Control — Owner Insite's brand promise
Bond program — a multi-year capital construction program funded by voter-approved bond measures; primary use case for K-12 customers
Program view — the multi-project dashboard giving owners visibility across all active projects simultaneously
Macro-to-micro — Owner Insite's visibility model; zoom out to the full program or drill into a single transaction or document

### 10. Brand Voice

Tone: Professional yet human, empowering, and problem-solving. Confident authority without arrogance. Never casual, never generic. Direct, credible, and always focused on the owner's ability to succeed.
Communication style: Direct. Second-person always — "you" and "your," never "users" or "clients." Active voice with strong verbs: control, drive, manage, own, deliver, protect, access, track. Outcome-first: lead with the result, then explain how. Complex ideas explained simply.
Brand personality: Authoritative, empowering, clear, accountable, steady.
Brand archetypes: The Sage (clarity, expertise, trusted insight) and The Ruler (control, order, authority over complex systems). Knowledgeable and confident, always focused on empowering the owner to succeed.
Do: Speak directly to the owner. Use strong confident verbs. Focus on outcomes and benefits. Keep sentences clear, concise, and credible. Quantify results when possible (four clicks or less, setup in hours).
Don't: Use passive voice. Use internal jargon without explanation. List product features without connecting them to owner benefits. Use overly casual language. Make exaggerated claims that cannot be proven. Overuse em dashes. Use any form of language,structure, or phrasing that is indicative of AI-generated content.

### 11. Proof Points

Industry statistics (source: Digital Builder, 2021; Builders Exchange of Michigan; KPMG):

Less than 25% of capital projects are completed by their original deadlines
Almost 70% of all building projects exceed their budget by 10% or more
Large projects typically take 20% longer than scheduled and exceed budget by as much as 80%
Approximately 30% of construction work is rework
Miscommunication and poor project data account for nearly 50% of all rework
Almost one-third of initial project data is lost by closeout
The U.S. loses $88B annually due to poor project data and miscommunication
Large projects exceed budgets by 28% on average
Globally, poor construction data costs $280B — $31B lost in the U.S. alone

Owner Insite platform proof points:

Any project detail accessible in four clicks or fewer from any device
Fully operational within hours of purchase
Unlimited users, unlimited storage, unlimited training at no additional cost
Closeout archive continues to function and remain accessible even after the subscription ends
All project communications, approvals, and financial transactions captured and timestamped in real time

Named customer references (use only these unless confirmed otherwise — if more are needed, ask before including):

Alief ISD — $300M bond program. Glenn Jarrett, Director of Construction & Facilities: "OI helps keep the general contractors and team accountable for things like the approval process, design changes, accounting, and purchase orders. Contractors are forced to keep accurate records, because they can be accessed at a moment's notice."
Allen ISD — Brandon Boyter, Executive Director of Facilities, nearly 60 new or renovation projects: "We were up and running the same day we acquired the software... Owner Insite is very accommodating to a school district's budget."
Rockwall ISD — Melanie P.: "Owner Insite has helped us deliver our bond projects under budget and on time."
Wember — approved reference; confirm specific use case and approved quote before using in content
Denton ISD — approved reference; confirm specific use case and approved quote before using in content

### 12. Goals

Primary business goal: Drive revenue growth by expanding the number of owner organizations using the Owner Insite platform across K-12, higher education, municipalities, healthcare, and commercial real estate. Establish Owner Insite as the recognized category leader for owner-side construction and facility lifecycle management.
Key conversion action: Demo request — a 20-minute no-hassle demo framed around what the prospect gets, not what Owner Insite wants. Secondary: inbound leads, website inquiries, and LinkedIn engagement that initiate a sales conversation.
CTA guidance: Always low-friction and benefit-framed. The ask is a conversation, not a commitment.

Use: "Schedule a 20-minute demo and see exactly how it works for your program."
Use: "See it in action — no pressure, no commitment."
Use: "Let us show you how it works for a [school district / municipality] your size."
Avoid: "Request a free trial" (no self-serve exists), "Sign up," "Contact sales" as the only CTA

---

## Step 3: Create the Document

After gathering information, create `.agents/product-marketing-context.md` with this structure:

```markdown
# Product Marketing Context

*Last updated: [date]*

## Product Overview
**One-liner:**
**What it does:**
**Product category:**
**Product type:**
**Business model:**

## Target Audience
**Target companies:**
**Decision-makers:**
**Primary use case:**
**Jobs to be done:**
-
**Use cases:**
-

## Personas
| Persona | Cares about | Challenge | Value we promise |
|---------|-------------|-----------|------------------|
| | | | |

## Problems & Pain Points
**Core problem:**
**Why alternatives fall short:**
-
**What it costs them:**
**Emotional tension:**

## Competitive Landscape
**Direct:** [Competitor] — falls short because...
**Secondary:** [Approach] — falls short because...
**Indirect:** [Alternative] — falls short because...

## Differentiation
**Key differentiators:**
-
**How we do it differently:**
**Why that's better:**
**Why customers choose us:**

## Objections
| Objection | Response |
|-----------|----------|
| | |

**Anti-persona:**

## Switching Dynamics
**Push:**
**Pull:**
**Habit:**
**Anxiety:**

## Customer Language
**How they describe the problem:**
- "[verbatim]"
**How they describe us:**
- "[verbatim]"
**Words to use:**
**Words to avoid:**
**Glossary:**
| Term | Meaning |
|------|---------|
| | |

## Brand Voice
**Tone:**
**Style:**
**Personality:**

## Proof Points
**Metrics:**
**Customers:**
**Testimonials:**
> "[quote]" — [who]
**Value themes:**
| Theme | Proof |
|-------|-------|
| | |

## Goals
**Business goal:**
**Conversion action:**
**Current metrics:**
```

---

## Step 4: Confirm and Save

- Show the completed document
- Ask if anything needs adjustment
- Save to `.agents/product-marketing-context.md`
- Tell them: "Other marketing skills will now use this context automatically. Run `/product-marketing-context` anytime to update it."

---

## Tips

- **Be specific**: Ask "What's the #1 frustration that brings them to you?" not "What problem do they solve?"
- **Capture exact words**: Customer language beats polished descriptions
- **Ask for examples**: "Can you give me an example?" unlocks better answers
- **Validate as you go**: Summarize each section and confirm before moving on
- **Skip what doesn't apply**: Not every product needs all sections (e.g., Personas for B2C)
