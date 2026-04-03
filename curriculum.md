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
- Vague in = vague out — specificity is the single biggest lever
- Four ingredients: Role (what Sierra is), Task (what you want), Context (the raw material), Format (how to respond)
- Your first prompt is a starting point — when Sierra misses, tell it what was wrong and add what it was missing
- When a thread goes sideways, start fresh — don't fight it
- Meta-prompt shortcut: ask Sierra to write the prompt for you from a rough description

**Day 10: Structuring Complex Tasks**
- You are the SME — Sierra does not know your process, project, or professional judgment; your job is to explain the reasoning sequence a competent person would follow
- Give it a reasoning sequence, not just a question: specify structure — criteria, assessment, uncertainty, conclusion — makes responses easier to review and push back on
- Break it into steps the way you'd brief a junior analyst: sequential prompts let you review each step before the next
- Tell it what a senior person would watch out for: be explicit about evaluation criteria, constraints, and where to flag uncertainty
- You're not just asking for output — you're directing how Sierra thinks through the problem

**Day 11: Context Engineering**
- The context window is everything the model processes at once — prompt, thread history, tool responses, system prompt, memories, workspace instructions
- Left side (per-thread): prompt, thread history, past tool responses
- Right side (persistent, automatic): system prompt, memories, style, user info
- Top (workspace-level): workspace instructions — shared context that applies across threads in that workspace
- Context shifts depending on where you're working — in a workspace, workspace-level instructions and shared context shape every thread automatically
- Context engineering = being deliberate about what fills that window; prompting controls the left side, memories and workspaces engineer the right, RAG fills it with retrieved knowledge

**Day 12: Working with Files — Part 1**
- Sierra does not read the whole file into the chat — it extracts text, indexes it in retrievable sections, and retrieves the most relevant passages based on your query
- Specific questions get better results — retrieval is query-driven, not whole-document
- The quality of retrieval depends on the quality of the source — clearly formatted, text-based documents tend to extract more reliably; extraction capabilities are actively improving
- Thread attachments are temporary and isolated; workspace files are persistent and shared across all users

**Day 13: Working with Files — Part 2**
- Getting structured output: summaries, extracted data, reformatted content, comparisons
- Give Sierra a template — paste an example of what you want and ask it to match the structure
- Ask targeted questions rather than "summarize everything" — specific asks surface specific content
- Sierra gives you content to work with, not finished deliverables — apply final formatting, branding, and production in your document tools
- Capabilities are actively expanding; the constant habit is: direct the output, then shape it into the final form yourself

---

### WEEK 4 (April 21-25): Knowledge Systems & Tools
*5 days: Monday - Friday*

**Day 14: Workspaces — Part 1**
- A workspace is a shared environment where threads can access common instructions, context, and files — configure once, work in that workspace benefits from it
- Workspace Context: standing guidance and background knowledge that applies across threads in the workspace
- Workspace Memories: durable shared information available to all threads and users without retrieval
- Workspace Files: searchable knowledge sources available across threads — mention file names in prompts to improve retrieval
- Context works differently depending on where you are — in a workspace, shared workspace-level context shapes every thread automatically

**Day 15: Workspaces — Part 2**
- Task Modes: reusable step-by-step instructions for specific, repeatable workflows — invoked by users when needed
- What a Task Mode can include: steps, which workspace files to reference, which tools to activate, output format requirements
- Rule of thumb: general background → Workspace Context / specific repeatable activity → Task Mode
- Task Modes help Sierra follow a more consistent workflow for repeatable tasks
- Real examples: survey report review, client summary generation, compliance assessment, meeting notes

**Day 16: Plato — Sierra's Maritime Research Mode**
- Plato is a specialized Sierra mode for maritime rules and regulatory research — not a general knowledge base *(in preview; may not be available to all users)*
- Built for surveyors, engineers, and auditors researching Class rules, IMO compliance, and survey procedures
- Knowledge sources *(expanding as Plato develops):* ABS Rules & Guides, IMO/IACS publications (partial), ABS internal survey procedures and job aids, and eCFR (Titles 33 and 46)
- Plato shows its reasoning and says when content isn't indexed rather than guessing

**Day 17: Using Plato Effectively**
- Be specific: state vessel type, rule set reference, Part/Chapter, or survey stage — vague queries produce vague results
- Search rule first, then procedure: find the Class requirement first, then search ETQ for the corresponding survey procedure or job aid
- Plato is honest about gaps — if content isn't indexed, verify through official sources or consult an ABS SME
- Combine with file uploads: attach a project document, ask Plato to cross-reference against applicable Class rules or regulations
- Outside Plato mode: standalone eCFR tool in main Sierra chat handles quick regulatory lookups without entering Plato

**Day 18: SkillShare & HR Tools**
- SkillShare: Sierra can search ABS Group's expertise directory — use when you need a human expert, not just an AI answer *(ABS Group employees only)*
- HR Tool: Sierra has access to ABS HR knowledge — policies, benefits, procedures, specific to company and country
- Both are retrieval tools — same pipeline as Plato and workspace files, different knowledge source
- SkillShare is for finding people; HR is for finding policy

---

### WEEK 5 (April 28 - May 1): Putting It Together
*4 days: Monday - Thursday*

**Day 19: Real Workflow — Writing & Document Work**
- End-to-end walkthrough: upload the file → set context → prompt with a specific ask → refine output
- Use workspace context or memories so Sierra already knows your audience, standards, and style
- Use a Task Mode for repeatable document tasks — review process, summary format, client deliverable template
- Always review outputs before sending — Sierra is your first draft engine, not your final editor

**Day 20: Real Workflow — Research & Analysis**
- End-to-end walkthrough: a typical research stack — Plato for ABS rules → eCFR for federal regulations → web search for current external info → files for project specifics → synthesize; use the tools available and relevant, not all at once
- Ask Sierra to cite sources, state its assumptions, and flag what may need verification — makes gaps and errors easier to spot
- Hallucinations are most likely near the edges: obscure topics, recent events, highly specific technical details — always cross-check against authoritative sources
- Build a repeatable research workflow in a workspace: load relevant files, set context, create a Task Mode for the research process

**Day 21: What You Now Know — Wrap-Up & Certification Prep**
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