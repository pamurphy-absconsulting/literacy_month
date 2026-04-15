# SIERRA Literacy Month — Week 4 Slides
## Days 14–19: Memories, Workspaces & Workflow Development

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 14: Memories*

---

**Day 14: Memories**

*Memories allow for persistent context — new threads don't have to start from scratch.*

[Visual: Three-column layout]

**What memories do:**
- Persistent context — injected into every thread automatically
- SIERRA uses them as background when forming responses
- Grounds the model output and allows for more tailored responses

**What to put in them:**
- **Role / specialization** — *marine surveyor, hull & machinery*
- **Operational Context** — *industry, region, team, organization*
- **Preferences** — *writing style, output format, etc.*

**How to set them:**
- Tell SIERRA: *"Remember that I am a marine surveyor focused on MODU & FPSO."*
- View and modify in profile settings

**Save key context to memories once — automatically included in every thread.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 15: Workspaces*

---

**Day 15: Workspaces**

A workspace is a collaborative environment where multiple 'members' can access common instructions, context, and files.

- **Workspace Context:** Background knowledge that applies across all threads in the workspace
- **Workspace Memories:** Shared information relevant to the workspace that can be dynamically added by each member
- **Workspace Files:** Searchable/retrievable knowledge sources available across threads and members — mention file names in prompts to improve retrieval

*Workspace context is shared and persistent. Thread content is yours and temporary.*

[Visual: Container diagram. Outer box labeled "WORKSPACE." Inside: three stacked horizontal bands — CONTEXT (blue: "Standing guidance"), MEMORIES (purple: "Shared team knowledge"), FILES (green: "Searchable documents"). Arrow down to a smaller box outside labeled "THREAD — yours & temporary." Callout: "Workspace context is shared and persistent. Thread content is yours and temporary."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 16: Workspace Task Modes*

---

**Day 16: Workspace Task Modes**

**Task Modes:**
- Reusable step-by-step instructions for specific, repeatable workflows
- Can include: instructions, steps to take, which workspace files to reference, which tools to activate, output format requirements
- Rule of thumb:
  - General background → Workspace Context
  - Specific repeatable activity → Task Mode
- Real examples: emergency response validation, incident root cause analysis, regulatory compliance check, flag state compliance

**CONTEXT + MEMORIES** *(always on, for everything)* → **TASK MODES** *(invoked when needed, for specific jobs)*

[Visual: Same WORKSPACE container as Day 15, now with a fourth band added: TASK MODES (red: "Reusable workflow instructions"). Below: two boxes — "CONTEXT + MEMORIES: always on, for everything" arrow to "TASK MODES: invoked when needed, for specific jobs."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 17: Workspace Walkthrough*

---

**Day 17: Workspace Walkthrough**

*Live walkthrough of the Sierra workspace interface — building one from scratch.*

**Settings:** Name, description, and member access — search anyone in the company and grant access; the workspace appears in their "Shared with me" tab.

**Context:** Workspace-level background information — set once, available in every chat opened within the workspace. Every new thread starts already up to speed on the domain.

**Files:** Upload key documents at the workspace level — accessible across all threads and members without re-uploading.

**Task Modes:** Saved, reusable prompts for specific tasks — configured and available to any member in any chat within the workspace.

**Memories (in beta):**
- Personal memories: your role, specialization, preferences — injected into all your chats
- Workspace memories: project/client-specific — shared with all workspace members; not the whole company

[Visual: Live screen recording — Sierra workspace interface showing Settings, Context, Files, Task Modes, and Memories tabs. Demo workspace built from scratch during recording.]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 18: Workspace Development*

---

**Day 18: Workspace Development**

*Full workspace build for a proposal generation workflow — step by step.*

**The approach:** Start in a regular chat, not the workspace. Outline what you're trying to configure — you can use the mic and describe it stream of consciousness. Then let Sierra help build the workspace components.

**Step 1 — Establish shared understanding**
Describe the workflow, attach meeting notes. Ask Sierra to summarize everything — not for the summary itself, but to verify it understands the domain before you build anything.

**Step 2 — Analyze the source material**
Upload sample proposals and templates. Ask Sierra to extract: section structure across proposal types, all variable placeholders, boilerplate vs. customization sections, regional content patterns, key differences by proposal type. Review it. This is the foundation.

**Step 3 — Generate the workspace context**
Ask Sierra to write the context block — include purpose, section structure, key variables, team structure, glossary, and an onboarding section so new members can press start and understand the workspace immediately.

**Step 4 — Build the task mode**
Describe the steps you want the prompt to take — Sierra writes the task mode instructions. Paste into the workspace. The prompt: extract and confirm variables → check with user on scope → generate section by section.

**Step 5 — Upload workspace files**
Templates and reference documents that every chat should be able to pull from — loaded once, available always.

**The goal:** 80% of the work handled within Sierra. Teams finish the last 20%. That's a win.

[Visual: Live screen recording — Sierra chat used to build workspace components, then switching into the workspace to paste context, create the task mode, and upload files. Ends with a sample RFQ run through the completed workspace.]

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
