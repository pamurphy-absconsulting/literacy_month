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
- Four ingredients: Role (the angle of approach — "you are a technical reviewer"), Task (explicit instruction — the more specific and example-backed, the better), Context (background information and raw material the model couldn't know on its own), Format (output specification: bullets, table, one page, plain language)
- Iterative by design — unlike a search engine, which ends at the first result, the conversation continues; build on what it returns until you get what you want
- Your first prompt is a starting point — when Sierra misses, tell it what was wrong and add what it was missing; when a thread goes sideways entirely, start fresh
- Meta-prompt shortcut: ask Sierra to write the prompt for you — describe the task rough, stream of consciousness, and ask it to structure a clean prompt from what you provided

**Day 10: Structuring Complex Tasks**
- You are the SME — Sierra does not know your process, project, client, or professional judgment; your job is to direct it, not hope it figures it out
- Don't throw a complex problem at it all at once — break it into sequential steps and guide it through
- One big prompt = one shot; sequential steps = you review each output before the next starts, catching errors early
- You decide the sequence and what good output looks like at each stage
- Once a workflow is dialed in, ask Sierra to build a reusable prompt from the conversation history — save it as a starting point for next time

**Day 11: Structuring Prompts for Data Extraction**
- What you are leveraging here is processing power, not reasoning — the model's ability to read and ingest massive amounts of information and pull out key data at scale; the goal is deterministic output, not brainstorming
- The organizing principle: reduce the model's cognitive load — every ambiguity you leave unresolved is left to the model to fill; the less it has to figure out, the more it focuses on the extraction
- Pre-prompt checklist: Field (what am I extracting?), Definition (what exactly counts?), Exclusions (what does not count?), Location (where in the document is it found?), Decision rules (if/then logic for ambiguous cases), Evidence (what proof should Sierra return?), Output format (how should results be structured?)
- Encode the structure — map your checklist to the document before you write the prompt; name the section, heading, or clause where each field lives
- Phased extraction: Pass 1 — pull high-level anchors (party names, vessel type, applicable schedule); Pass 2 — inject those anchors back into the prompt with the same file and precise instruction for granular fields; the second pass is grounded, not guessing
- ABS example: Pass 1 — "Identify the contracting party, contract type, and which pricing schedule applies." Pass 2 — "Under Schedule B as confirmed above, extract the day-rate for each vessel class as defined in Clause 4. List exclusions. Return one row per vessel class with: vessel class | day-rate | applicable clause | exclusions."

**Day 12: Working with Files — Part 1**
- Common misconceptions: uploaded files are not added to Sierra's internal knowledge; the entire file is not dumped into the context window on every message
- What actually happens: file is converted to raw text and indexed into a separate store; when you send a query, Sierra pulls the most relevant sections into context and sends those — along with your question — to the model; different queries surface different sections
- Preview is available before attaching — you can inspect what the conversion produced before it hits the thread
- Source quality matters — clean, structured text converts and retrieves more reliably; complex, image-heavy files produce less reliable conversions
- Thread attachments are temporary and isolated; workspace files are persistent and shared across all users

**Day 13: Working with Files — Part 2**
- No amount of prompting compensates for data that wasn't read in correctly — input integrity comes before prompt quality
- What to consider before attaching: Is it text-based or image-heavy? Is it a scanned PDF or a DOCX? Tabular or diagram-heavy? These determine conversion quality
- How conversion works: images and diagrams are converted to text descriptions; complexity affects how accurate and complete that description will be
- Fast vs. full conversion: by default Sierra uses fast (strips to raw text, maintains general structure); switch to full for scanned or image-heavy files — full runs OCR first and produces a more complete, structured output
- Preview the conversion — check it before relying on it; if the conversion is wrong, the prompt won't fix it
- The default troubleshooting instinct should be the same as a calculator: if the output is wrong, check what was keyed in — the problem is usually in the data ingested, not the model

---

### WEEK 4 (April 21-25): Knowledge Systems & Tools
*5 days: Monday - Friday*

**Day 14: Memories**
- Memories are persistent context — injected into every thread automatically, no retyping required
- What to put in them: role and specialization; operational context (industry, region, team, organization); preferences (writing style, output format)
- Set them by telling Sierra directly ("Remember that I...") or through profile settings
- Save key context once — automatically included in every thread; the model output is grounded and more tailored before you type a word

**Day 15: Workspaces**
- A workspace is a collaborative environment where multiple members can access common instructions, context, and files
- Workspace Context: background knowledge that applies across all threads in the workspace
- Workspace Memories: shared information relevant to the workspace — can be dynamically added by each member
- Workspace Files: searchable/retrievable knowledge sources available across threads and members — mention file names in prompts to improve retrieval
- Workspace context is shared and persistent; thread content is yours and temporary

**Day 16: Workspace Task Modes**
- Task Modes: reusable step-by-step instructions for specific, repeatable workflows — invoked by users when needed
- What a Task Mode can include: steps, which workspace files to reference, which tools to activate, output format requirements
- Rule of thumb: general background → Workspace Context / specific repeatable activity → Task Mode
- Real examples: emergency response validation, incident root cause analysis, regulatory compliance check, flag state compliance
- Context + Memories are always on for everything; Task Modes are invoked when needed for specific jobs

**Day 17: Plato — Sierra's Maritime Research Mode**
- Plato is a specialized Sierra mode for maritime rules and regulatory research — not a general knowledge base *(in preview; may not be available to all users)*
- Built for surveyors, engineers, and auditors researching Class rules, IMO compliance, and survey procedures
- Knowledge sources *(expanding as Plato develops):* ABS Rules & Guides, IMO/IACS publications (partial), ABS internal survey procedures and job aids, and eCFR (Titles 33 and 46)
- Plato shows its reasoning and says when content isn't indexed rather than guessing

**Day 18: Using Plato Effectively**
- Be specific: state vessel type, rule set reference, Part/Chapter, or survey stage — vague queries produce vague results
- Search rule first, then procedure: find the Class requirement first, then search ETQ for the corresponding survey procedure or job aid
- Plato is honest about gaps — if content isn't indexed, verify through official sources or consult an ABS SME
- Combine with file uploads: attach a project document, ask Plato to cross-reference against applicable Class rules or regulations
- Outside Plato mode: standalone eCFR tool in main Sierra chat handles quick regulatory lookups without entering Plato

---

### WEEK 5 (April 28 - May 1): Putting It Together
*4 days: Monday - Thursday*

**Day 19: SkillShare & HR Tools**
- SkillShare: Sierra can search ABS Group's expertise directory — use when you need a human expert, not just an AI answer *(ABS Group employees only)*
- HR Tool: Sierra has access to ABS HR knowledge — policies, benefits, procedures, specific to company and country
- Both are retrieval tools — same pipeline as Plato and workspace files, different knowledge source
- SkillShare is for finding people; HR is for finding policy

**Day 20: Real Workflow — Writing & Document Work**
- End-to-end walkthrough: upload the file → set context → prompt with a specific ask → refine output
- Use workspace context or memories so Sierra already knows your audience, standards, and style
- Use a Task Mode for repeatable document tasks — review process, summary format, client deliverable template
- Always review outputs before sending — Sierra is your first draft engine, not your final editor

**Day 21: Real Workflow — Research & Analysis**
- End-to-end walkthrough: a typical research stack — Plato for ABS rules → eCFR for federal regulations → web search for current external info → files for project specifics → synthesize; use the tools available and relevant, not all at once
- Ask Sierra to cite sources, state its assumptions, and flag what may need verification — makes gaps and errors easier to spot
- Hallucinations are most likely near the edges: obscure topics, recent events, highly specific technical details — always cross-check against authoritative sources
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