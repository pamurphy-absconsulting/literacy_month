# SIERRA Literacy Month — Study Guide
*Certification Quiz Prep | 22 Days*

---

## Day 1 — Why SIERRA

**Know these ideas**
- SIERRA is not its own AI model — it is a secure wrapper that provides access to frontier models (ChatGPT, Claude, Grok) hosted within ABS's Azure environment
- The primary reason SIERRA exists is data security: files and conversations stay within ABS's infrastructure and are not used to train external models
- Using commercial AI tools directly (ChatGPT.com, Claude.ai) risks data leakage — SIERRA prevents that

**Work application**
- Be ready to explain SIERRA in one sentence to a colleague who hasn't used it
- Know why ABS requires SIERRA rather than allowing direct use of commercial tools

---

## Day 2 — Privacy, Security & Data Governance

**Know these ideas**
- Three security layers build upward: **Azure infrastructure → app design and data governance → policy compliance**
- When SIERRA performs a web search, only targeted keyword parameters are sent to the internet — not your conversation or uploaded files
- Client contractual terms that prohibit AI usage **override the ABS data policy**, even on SIERRA

**Work application**
- Be able to explain the difference between "generally allowed in SIERRA" and "still not allowed because of client contract terms"
- Know what happens to your data when SIERRA runs a web search

---

## Day 3 — What Are Large Language Models?

**Know these ideas**
- An LLM is a **statistical text predictor** — at its core, it predicts the most likely continuation of input text
- It is not retrieving stored facts from a database, and it does not "understand" in a human sense
- Individual words in a prompt can meaningfully shift the output — wording matters
- Different models handle the same prompt differently

**Work application**
- Practice explaining why people call an LLM a "text calculator"
- Be able to explain how small prompt changes can change the response

---

## Day 4 — What the Model Knows

**Know these ideas**
- Models were trained on public internet text — they have broad general knowledge up to a training cutoff date
- **ABS internal data was never public — it is not in any model's training data**
- The model does not automatically know: internal ABS information, HR policies, recent events, live operational data, or project/client-specific material
- Disable external tools and the model cannot reliably answer any of those categories

**Work application**
- Be ready to distinguish between what a model may know from training versus what must be brought in through files, web search, or a repository
- Know why internal ABS tasks almost always require the user to supply source material

---

## Day 5 — Context

**Know these ideas**
- Context includes: **your prompt, the full conversation history, and any uploaded files or tool results**
- The model is static — it does not learn from your chat or update between sessions
- Each time you send a message, the model reprocesses all available context from scratch
- Think of SIERRA as a reasoning engine: **you supply the raw materials (context) it reasons over** — the quality of the output depends entirely on the quality of what you put in
- Better context produces better, more grounded output

**Work application**
- Be able to define context in one sentence
- Understand that your role is active, not passive — you control what the model has to work with

---

## Day 6 — SIERRA's Tools for Adding Context

**Know these ideas**
- SIERRA is a platform, not just a model — it has tools that bring external information into the context window
- Three main tools: **file attachments, web search, and ABS-curated knowledge repositories**
- The HR policy tool returns accurate answers because ABS built an internal knowledge repository — the base model was never trained on that information
- **Web search must be explicitly requested** — SIERRA does not run it automatically

**Work application**
- Be ready to explain why "SIERRA is a platform" is more accurate than "SIERRA is an AI"
- Know when to ask explicitly for web search rather than assuming it runs on its own

---

## Day 7 — Context Windows

**Know these ideas**
- The context window is the model's working memory — large but not infinite
- One page of text ≈ **650 tokens**
- As a thread grows (longer conversation, file uploads, web results), earlier content can be cut off from the context window
- When key earlier content is gone, the model falls back on statistical patterns rather than your actual document — this is a leading cause of hallucinations in long threads

**Work application**
- Know why focused threads usually outperform long, sprawling ones
- Be prepared to explain what happens when important earlier content is no longer available in the context window

---

## Day 8 — Hallucinations

**Know these ideas**
- A hallucination is **confident, fluent output that is factually wrong** — the model is not lying, it is pattern-completing
- Polished, well-formatted writing is not a signal of accuracy
- Hallucinations are harder to detect without domain expertise in the subject
- The risk is highest when the model lacks sufficient context, the thread is very long, or the question is at the edge of training knowledge

**Work application**
- Be able to explain why a smooth-sounding answer can still be wrong
- Know why verification is required before submitting Sierra output in client deliverables

---

## Day 9 — Prompting Fundamentals

**Know these ideas**
- The four components of a well-structured prompt: **Role, Task, Context, Format**
- Prompting is iterative — your first message is a starting point, not a final answer
- SIERRA is fundamentally different from a search engine: it allows back-and-forth refinement
- The highest-impact prompting approach: **ask SIERRA to write the prompt for you** from a rough, plain-language description of what you need

**Work application**
- Practice turning a vague instruction into a structured prompt using the four components
- Be able to explain what each component contributes

---

## Day 10 — Structuring Complex Tasks

**Know these ideas**
- The most common mistake: asking for the final deliverable without completing upstream steps first
- Break complex tasks into sequential steps and review each output before moving on
- After a successful multi-step workflow, ask SIERRA to **produce a reusable prompt from the full conversation** — this makes the workflow repeatable
- You remain the subject matter expert; SIERRA supports execution

**Work application**
- Be ready to explain why one large prompt is often worse than a staged workflow
- Know how to convert a completed workflow into something reusable

---

## Day 11 — Structuring Prompts for Data Extraction

**Know these ideas**
- Before writing the prompt, define: **Field → Definition → Exclusions → Location → Decision rules → Evidence → Output format**
- **Evidence** means asking the model to return a justification (exact quote, clause reference) alongside each extracted value — this makes output verifiable
- Defining the output format reduces the model's cognitive load so it can focus on precise extraction
- **Phased extraction**: Pass 1 pulls high-level anchors; Pass 2 injects those confirmed anchors and goes granular — this grounds the model before the harder extraction

**Work application**
- Be able to explain why extraction quality improves when rules are defined before the prompt is written
- Know what "evidence" means in an extraction context and why it matters for review

---

## Day 12 — Working with Files, Part 1

**Know these ideas**
- File processing flow: **upload → convert to raw text → index into a vector store → query-based retrieval into context window**
- SIERRA does not read or "know" the whole file — it surfaces relevant sections based on what you ask
- Specific, targeted queries retrieve better content than vague ones
- **Files do not persist across threads** — a file uploaded in one thread is not available in a new one

**Work application**
- Be ready to explain why "I uploaded it" is not the same as "the model now knows all of it"
- Know what to expect when you ask a vague question about a file versus a specific one

---

## Day 13 — Working with Files, Part 2

**Know these ideas**
- Input quality determines output quality — if the file conversion is poor, the answer will be poor
- **First thing to check when output seems wrong: preview the file conversion**, not the prompt
- Two conversion modes:
  - **Fast**: strips to raw text, preserves general structure (default)
  - **Full**: runs OCR, reads images and scanned content, produces more complete output
- Use Full conversion for scanned PDFs, image-heavy files, or documents with embedded diagrams

**Work application**
- Know when to switch from Fast to Full conversion and why it matters
- Apply the calculator rule: if the output is wrong, check what you put in

---

## Day 14 — Memories

**Know these ideas**
- Memories are **persistent context automatically injected into every chat** — set once, always available without re-entering
- Best content for personal memories: stable information about you — role, specialization, regional context, preferred output format
- Do not store project-specific or time-sensitive content in memories — that belongs in workspace memories or uploaded files

**Work application**
- Be able to explain the difference between a cold thread and a memories-enabled thread
- Know what belongs in personal memory versus what belongs elsewhere

---

## Day 15 — Workspaces

**Know these ideas**
- **Thread content** = private, temporary, belongs to the individual user
- **Workspace content** = shared and persistent for all members: context, memories, files, task modes
- A file uploaded to a workspace's Files tab is accessible to all members in their own chats — no re-upload needed
- Workspace context is background orientation that applies to every thread in the workspace automatically

**Work application**
- Be ready to explain the difference between thread content and workspace content
- Know why a shared workspace eliminates repetitive setup across a team

---

## Day 16 — Workspace Task Modes

**Know these ideas**
- **Workspace context and memories** = always-on background, applies to all threads
- **Task modes** = invoked when needed, for specific repeatable workflows
- Rule of thumb: background and orientation → workspace context; specific step-by-step instructions → task mode
- If you've written the same multi-step prompt more than twice, it probably belongs in a task mode

**Work application**
- Be prepared to distinguish between general workspace context and a specific repeatable instruction set
- Know the types of work that benefit most from task modes: compliance checks, document reviews, proposal generation

---

## Day 17 — Workspace Walkthrough

**Know these ideas**
- Five workspace tabs: **Settings, Context, Files, Task Modes, Memories**
- **Personal memories** = about you (role, preferences, domain) — visible only to you, across all chats
- **Workspace memories** = about the project or client (scope, stakeholders, requirements) — shared with all workspace members
- When in doubt: if it describes you → personal memory; if it describes the work → workspace memory

**Work application**
- Be ready to walk through what each workspace tab is for
- Know the distinction between personal and workspace memories and be able to give an example of each

---

## Day 18 — Building a Workspace

**Know these ideas**
- Start in a **regular chat**, not inside the workspace — use SIERRA to analyze sample materials and draft the context and task mode instructions before moving them in
- Frontier models have no inherent knowledge of what a SIERRA workspace is — its structure must be explained explicitly
- Analyze sample documents first: what is consistent, what varies, what the key variables are — build a confirmed understanding before constructing workspace components
- Design task modes to **pause and confirm key variables with the user** before generating output — this is what "bringing a human into the loop" means

**Work application**
- Be ready to explain why you start in a regular chat rather than building directly inside the workspace
- Know why the task mode design includes a variable confirmation step before output is generated

---

## Day 19 — Plato Demo

**Know these ideas**
- Plato is SIERRA's maritime rules tool — it synthesizes across **multiple rule sections** to address complex, scenario-based questions
- Ask Plato the way you'd ask a colleague — compound, multi-part questions in a single query are appropriate
- When a follow-up introduces new scenario context (e.g. a prior finding of substantial corrosion in a ballast tank), Plato **connects requirements from two different rule areas** and builds a specific, actionable follow-up plan — including things like close-up survey scope and thickness measurement expectations
- Always click through citations to verify the rule reference is correct

**Work application**
- Know when Plato is the right tool and how to frame questions for best results
- Understand that Plato's value is scenario synthesis: it doesn't just cite a rule, it connects multiple sub-requirements into a concrete plan

---

## Day 20 — Environmental Plan Review Workspace

**Know these ideas**
- One workspace can support multiple document types through separate task modes — you don't need a new workspace per task type
- Shared context and style live at the workspace level; specific review instructions live in individual task modes
- Build task mode instructions by pasting existing review criteria into a regular chat and asking SIERRA to convert them — you don't write them from scratch
- Good review output includes: **yes/no flags, findings, source references within the document, and a reviewer check column** — this is a deliberate human oversight mechanism

**Work application**
- Be ready to explain the one-workspace, multiple-task-modes design principle
- Know what a well-structured review output looks like and why the reviewer check column matters

---

## Day 21 — Web Search & Deep Research

**Know these ideas**
- **Web search**: runs multiple targeted searches, synthesizes results into a **structured comparison table or summary with source citations** — faster, best for current information and multi-topic comparisons (e.g. comparing regulatory timelines across three fuel types)
- **Deep research**: conducts a more comprehensive multi-source investigation and generates a detailed, downloadable technical report — better for higher-stakes or more complex questions
- Both tools link to sources — verifying citations before using the output is always required
- Sierra is not the final authority on external information; it synthesizes and cites, you verify

**Work application**
- Be ready to choose between web search and deep research based on the depth and stakes of the question
- Know that web search is the right tool when you need a structured multi-dimension comparison across several topics or entities — it runs multiple searches and synthesizes them, not just one lookup
- Know that source verification is required regardless of which tool is used

---

## Day 22 — HR Policy Repository

**Know these ideas**
- SIERRA automatically identifies your **entity and home country** from your profile and applies the correct policy — you do not need to specify it
- Two employees in different countries asking the same question receive different, personalized answers
- If a policy is not in the repository, SIERRA clearly states this and directs you to your HR business partner — it does not fill gaps with approximations or guesses

**Work application**
- Know what makes the HR repository different from simply uploading an HR document and asking a question
- Be able to explain what "safe failure" looks like when a policy is missing from the repository

---

## Things People Get Wrong

- **"SIERRA knows my file"** — It indexed it. Different questions surface different sections. Files don't persist across threads.
- **"Well-written = accurate"** — No. Verify before using in client deliverables.
- **"One long thread is fine"** — Long threads degrade quality. Start fresh when topics change.
- **"I need to specify my country for HR questions"** — SIERRA reads your profile automatically.
- **"I need to write workspace components from scratch"** — Use a regular chat to draft them.
- **"Web search runs automatically"** — You have to explicitly request it.
- **"Context and task modes are the same thing"** — Context is always on; task modes are invoked for specific jobs.
