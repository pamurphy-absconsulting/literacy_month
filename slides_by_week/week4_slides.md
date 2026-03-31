# SIERRA Literacy Month — Week 4 Slides
## Days 14–18: Knowledge Systems & Tools

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 14: Working with Files — Part 2*

---

**Day 14: Working with Files — Part 2**

- Sierra can generate structured output from files: summaries, extracted data, reformatted content, comparisons
- If output format matters, give Sierra a template — paste an example of what you want and ask it to match the structure
- LLM cleanup: Sierra can reformat and fix messy text extracted from converted or scanned documents
- What Sierra cannot do: produce formatted Word/PDF files, retain brand styling, generate charts, or produce pixel-perfect output
- Practical habit: Sierra gives you the content — you apply the final formatting in Word or PowerPoint

[Visual: Before/after diagram. Left box: "Messy or Raw Input" (rough text, inconsistent formatting). Center: arrow through a box labeled "SIERRA + Template." Right box: "Clean, Structured Output." Below: a small callout — "Sierra produces the content. You handle the final formatting."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 15: Workspaces — Part 1*

---

**Day 15: Workspaces — Part 1**

- A workspace is a persistent, shared context environment for teams — set it up once, every thread inherits it
- **Settings:** control which users have access to the workspace
- **Workspace Context:** written background knowledge injected into the system prompt for every thread — purpose, standards, definitions, standing instructions; always-on, applies to everything
- **Workspace Memories:** shared team memories also injected via the system prompt — no retrieval needed; used for shared project context, team preferences, and workspace-specific knowledge; accessible to all users
- **Workspace Files:** documents loaded via RAG, searchable by any thread and any user — explicitly mention file names in prompts to improve retrieval
- Important: personal memories do not apply inside workspaces; workspace memories do not carry over to regular Sierra chats — they are separate systems

[Visual: Container diagram. Outer box labeled "WORKSPACE." Inside: three stacked horizontal bands — CONTEXT (blue: "Written background — always injected"), MEMORIES (purple: "Shared team knowledge — always injected"), FILES (teal: "RAG-searchable documents — retrieved on demand"). Outside/below: a smaller box labeled "THREAD" with an arrow pointing into it labeled "Inherits from workspace." A separate callout: "Personal memories ≠ Workspace memories."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 16: Workspaces — Part 2*

---

**Day 16: Workspaces — Part 2**

- **Task Modes:** reusable step-by-step instructions for specific, repeatable workflows — invoked by users when needed
- What a Task Mode can include: steps, which workspace files to reference, which tools to activate (File Search, Web Search, SkillShare), output format requirements
- Rule of thumb: general background → Workspace Context or Memories / specific repeatable activity → Task Mode
- Users invoke a Task Mode when they need it — Sierra follows the defined workflow consistently every time
- Real examples: survey report review, client summary generation, compliance assessment, meeting notes

[Visual: Full workspace diagram — same container as Day 15, now with a fourth band added: TASK MODES (orange: "Reusable workflow instructions — invoked on demand"). Below the diagram: a two-row callout — "Context + Memories: always on, for everything" vs. "Task Modes: invoked when needed, for specific jobs."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 17: Plato — ABS Knowledge Base — Part 1*

---

**Day 17: Plato — ABS Knowledge Base — Part 1**

- Plato is ABS's internal knowledge base — procedures, standards, technical guidance, and company-specific reference material
- It works via RAG (same pipeline as Days 12–13) — Sierra searches Plato and retrieves relevant chunks to reason over
- When to use Plato: ABS procedures, technical standards, compliance guidance, anything internal and authoritative
- When not to use Plato: current external events, client-specific data, or information that isn't in the knowledge base
- Specific queries get better retrieval — same principle applies here as everywhere else

[Visual: Three-column positioning diagram. Column 1 — "LLM Internal Knowledge" (general, up to cutoff date). Column 2 — "Plato" (ABS-specific, authoritative, current). Column 3 — "Web Search" (live, external, time-sensitive). Each column has a "Best for:" label below it. Shows users where to reach for what.]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 18: Plato — ABS Knowledge Base — Part 2*

---

**Day 18: Plato — ABS Knowledge Base — Part 2**

- Write better Plato queries: use specific ABS terminology, procedure names, document titles — vague = poor retrieval
- Combine Plato with file uploads for richer context: attach a project document and ask Sierra to cross-reference against ABS standards
- Plato for compliance: ask Sierra to check whether a process or approach aligns with a specific ABS standard or requirement
- Plato has limits — not everything is in it; if Sierra can't find something, it will say so — that's the system working correctly
- Workflow tip: Plato + files + a focused prompt is one of the most powerful combinations in Sierra

[Visual: Workflow diagram. Two inputs on the left — YOUR PROJECT FILE (document icon) and PLATO RETRIEVAL (database icon) — both feed into a CONTEXT WINDOW box in the middle, which flows into MODEL → RESPONSE. Label the output: "Answer grounded in ABS standards + your specific project." Shows the combination pattern clearly.]

**ABS & Affiliated Companies**

---
