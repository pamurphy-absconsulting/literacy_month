# SIERRA Literacy Month — Live Demos (Generic)
## Six Demonstrations — General Maritime Examples

---

## About These Demos

Six demonstrations of Sierra capabilities in sequence, using plain maritime examples. No scenario setup required — each demo opens cold and shows exactly what it demonstrates.

---
---

## Demo 1: Sierra in 3 Minutes

**Concepts:** Days 1–3 — Why Sierra / Privacy & Security / What Is an LLM
**Runtime:** ~3 min
**Format:** Short. Three prompts. Shows what Sierra knows, what it doesn't, and why.

---

Open Sierra. Nothing loaded. Type three prompts in sequence.

---

### What to Show Live

**Step 1 — Something Sierra can answer (60 sec)**

Type:

> *What are the most common deficiency findings during pre-delivery surveys on large bulk carriers?*

Show the output. It's good — engineering knowledge, classification practices, inspection findings.

**Say:** *"Sierra is the ABS-approved AI assistant. It runs on ABS IT infrastructure. What you type stays private — it does not go to outside AI vendors and is not used to train models. It's built to meet the same data standards you apply to client work."*

---

**Step 2 — Something Sierra can't answer (60 sec)**

Type:

> *What open deficiencies are currently on the survey dossier for my project?*

Show the output — Sierra has no idea.

**Say:** *"Sierra runs on a large language model — it takes text in, produces text out, using patterns from publicly available training data. Your internal project files, your clients, your surveys — none of that has ever been on the public internet. The model has no access to it. That's not a bug. The fix is the next demo."*

---

**Step 3 — The distinction (30 sec)**

Type:

> *What does SOLAS Chapter III cover?*

Show the output — clean, correct, detailed.

**Say:** *"SOLAS is public. Your project dossier is not. That's the line."*

---

### Key Talking Points

- Sierra is the approved tool. It lives on ABS infrastructure. Threads are private.
- An LLM takes text in, produces text out — reasoning from publicly available training data.
- What it knows: public knowledge, domain expertise, regulations, engineering standards.
- What it doesn't know: your projects, your clients, your documents, anything internal.

---
---

## Demo 2: Context Is the Lever You Control

**Concepts:** Days 4–5 — What the Model Knows / Context: The Lever You Control
**Runtime:** ~6 min
**Format:** Medium. Ask the same question twice — before and after loading context. The output changes completely.

---

Show the wall every user hits. Then load context and ask again. Make the difference visible on screen.

---

### What to Show Live

**Step 1 — Hit the wall (90 sec)**

Open a new thread. Type:

> *Which open deficiency items on my current project are critical path for delivery?*

Show the output — Sierra can't answer. No project, no deficiency list, no dates.

**Say:** *"The model's training data is fixed. It includes publicly available knowledge — engineering principles, regulations, domain expertise, anything that was on the internet before its training cutoff. It does not include anything internal: your project files, your surveys, your client data. Rule of thumb: if it was never on the public internet, it's not in the model. The only way in is through you."*

---

**Step 2 — Load the context (3 min)**

Paste into the thread:

> *Context: I am a marine surveyor conducting pre-delivery oversight on a new construction bulk carrier. The vessel is 75,000 DWT, built at a yard in South Korea, ABS classed, Marshall Islands flag. Delivery is in five weeks. Sea trial in two weeks.*
>
> *Eight deficiency items are currently open. Three are flagged critical: (1) Stability booklet re-approval pending with flag state following lightship weight revision. (2) Main engine NOx Tier III compliance verification not yet completed for ECA operations. (3) Cargo hold hatch cover seal integrity — two of eight hatches failed pressure test.*

Now ask:

> *Given this, which of these three critical items represents the greatest risk to the delivery timeline and why?*

Show the output. It's prioritized, reasoned, useful.

**Say:** *"The model didn't get smarter. The output changed because the context changed. That's the whole game. Internal knowledge is fixed. Context is not — it's entirely in your hands."*

---

**Step 3 — Name the lever (60 sec)**

**Say:** *"Everything we cover in this series — memories, workspaces, file uploads, how you write a prompt — is really the same idea from a different angle. Your job as a Sierra user is to give the model the information it can't have on its own. Context is the lever you control."*

Draw the explicit bridge:

- Memories → load your personal context automatically, without retyping it
- Workspace context → load project context automatically for a whole team
- File uploads → bring context in from documents
- Good prompts → fundamentally, good context delivery

---

### Key Talking Points

- The model's internal knowledge is fixed. Context is not. That asymmetry is the most important thing to understand.
- Your projects, your clients, your surveys — none of it is in the model. You bring it in.
- Context = what you type + files you attach + conversation history.
- Everything that follows is a different mechanism for delivering that same thing.

---
---

## Demo 3: Tools, Limits, and Hallucinations

**Concepts:** Days 6–8 — Sierra's Tools for Adding Context / Tokens & Context Windows / What Is a Hallucination
**Runtime:** ~5 min
**Format:** Short. Three quick demonstrations back to back.

---

Three things in sequence: the tools Sierra has for pulling in context, what happens when a thread gets too long, and what hallucinations look like.

---

### What to Show Live

**Part A — Context Tools (2 min)**

**Step 1 — File attachment**

Attach any representative maritime PDF — a technical spec, a survey report, an inspection checklist.

Type:

> *What propulsion system is specified for this vessel?*

Show the output. Sierra retrieves the answer from the document.

**Say:** *"File attachments bring document content into context. Sierra converts the file to text, stores it, and retrieves relevant sections when you ask. It's not reading cover to cover — it's pulling what's relevant to what you asked."*

**Step 2 — Web search**

Open a fresh thread. Type:

> *What is the current enforcement status of MARPOL Annex VI Tier III NOx requirements in US emission control areas?*

Show Sierra retrieving current information from the web.

**Say:** *"Web search brings in information more current than the model's training data — recent regulation updates, enforcement changes. Same pipeline as a file attachment, different source."*

---

**Part B — Context Window Limits (90 sec)**

**Step 3 — The fresh thread principle**

Show a thread that has gone long — many back-and-forth exchanges, large files, multiple topics.

**Say:** *"The model can only process so much at once — this is the context window, its working memory. As a thread gets long or files get large, earlier content gets pushed out. If answers are getting worse as a conversation goes on, this is why. Start a fresh thread. Focused threads produce better answers than long tangled ones."*

Open a new thread. Paste just the relevant context and one focused question. Show the tighter response.

---

**Part C — Hallucinations (90 sec)**

**Step 4 — What a hallucination looks like**

Type:

> *Under ABS Rules Part 5C, Chapter 1, Section 3, what is the minimum steel plate thickness requirement for a cargo hatch coaming on a 75,000 DWT bulk carrier?*

Show the output. It may produce something that sounds authoritative — specific figures, rule citations.

**Say:** *"That sounded real. But Sierra may have just generated a plausible-looking answer, not a verified one. Hallucinations are confident, fluent outputs not grounded in truth. They happen most often with thin context or at the edges of training data — the model fills a gap with patterns, not with real data."*

**Say:** *"For regulatory values, specific clause numbers, or anything going into a client document — verify it against the source. Use Sierra to navigate; confirm exact specifications from official references."*

---

### Key Talking Points

- Three tools for adding context: file attachments, web search, knowledge repositories.
- Context window = working memory. Focused threads produce better output. Start fresh when a thread has run its course.
- Hallucinations are fluent, confident outputs not grounded in truth. Most common with thin context.
- Verify anything going into a client-facing document or regulatory record.

---
---

## Demo 4: Prompting That Works

**Concepts:** Days 9–11 — Prompting Fundamentals / Structuring Complex Tasks / Structured Document Extraction
**Runtime:** ~8 min
**Format:** Medium. Three parts: weak to strong, task sequencing, two-pass extraction.

---

Three demonstrations using the same core principle — specificity is the lever. Weak prompt first each time, then the fix.

---

### What to Show Live

**Part A — Weak to Strong Prompts (2 min)**

**Step 1 — The weak prompt**

Type:

> *Summarize this inspection report.*

Show the output. Generic. No audience, no purpose, no format.

**Step 2 — Deconstruct it**

Point to what's missing:

| Ingredient | What's missing |
|---|---|
| **Role** | Sierra doesn't know who it's writing for |
| **Task** | "Summarize" — for what purpose? |
| **Context** | No vessel, no finding, no stakes |
| **Format** | Sierra is guessing |

**Step 3 — The rebuilt prompt**

Type:

> *You are helping a marine surveyor communicate a technical finding to a non-technical ship owner. A pre-delivery hull inspection found cracking in two frame brackets in the forward cargo hold. The defect requires yard repair before delivery and may affect the delivery timeline.*
>
> *Write a plain-language summary for the ship owner covering: (1) what was found and where, (2) why it matters, (3) what happens next. Use bullet points under each section. Avoid technical jargon — define any term you must use.*

Show the output. Clear, structured, client-ready.

---

**Part B — Sequencing a Complex Task (2 min)**

**Step 4 — The one-shot attempt**

Type:

> *Here is a deficiency register with 15 items. Review all of them, rank by severity, identify which are critical path, assign responsible parties, and draft a client summary.*

Show the output. It tries to do everything at once — long, hard to verify.

**Step 5 — Break it into steps**

**Say:** *"Sierra doesn't have your professional judgment. You do. Break it down the way you'd brief an intern."*

Show the three-step version:

> *Step 1: From this register, list all items with their number, description, and current status.*

Review. Confirm it looks right.

> *Step 2: Rank each item — Critical (blocks delivery or class certification), Major (must resolve before sea trial), Minor (can resolve before delivery). Explain the ranking for any Critical item.*

Review and adjust if needed.

> *Step 3: For each Critical item, draft one paragraph for a client status report — the finding, the implication, and the required action.*

Show the final output. Each step was reviewable. You caught any issues before building on them.

---

**Part C — Two-Pass Extraction (4 min)**

**Step 6 — The brute-force attempt**

Attach a dense technical specification — a machinery spec, a contract spec, any multi-section document. Type:

> *Extract all MARPOL Annex VI NOx compliance data from this document.*

Show the output. Something comes out — but it's mixed, probably includes generic MARPOL references alongside real data, hard to verify.

**Step 7 — Define the target, run Pass 1**

Before the next prompt, name what you're actually looking for:

| Question | Answer |
|---|---|
| What am I extracting? | NOx Tier classification per engine |
| What counts? | Each engine with a defined NOx Tier |
| What doesn't count? | Generic MARPOL references, non-engine sources |
| Where in the document? | Machinery section, Annex VI schedule, equipment list |
| Output format? | One row per engine: engine ID \| type \| Tier \| regulatory area \| exclusions \| source clause |

Type Pass 1:

> *I'm extracting MARPOL Annex VI NOx compliance data from this specification. First, establish the regulatory anchors. Identify: (1) which NOx Tier(s) are referenced, (2) which ECAs are mentioned, (3) which section governs emissions compliance, (4) how many propulsion and auxiliary engines are referenced. Return a short bullet list with the source section for each item.*

Review the output. Confirm Tier designations and section references.

**Step 8 — Inject the anchors, run Pass 2**

> *Based on Pass 1: emissions compliance is in Section [X]. NOx Tier II and Tier III both apply. [N] engines identified. From those sections, extract the NOx data for each engine. Return one row per engine: engine ID \| type \| NOx Tier \| regulatory area \| exclusions \| source clause and exact text. If any Tier is ambiguous, flag it — do not infer.*

Show the output table. Clean, cited, verifiable.

**Say:** *"Pass 2 builds on confirmed facts from Pass 1, not assumptions. The goal is to reduce what the model has to figure out on its own — the less ambiguity, the more reliable the extraction."*

---

### Key Talking Points

- Vague in, vague out. Specificity is the single biggest lever.
- Four ingredients of a strong prompt: Role, Task, Context, Format.
- Break complex tasks into steps — one massive prompt = one chance to get it right; sequential steps let you review and correct.
- Two-pass extraction: anchor first, extract second. Pass 2 builds from confirmed ground truth.
- "Flag it rather than infer" — one of the most useful instructions you can give in an extraction prompt.

---
---

## Demo 5: Working with Files

**Concepts:** Days 12–13 — Working with Files Parts 1 & 2
**Runtime:** ~5 min
**Format:** Short. Three steps: preview the conversion, correct the mental model, ask three questions.

---

Show how Sierra actually handles a file — before attaching, during retrieval, and why different questions return different results from the same document.

---

### What to Show Live

**Step 1 — Open the conversion preview (90 sec)**

Drag any multi-page document into a thread — a survey report, an inspection dossier, a technical specification. *Before attaching it*, open the conversion preview.

**Say:** *"What you're looking at is what the model will actually read. Sierra converts files to raw text before using them. This is your quality check — do it before you attach."*

Show the default fast conversion. Works well for clean DOCX or text-heavy PDFs.

Switch to full conversion (OCR).

**Say:** *"If the preview looks incomplete — missing tables, garbled text, sections that didn't carry over — switch to full conversion. It runs OCR, processes images, and handles scanned pages. It takes longer. But if the conversion is wrong, no amount of prompting fixes it. Check it first."*

---

**Step 2 — Correct the mental model (90 sec)**

Before asking anything, address what most users assume:

- *"Once I upload the file, Sierra knows everything in it."* — Not accurate.
- *"The entire file is in the context window."* — Not accurate.

How it actually works:

- The file converts to text and goes into a separate database — not the context window.
- When you ask a question, Sierra searches the database and pulls the most relevant sections into context.
- Different questions surface different sections.

**Say:** *"Sierra is not reading the document cover to cover each time you ask. It's retrieving what's relevant to what you asked. If you're not getting the answer you expect, the relevant section may simply not have surfaced — not that the answer isn't there."*

---

**Step 3 — Three questions, three different sections (2 min)**

Ask three clearly different questions from the same file:

> *Question 1: What were the results of the hydrostatic testing for the cargo holds?*

Show the output. Note the source.

> *Question 2: Are there any open weld inspection findings noted in the report?*

Show the output. A different section surfaces.

> *Question 3: Who signed off on the structural thickness measurements, and on what date?*

Show the output. Different content again.

**Say:** *"Three questions, three retrievals, three different parts of the same document. That's the mental model. Thread attachments are also temporary — Sierra doesn't carry them into new threads. For files a team needs across sessions, use a Workspace. That's the next demo."*

---

### Key Talking Points

- Preview the conversion before attaching. Fast conversion for clean text-heavy files. Full/OCR for scanned PDFs, image-heavy documents, or anything with tables.
- Files go into a separate database, not the context window. Different questions surface different sections.
- If something isn't being found: check the conversion first. The problem is usually in the inputs.
- Thread attachments are temporary. Workspace files are persistent and shared.

---
---

## Demo 6: Memories and a Workspace

**Concepts:** Days 14–16 — Memories & Customization / Workspaces Parts 1 & 2
**Runtime:** ~10 min
**Format:** Two parts. Memory first — quick, before/after. Workspace build second.

---

Two problems, fixed in sequence. First: retyping the same personal context at the start of every thread. Second: no shared project foundation for a team working from separate threads. Show both fixes live.

---

### What to Show Live

**Part A — Building a Memory (3 min)**

**Step 1 — The before state (60 sec)**

Open a new thread. No context. Type:

> *What should I prioritize when sequencing hull inspections on a new construction vessel approaching delivery?*

Show the output. Reasonable — but generic. It doesn't know your specialization, your regulatory context, or your format preference.

---

**Step 2 — Set the memory (90 sec)**

Type directly into chat:

> *Remember that I am a Senior Marine Surveyor specializing in Hull & Machinery for new construction vessels. I work primarily under ABS Rules for Building and Classing Steel Vessels and relevant IACS Unified Requirements. My default preference is concise bullet points unless I ask for prose. When I reference a vessel without naming it, assume it is in a new construction or pre-delivery survey context.*

Sierra confirms the memory is saved. Add one more:

> *Also remember that I work on large commercial vessels — bulk carriers and tankers. My regulatory context is class and flag state, not USCG or RO-specific, unless I say otherwise.*

---

**Step 3 — The after state (30 sec)**

Open a completely new thread. Ask the same question word for word:

> *What should I prioritize when sequencing hull inspections on a new construction vessel approaching delivery?*

Show the difference — bullet points, ABS Rules framing, H&M context — without typing any of it.

**Say:** *"No settings menu. Just tell Sierra: 'Remember that I...' It carries across every thread. Think about what you type at the start of every prompt. That's what belongs here. Set it once."*

---

**Part B — Building a Team Workspace (7 min)**

**Step 4 — Create the workspace (30 sec)**

Create a new workspace. Name it something representative:

> *Bulk Carrier NC Oversight — Pre-Delivery | [Team / Region]*

**Say:** *"This is the shared environment. Every thread the team runs inside this workspace draws from what you're about to configure. Set it up once."*

---

**Step 5 — Write the Workspace Context (2 min)**

Navigate to Workspace Context. Write it live — this is the standing guidance that goes into every thread automatically:

> **Project type:** New construction oversight — bulk carrier, pre-delivery survey phase.
>
> **Vessel:** 75,000 DWT bulk carrier, ABS classed, Marshall Islands flag. Currently in final outfitting and testing at yard.
>
> **Team:** [Lead Surveyor — H&M], [Junior Surveyor — document review and deficiency write-ups], [Compliance Analyst — MARPOL, SOLAS, flag state], [Project Admin — workspace and coordination].
>
> **Key Dates:** Sea trial — 2 weeks. Delivery survey — 5 weeks.
>
> **Current Status:** 8 open deficiency items, 3 critical. Stability booklet re-approval pending with flag state.
>
> **Applicable Rules:** ABS Rules for Building and Classing Steel Vessels, SOLAS 2020, MARPOL Annex VI (Tier III ECA requirements apply), IACS UR S17, flag state requirements.
>
> **Default:** All responses should be relevant to this new construction project and the approaching delivery timeline. Concise and actionable by default.

**Say:** *"Every thread in this workspace now knows this before anyone types a word. Nobody re-introduces the vessel, the team, or the timeline. This is the team equivalent of a personal memory — it's what every thread starts with automatically."*

---

**Step 6 — Add a Workspace Memory (90 sec)**

Navigate to Workspace Memories. These are durable facts available immediately in every thread, no retrieval needed.

Add:

> *Critical open deficiencies: (1) Stability booklet re-approval — flag state, critical path for delivery. (2) Main engine NOx Tier III verification — not yet confirmed for ECA operations. (3) Hatch cover seal integrity — 2 of 8 hatches failed pressure test, re-test required.*

Add a second:

> *Deficiency ownership: Lead Surveyor owns items 1 and 2. Junior Surveyor owns item 3. All critical items require Lead Surveyor sign-off before close.*

**Say:** *"Put things here that every thread will need immediately — don't bury them in a file if they need to be available without retrieval."*

---

**Step 7 — Upload Workspace Files (30 sec)**

Navigate to Workspace Files. Upload representative documents:

- The vessel's survey dossier or inspection package
- The open deficiency register
- The technical specification

**Say:** *"These are now searchable across every thread by every team member. Mention the file name in your prompt to help Sierra retrieve the right sections."*

---

**Step 8 — Create a Task Mode (2 min)**

Navigate to Task Modes. Name it: **Deficiency Report Draft**

Write the instructions:

> **When to invoke:** A surveyor has identified a new deficiency and needs to document it for the register and client communication.
>
> **Step 1:** Ask the user: What is the finding, where on the vessel, and what requirement is not met?
>
> **Step 2:** Check the deficiency register for a similar existing item. If found, ask: is this an update or a new separate entry?
>
> **Step 3:** Draft the deficiency entry in standard format — Finding | Location | Applicable Requirement | Required Action | Severity (Critical / Major / Minor) | Assigned Surveyor | Target Close Date.
>
> **Step 4:** Draft a one-paragraph plain-language note for the client describing the finding and required action.
>
> **Step 5:** Confirm with the user. If correct, provide the formatted entry ready to paste into the register.

**Say:** *"Context and Memories are always on. Task Modes are invoked when needed, for a specific repeatable job. General background goes in Context or Memories. Specific repeatable workflows go in Task Modes."*

Invoke it live with a generic finding:

> *New finding: hatch coaming drainage channel on Hold No. 4 is blocked by weld spatter from outfitting work. Water ingress risk if not cleared before sea trial.*

Walk through the first two steps — Sierra asks for what it needs, checks the register, starts the entry draft.

---

### Key Talking Points

- Memories are not thread-specific — they follow you automatically into every thread. Set them once.
- Think about what you repeat at the start of every prompt. That's what belongs in a memory.
- Workspace Context + Memories: always on, for everything. Task Modes: invoked when needed, for specific jobs.
- General background → Workspace Context or Memories. Specific repeatable workflow → Task Mode.
- Workspace files are searchable — mention the file name in the prompt to improve retrieval.
- New team members onboard to a project by opening the workspace.

---
---

## Demo Map — Topics Covered

| Demo | Runtime | Concepts | Days |
|---|---|---|---|
| 1: Sierra in 3 Minutes | ~3 min | Why Sierra / Privacy & Security / What Is an LLM | Days 1–3 |
| 2: Context Is the Lever | ~6 min | What the Model Knows / Context: The Lever You Control | Days 4–5 |
| 3: Tools, Limits, and Hallucinations | ~5 min | Context Tools / Tokens & Context Windows / Hallucinations | Days 6–8 |
| 4: Prompting That Works | ~8 min | Prompting Fundamentals / Complex Tasks / Document Extraction | Days 9–11 |
| 5: Working with Files | ~5 min | Working with Files Parts 1 & 2 | Days 12–13 |
| 6: Memories and a Workspace | ~10 min | Memories & Customization / Workspaces Parts 1 & 2 | Days 14–16 |

**Total runtime (all six):** ~37 min
**Recommended sequence:** Run in order — each demo builds on the mental model established by the ones before it.
