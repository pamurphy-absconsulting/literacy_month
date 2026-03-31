# SIERRA AI Literacy Program
## 22-Day Learning Journey (April 1 - May 1, 2026)

---

### WEEK 1 (April 1-3): First Steps
*3 days: Wednesday - Friday*

**Day 1: Why Sierra**
- Sierra is the ABS-approved AI assistant — uses best-available models, resides on ABS IT infrastructure
- Protects client data and keeps messages private from AI vendors
- Meets compliance requirements
- Other AI assistants: not explicitly approved, risk of data leakage

**Day 2: Privacy, Security & Data Governance**
- Policy Compliance: users must abide by the Sierra Data Policy; client contractual terms supersede it
- App Design & Data Governance: chat threads are private; workspaces manage collaboration; limited web search/external resource usage
- Protected IT Infrastructure: approved by ABS cyber teams
- *(Three-layer pyramid: Policy Compliance → App Design & Data Governance → Protected IT Infrastructure)*

**Day 3: What Is a Large Language Model?**
- An LLM is a calculator that converts a text input (prompt) to a text output (response)
- It has learned patterns from vast amounts of text to produce replies that seem knowledgeable and logical
- *(Visual: Text Input → Large Language Model → Text Output)*

---

### WEEK 2 (April 7-11): AI Fundamentals
*5 days: Monday - Friday*

**Day 4: What the Model Knows — and Where It Stops**
- Internal knowledge does NOT include: anything never on the public internet, events after training cutoff, anything ABS-specific
- Internal knowledge DOES include: public knowledge, historical events, general logic, deep domain expertise
- Training cutoffs for current Sierra models: late 2024 to mid-2025
- Rule of thumb: if it was never on the public internet, it is not in the model's internal knowledge
- Everything ABS-specific must come from the user through context

**Day 5: Context — The Lever You Control**
- Two and only two sources: internal knowledge (fixed) and context (what you provide)
- Context is the lever users control — internal knowledge is not
- Context includes: prompt text, files you attach, conversation history
- The model works with both simultaneously — context shapes what it reasons over
- Goal: load up context with what the model can't know on its own

**Day 6: How Sierra Bridges the Gap**
- LLMs are static — parameters set at training, never change, never learn from conversations
- Sierra does not learn from your conversations — your chats do not modify the model in any way
- ABS does NOT train its own LLMs — too expensive, and a trained model is still static
- Solution: ABS builds knowledge systems — curated repositories Sierra retrieves from on demand
- Example: HR vacation policy — Sierra doesn't know it internally; it retrieves from an ABS-built knowledge base
- As ABS evolves, we update knowledge systems — not the model

**Day 7: Tokens, Cost & Context Window**
- Tokens are small pieces of text: words, parts of words, punctuation (~4 characters, ~0.75 words; about 666 tokens per page)
- Every LLM request is priced on tokens processed — both input and output; tokens are cheap, ABS absorbs significant usage
- Models reprocess the entire conversation history with each message — long, noisy threads degrade output quality
- Context window = working memory: everything the model can hold in mind at once while responding
- Current Sierra models: 200,000 to 2,000,000 tokens (~300–3,000 pages); focused threads keep that memory on what matters
- Starting a new thread when switching topics is primarily about quality, secondarily about cost

**Day 8: What Is a Hallucination?**
- A hallucination is a confident, fluent output not grounded in truth
- Models are trained to produce the most probable continuation of text, not necessarily the most truthful
- This often occurs with insufficient context — filling a gap based on patterns, not real data
- This is why much of the focus is on building internal knowledge systems
- Also watch for: out-of-date responses (verify anything time-sensitive against the cutoff) and irrelevant responses (if Sierra misses the point, add more context)
- Always review outputs before sending to clients — fluent does not mean accurate

---

### WEEK 3 (April 14-18): Prompting & How Sierra Works
*5 days: Monday - Friday*

**Day 9: Prompting Fundamentals**
- What makes a prompt strong: role, task, context, format
- Specific vs. vague — the single biggest lever you have
- Prompting is iterative — one exchange rarely gets you there; refine and build
- Bad vs. good prompt examples in an ABS context

**Day 10: Advanced Prompting Techniques**
- Voice-to-text: speak your prompt — faster, more natural, often more detailed
- Meta-prompting: ask Sierra to rewrite your rough idea as a clean, reusable prompt
- Know when to continue a thread vs. start fresh — scattered threads produce scattered answers
- Iterative loop: prompt → review output → refine the ask → repeat

**Day 11: The Context Window — What Sierra Sees**
- The LLM only processes what's in its context window at the moment of each response
- What gets injected: your prompt, system prompt, memories, workspace context, retrieved chunks, conversation history
- Persistent vs. ephemeral: memories and workspace context persist across threads; thread content does not
- Personal memories apply in standard Sierra threads; inside a workspace, workspace memories replace them — personal memories do not carry over into workspaces and vice versa
- This is the mental model behind all of Sierra's features — workspaces, memories, and retrieval tools all exist to put the right information in front of the model automatically

**Day 12: How Sierra Retrieves Information (RAG)**
- RAG in practice: your query → semantic search → relevant chunks retrieved → added to context → model responds
- The model only reasons over what gets retrieved — not the entire knowledge base
- Specific queries = better retrieval = better answers (same principle as Day 9 prompting)
- RAG is the mechanism behind file uploads, workspace files, Plato, and other knowledge tools — same pipeline, different sources

**Day 13: Working with Files — Part 1**
- Uploading documents into a thread: Sierra converts to text → chunks → vector store → retrieves via RAG (Day 12 pipeline applied)
- File-friendly formats: text-based PDFs, Word, Excel — structured, selectable text works best
- File-unfriendly: scanned documents, image-heavy PDFs, complex nested tables — extraction quality drops significantly
- Thread attachments vs. workspace files: isolated to one thread vs. persistent and shared — know which to use when

---

### WEEK 4 (April 21-25): Knowledge Systems & Tools
*5 days: Monday - Friday*

**Day 14: Working with Files — Part 2**
- Getting structured output from files: summaries, extracted data, reformatted content, comparisons
- If output format matters, give Sierra a template — paste an example and ask it to match the structure
- LLM cleanup: Sierra can reformat and fix messy text extracted from converted or scanned documents
- What Sierra cannot do: produce formatted Word/PDF files, retain brand styling, generate charts, pixel-perfect output
- Practical habit: Sierra gives you the content — you apply the final formatting in Word or PowerPoint

**Day 15: Workspaces — Part 1**
- A workspace is a persistent, shared context environment for teams — set it up once, every thread inherits it
- Settings: manage which users have access to the workspace
- Workspace Context: written into the system prompt for every thread — purpose, standards, definitions, standing instructions; always-on, applies universally
- Workspace Memories: shared memories injected into every thread via the system prompt — no retrieval needed; used for shared project context, team preferences, and workspace-specific standards; accessible to all users in the workspace
- Workspace Files: documents loaded via RAG, searchable by any thread and any user — explicitly mention file names in prompts to improve retrieval
- Key distinction: personal memories do not apply inside workspaces; workspace memories do not carry over to regular Sierra chats — they are separate systems
- Context is for general background; specific repeatable activities belong in Task Modes, not here

**Day 16: Workspaces — Part 2**
- Task Modes: reusable step-by-step instructions for specific, repeatable workflows — invoked by users when needed
- What a Task Mode can include: steps, which workspace files to reference, which tools to activate, output format requirements
- Rule of thumb: general background → Workspace Context / specific repeatable activity → Task Mode
- Sierra follows the defined workflow consistently every time a Task Mode is invoked
- Real examples: survey report review, client summary generation, compliance assessment, meeting notes

**Day 17: Plato & eCFR — ABS & Regulatory Knowledge Bases — Part 1**
- Plato is ABS's internal knowledge base — procedures, standards, technical guidance, company-specific reference material *(currently in preview; may not be available to all users yet)*
- eCFR (Electronic Code of Federal Regulations) is a curated index of US federal regulations — 46 CFR (shipping), 33 CFR (Coast Guard), and others directly relevant to ABS work *(also in preview)*
- Both work via RAG (same pipeline as Days 12-13) — Sierra searches and retrieves relevant chunks to reason over
- When to use Plato: ABS procedures, technical standards, compliance guidance, anything internal and authoritative
- When to use eCFR: US federal maritime and safety regulations, CFR cross-references, regulatory research
- Specific queries get better retrieval — same principle applies to both

**Day 18: Plato & eCFR — Part 2**
- Writing better queries for both: use specific rule numbers, procedure names, document titles, regulatory citations — vague = poor retrieval
- Combining Plato or eCFR with file uploads: attach a project document and ask Sierra to cross-reference against ABS standards or federal regulations
- For compliance work: check whether a process or approach aligns with a specific ABS standard or CFR requirement
- Plato and eCFR have limits — if Sierra can't find something, it will say so; that's the system working correctly
- Workflow tip: Plato + eCFR + files + a focused prompt covers both internal standards and external regulatory requirements in a single thread

---

### WEEK 5 (April 28 - May 1): Putting It Together
*4 days: Monday - Thursday*

**Day 19: SkillShare & HR Tools**
- SkillShare: Sierra can search ABS Group's skillset and resume database — use it when you need a human expert, not just an AI answer *(ABS Group employees only; not available to Bureau or Wavesight by default)*
- HR Tool: Sierra has access to ABS HR knowledge — policies, benefits, procedures, specific to company (Bureau/Group/Wavesight) and country — ask naturally, it retrieves accurately
- Both are retrieval tools — same RAG pipeline as Plato and workspace files, different knowledge source
- SkillShare is for finding people; HR is for finding policy — know which one to reach for

**Day 20: Real Workflow — Writing & Document Work**
- End-to-end walkthrough: upload the file → set context → prompt with a specific ask → refine output
- Use workspace context or memories so Sierra already knows your audience, standards, and style
- Use a Task Mode for repeatable document tasks — review process, summary format, client deliverable template
- Always review outputs before sending — Sierra is your first draft engine, not your final editor

**Day 21: Real Workflow — Research & Analysis**
- End-to-end walkthrough: Plato for internal standards → web search for current external info → files for project specifics → synthesize
- Ask Sierra to cite sources and explain its reasoning — easier to verify and spot hallucinations
- Hallucinations are most likely near the edges: obscure topics, recent events, highly specific technical details — always cross-check these
- Build a repeatable research workflow in a workspace: load relevant files, set context, create a Task Mode for the research process

**Day 22: What You Now Know — Wrap-Up & Certification Prep**
- The mental model you've built: model limits → context → retrieval (RAG) → prompting → workspaces → full workflows
- The habits that matter: focused threads, specific queries, provide context before you prompt, verify before you send
- Common mistakes to avoid going forward
- What's next: certification exam through iAchieve — and then actually using this every day

---

## Course Structure

**Format:** 1 module per day, 22 business days total
- 5-minute instructional video
- 1 hands-on exercise
- Final assessment at completion

**Schedule:** April 1 - May 1, 2026
- Week 1: 3 days (Wed-Fri)
- Weeks 2-4: 5 days each (Mon-Fri)
- Week 5: 4 days (Mon-Thu)