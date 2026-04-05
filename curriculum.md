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

**Day 6: SIERRA's Tools for Adding Context**
- Sierra is not a model — it's a platform with secure access to various LLMs and a set of tools built around them
- The models were trained on public data; ABS-specific work — projects, rules, client data, procedures — is not in there by default
- Sierra has three tools to bring in what the model doesn't know: web search (current/external info), file attachments (documents you upload), and knowledge repositories (CoE-built data sets Sierra searches automatically)
- Example: HR vacation policy — the model has no idea; Sierra retrieves it from an ABS-built knowledge repository and responds correctly
- In all three cases, the model only processes what's in its context window — these tools exist to make sure the right information gets there

**Day 7: Tokens & Context Windows**
- The model only processes what's in its context window — nothing from other threads, nothing not explicitly provided or retrieved
- Context window = working memory: everything the model can hold and process at once — large, but not infinite
- Tokens are the unit of measurement: roughly 666 tokens per page
- The quality constraint: the model processes everything in the window on every message — irrelevant content degrades output quality, not just efficiency
- Focused threads get better results: start a new chat when switching topics, keep threads tight and on one subject
- Failure mode: long conversations push earlier context out of the window — the model loses information it once had; that sets up Day 8

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
- Four ingredients: Role (the angle of approach — "you are a technical reviewer"), Task (explicit instruction on what to do), Context (background information and raw material), Format (how to structure the output)
- Your first prompt is a starting point — when Sierra misses, tell it what was wrong and add what it was missing
- When a thread goes sideways, start fresh — don't fight it
- Meta-prompt shortcut: ask Sierra to write the prompt for you from a rough description

**Day 10: Structuring Complex Tasks**
- You are the SME — Sierra does not know your process, project, client, or professional judgment; your job is to direct it, not hope it figures it out
- Don't throw a complex problem at it all at once — break it into sequential steps and guide it through
- One big prompt = one shot; sequential steps = you review each output before the next starts, catching errors early
- You decide the sequence and what good output looks like at each stage
- Once a workflow is dialed in, ask Sierra to build a reusable prompt from the conversation history — save it as a starting point for next time

**Day 11: Memories & Customization**
- Memories are persistent context that carry into every thread automatically — no retyping required
- What to put in them: role and specialization, typical audience, response preferences, team/group context
- Personal memories follow you across all standard threads; workspace memories are shared across a team
- Set memories once, stop repeating yourself every thread — the response improves before you type a word

**Day 12: Working with Files — Part 1**
- Sierra does not read the whole file into the chat — it extracts text, indexes it in retrievable sections, and retrieves the most relevant passages based on your query
- Your query drives what gets retrieved — vague questions surface vague content; specific questions surface specific content
- Reference sections, topics, or names directly to improve retrieval; if Sierra misses something, restate with more specificity or quote a term from the document
- The quality of retrieval depends on the quality of the source — clearly formatted, text-based documents retrieve more reliably
- Thread attachments are temporary and isolated; workspace files are persistent and shared across all users

**Day 13: Working with Files — Part 2**
- Getting structured output: give Sierra a template — paste an example and say "match this structure"; don't describe format in the abstract when you can show it
- Break it into steps: extract first, then rank, then write — don't ask for the finished deliverable in one shot
- Be explicit about audience and purpose; ask it to flag uncertainty and assumptions
- If the first output misses: tell it what was wrong rather than starting over — point it back to the specific section
- Sierra gives you content to work with, not finished deliverables — direct the output, then shape it into final form yourself

---

### WEEK 4 (April 21-25): Knowledge Systems & Tools
*5 days: Monday - Friday*

**Day 14: Workspaces — Part 1**
- Context engineering: every response is shaped by more than your prompt — prompt, thread history, memories, workspace instructions, and retrieved knowledge all feed into what the model sees; workspaces are how you engineer the persistent, shared side of that at a team level
- A workspace is a shared environment where threads can access common instructions, context, and files — configure once, every thread in that workspace benefits
- Workspace Context: standing guidance and background knowledge that applies across all threads in the workspace
- Workspace Memories: durable shared information available to all threads and users without retrieval
- Workspace Files: searchable knowledge sources available across threads — mention file names in prompts to improve retrieval

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