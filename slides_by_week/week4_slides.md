# SIERRA Literacy Month — Week 4 Slides
## Days 14–19: Knowledge Systems & Tools

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 14: Memories & Customization*

---

**Day 14: Memories & Customization**

*Opening note: "I mentioned context engineering at the end of Day 10 — we'll get to the full picture today and next week. First, the simplest thing you can do to make Sierra better before you type a single word."*

**Stop re-explaining yourself. Every thread shouldn't start from zero.**

**What memories do:**
- Memories are persistent context — they carry into every thread automatically, without you typing them
- Sierra uses them as background when forming responses
- The response improves before you type a single word

**What to put in them:**
Things you'd otherwise repeat at the start of every prompt:
- **Role / specialization** — e.g. marine surveyor, hull & machinery, new construction vs. in-service
- **Operating context** — e.g. division, regions, typical asset types or survey work you do most often *(stable across threads)*
- **Preferences** — e.g. concise by default, bullet points unless you ask otherwise, plain vs. technical language as your usual default
- **Regulatory focus** — e.g. ABS Rules & Guides, SOLAS, MARPOL, IACS — whichever frameworks you usually reason in *(bias the angle; don't replace Plato or files)*

*Who you're writing for often changes thread to thread — put that in the prompt when it matters, not in memories.*

**How to set them:**
Tell Sierra directly — *"Remember that I..."* — or add them in your profile settings.

**Personal vs. Workspace memories:**
- Personal memories: yours alone — follow you across all your standard threads
- Workspace memories: shared across a team — covered tomorrow with Workspaces

**Set it once. Stop repeating it every thread.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 15: Workspaces — Part 1*

---

**Day 15: Workspaces — Part 1**

- A workspace is a shared environment where threads can access common instructions, context, and files — configure it once, work done in that workspace benefits from it
- **Workspace Context:** standing guidance and background knowledge that applies across threads in the workspace
- **Workspace Memories:** durable shared information relevant to the workspace — available to all threads and users without needing retrieval
- **Workspace Files:** searchable knowledge sources available across threads and users — mention file names in prompts to improve retrieval
- Context works differently depending on where you are — in a workspace, shared workspace-level context shapes every thread automatically

[Visual: Container diagram. Outer box labeled "WORKSPACE." Inside: three stacked horizontal bands — CONTEXT (blue: "Standing guidance"), MEMORIES (purple: "Shared team knowledge"), FILES (teal: "Searchable documents — retrieved on demand"). Outside/below: a smaller box labeled "THREAD" with an arrow pointing into it labeled "Draws from workspace." Callout: "Workspace context is shared and persistent. Thread content is yours and temporary."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 16: Workspaces — Part 2*

---

**Day 16: Workspaces — Part 2**

- **Task Modes:** reusable step-by-step instructions for specific, repeatable workflows — invoked by users when needed
- What a Task Mode can include: steps, which workspace files to reference, which tools to activate, output format requirements
- Rule of thumb: general background → Workspace Context or Memories / specific repeatable activity → Task Mode
- Users invoke a Task Mode when they need it — Task Modes help Sierra follow a more consistent workflow for repeatable tasks
- Real examples: survey report review, client summary generation, compliance assessment, meeting notes

[Visual: Full workspace diagram — same container as Day 15 (now Day 16), now with a fourth band added: TASK MODES (orange: "Reusable workflow instructions — invoked on demand"). Below the diagram: a two-row callout — "Context + Memories: always on, for everything" vs. "Task Modes: invoked when needed, for specific jobs."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 17: Plato — Sierra's Maritime Research Mode*

---

**Day 17: Plato — Sierra's Maritime Research Mode**

- Plato is a specialized Sierra mode for maritime rules and regulatory research — not a general knowledge base
- Built for surveyors, engineers, and auditors researching Class rules, IMO compliance, and survey procedures
- **Knowledge sources inside Plato** *(expanding as Plato develops):*
  - **ABS Rules & Guides** — classification rules for vessel types, offshore structures, and more
  - **IMO/IACS Publications** — relevant conventions, codes, and unified requirements *(partial collection)*
  - **ABS Internal Procedures** — procedural requirements and job aids for surveys and inspections
  - **eCFR** — US federal regulations, Titles 33 (Navigation) and 46 (Shipping)
- Currently in preview — not all content is indexed yet; Plato will tell you when something isn't available rather than guessing
- Plato is designed to show what it searched and why before answering — follow that reasoning to refine your query

[Visual: Four-source diagram — ABS RULES & GUIDES / IMO/IACS / ETQ (ABS Procedures) / eCFR — all feeding into PLATO MODE (center). Label: "Sierra's specialized maritime research assistant — Class rules, regulations, and survey procedures."]

**ABS & Affiliated Companies**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 18: Using Plato Effectively*

---

**Day 18: Using Plato Effectively**

- **Be specific:** state vessel type, rule set reference, Part/Chapter number, or survey stage — vague questions produce vague results
- **Search rule first, then procedure:** find the Class requirement or regulation first, then search ETQ for the corresponding survey procedure or job aid
- **Plato is honest about gaps:** if content isn't indexed, it will say so rather than guess — treat that as a signal to check official sources or consult an SME within ABS
- **Combine with file uploads:** attach a survey report or project document, then ask Plato to cross-reference against the applicable Class rules or regulatory requirements
- **Outside Plato mode:** the standalone eCFR tool in the main Sierra chat lets you search US federal regulations without entering Plato — useful for quick regulatory lookups

> *Less useful: "What are the requirements for this vessel?"*
> *More useful: "What are the hull inspection requirements for a bulk carrier under MVR Part 7?"*

[Visual: Two-prompt comparison (less useful vs. more useful). Below: Rule → Procedure flow: FIND THE REQUIREMENT (Rule Manager / IMO / eCFR) → FIND THE PROCESS (ETQ: PRI/JBA). Callout: "If Plato can't find it, verify through official sources or consult an ABS subject matter expert."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 19: SkillShare & HR Tools*

---

**Day 19: SkillShare & HR Tools**

- **SkillShare:** Sierra can search ABS's internal expertise directory — use it when you need to find a human expert, not just an AI answer *(ABS Group employees only; not available to Bureau or Wavesight by default)*
- **HR Tool:** Sierra has access to ABS HR knowledge — policies, benefits, procedures, specific to company (Bureau/Group/Wavesight) and country — ask naturally, it retrieves accurately
- Both are retrieval tools — same pipeline as Plato and workspace files, different knowledge source
- SkillShare is for finding people; HR is for finding policy — know which one to reach for
- These tools extend what Sierra knows about ABS — they don't replace your judgment or relationships

[Visual: Three-panel row — PLATO (ABS standards/technical), SKILLSHARE (ABS people/expertise), HR TOOL (ABS policies/benefits). Each panel has a short "Best for:" label. Header: "ABS-Specific Retrieval Tools — same pipeline, different sources."]

**ABS & Affiliated Companies**

---
