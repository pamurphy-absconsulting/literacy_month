# SIERRA Literacy Month — Certification Quiz
*50 Questions | All 22 Days Covered*

---

## Instructions
Select the single best answer for each question. Questions test both conceptual understanding and applied judgment — not just definitions. At least one question covers each of the 22 days.

---

### Day 1 — Why Sierra

**Question 1.**
SIERRA is best described as which of the following?

A. A proprietary AI model trained exclusively on ABS data  
B. A secure wrapper that hosts various frontier models within an Azure environment  
C. A stand-alone chatbot with no connection to external models  
D. A fine-tuned version of GPT built by the ABS IT department

> **Answer: B** — SIERRA is not its own model; it provides secure access to frontier models hosted within a protected Azure environment.

---

**Question 2.**
The primary reason SIERRA is the only ABS-approved AI system — rather than ChatGPT, Claude, or Grok used directly — is:

A. It is faster than commercial alternatives  
B. It has a larger context window than ChatGPT  
C. It prevents data leakage by keeping uploaded files within ABS's secure environment  
D. It is less expensive than purchasing enterprise ChatGPT licenses

> **Answer: C** — Data leakage is the core concern. When using commercial tools directly, files and conversations may be used to train external models or shared with third parties. SIERRA keeps all data within ABS's secure environment.

---

### Day 2 — Privacy, Security & Data Governance

**Question 3.**
SIERRA's security framework is described as having three layers. Which of the following correctly orders them from *bottom to top*?

A. Policy compliance → app design → Azure infrastructure  
B. Azure infrastructure → app design and data governance → policy compliance  
C. App design → policy compliance → Azure infrastructure  
D. Azure infrastructure → policy compliance → app design

> **Answer: B** — The three layers build upward: Azure infrastructure at the base, then app design and data governance, then policy compliance at the top.

---

**Question 4.**
When SIERRA performs a web search, which of the following accurately describes what is sent to the internet?

A. The full contents of all uploaded files in the current thread  
B. The entire conversation history up to that point  
C. Targeted keyword parameters — typically just a handful of words  
D. A compressed summary of the user's last three messages

> **Answer: C** — Web search uses targeted keyword parameters and does not leak chat details or uploaded file content.

---

**Question 5.**
Under what specific circumstance does ABS's own SIERRA Data Policy get *superseded*?

A. When a government subpoena is issued  
B. When a client's contractual terms prohibit any AI usage  
C. When the user has completed SIERRA certification  
D. When the conversation is conducted inside a workspace

> **Answer: B** — Client contractual terms that prohibit AI usage override the ABS data policy, even on secure, ABS-hosted infrastructure.

---

### Day 3 — What Are Large Language Models?

**Question 6.**
At its most fundamental level, what is a large language model doing when it generates a response?

A. Searching a database for stored facts and retrieving them  
B. Translating your input into code and executing it  
C. Predicting the statistically most likely continuation of the input text  
D. Comparing your input against a curated knowledge graph

> **Answer: C** — An LLM is a text-completion and prediction engine operating on statistical relationships established during training.

---

**Question 7.**
A user experiments with SIERRA by regenerating the same response multiple times and making small word changes to the prompt — for example, swapping out the type of expert or deleting the phrase "most likely." What is the most important insight this kind of experiment is designed to surface?

A. That all models produce identical output for the same prompt  
B. That individual words in a prompt can meaningfully shift the model's output, and that different models handle the same prompt differently  
C. That the context window fills up faster with longer prompts  
D. That web search must be explicitly enabled for accurate answers

> **Answer: B** — Small prompt changes can noticeably shift outputs; swapping models reveals that different models behave differently with the same input.

---

### Day 4 — What the Model Knows

**Question 8.**
Which of the following categories of information would a frontier LLM be *least* likely to have based solely on its training data?

A. Historical geopolitical events  
B. General principles of thermodynamics  
C. ABS internal contract data and employee records  
D. Widely published scientific research

> **Answer: C** — Corporate IP and internal ABS information was never public and was therefore never part of any model's training data.

---

**Question 9.**
A user disables SIERRA's external tools and knowledge bases, then asks about ABS HR policies, recent news events, and the weather. SIERRA cannot answer any of these reliably. What does this demonstrate?

A. That SIERRA's memory feature is unreliable  
B. That SIERRA's base model knowledge alone cannot answer questions requiring internal ABS data, real-time events, or live data  
C. That context windows fill up quickly with web search results  
D. That workspaces are required for any HR-related queries

> **Answer: B** — Removing external tools reveals the model's knowledge gaps — it cannot answer those questions from training data alone.

---

### Day 5 — Context

**Question 10.**
Which of the following is the most precise definition of "context" as used throughout SIERRA training?

A. The model's training data  
B. The entirety of information provided to the model within a given interaction, including conversation history, prompts, and uploaded files  
C. Only the most recent message typed into the chat window  
D. The background knowledge the model learned during pre-training

> **Answer: B** — Context includes the full conversation history, the current prompt, and any file-derived information — not just the last message.

---

**Question 11.**
SIERRA's underlying model is compared to a "reasoning engine." What does this analogy most directly imply about the user's role?

A. The user must train the model before each session  
B. The user is responsible for providing the raw materials (context) the engine reasons over  
C. The user's role is passive once a good prompt is submitted  
D. The model improves through the interactions it has with the user

> **Answer: B** — The model is a static engine; the user controls the raw materials (context) it reasons over.

---

### Day 6 — SIERRA's Tools for Adding Context

**Question 12.**
A colleague asks Sierra about the ABS vacation policy without uploading anything or providing any instructions. Sierra is still able to return a useful, accurate answer. What best explains this?

A. The model was trained on ABS internal documentation  
B. Sierra retrieved that information from an ABS-curated knowledge repository built internally by the CoE  
C. Sierra performed an automatic web search for the policy  
D. The model inferred the policy from general HR best practices

> **Answer: B** — Sierra has access to an ABS-curated knowledge repository — this is distinct from the model's training data.

---

**Question 13.**
Regarding web search within Sierra: a user wants current regulatory information related to their project. What is the recommended practice?

A. Sierra will automatically trigger a web search whenever it detects outdated information, so no action is needed  
B. The user should explicitly instruct Sierra to run a web search, since it does not typically initiate one on its own  
C. Web search is disabled in Sierra for data security reasons  
D. The user should copy the regulatory text manually into the chat window instead

> **Answer: B** — Web search must be explicitly requested; Sierra does not automatically initiate searches on its own.

---

### Day 7 — Understanding Context Windows

**Question 14.**
Approximately how many tokens does one page of text represent?

A. 100  
B. 650  
C. 4,096  
D. 2,500

> **Answer: B** — One page of text is approximately 650 tokens.

---

**Question 15.**
A user introduces an important project document at the start of a long Sierra conversation. After many back-and-forth exchanges, additional file uploads, and web searches, they ask a question that references that early document. Sierra generates a confident but inaccurate answer that doesn't reflect the document at all. What most likely explains this?

A. Sierra does not support multi-turn conversations longer than 10 exchanges  
B. The document was in a format Sierra cannot read  
C. The earlier content was cut off from the context window as it filled up, so the model generated a response based on its general statistical patterns rather than the actual document  
D. The user would need to re-enter their credentials for Sierra to access the file again

> **Answer: C** — When the context window fills up, earlier content is cut off; the model then falls back on statistical patterns rather than grounded document content.

---

### Day 8 — Hallucinations

**Question 16.**
A user asks SIERRA a difficult question in their area of expertise and adds the instruction: "Do not search the internet to answer my question." The user then carefully evaluates the response. What behavior is this exercise specifically designed to surface?

A. That SIERRA refuses to answer without internet access  
B. That different models produce identical errors on the same question  
C. That the model can produce polished, fluent answers that are factually wrong — and that these may be hard to detect without domain expertise  
D. That SIERRA always discloses when it is uncertain

> **Answer: C** — The exercise surfaces hallucination behavior: fluent, confident output that may be wrong, and the importance of subject-matter verification.

---

**Question 17.**
A team member reviews a Sierra-generated response and finds it well-written, detailed, and professionally formatted. They submit it directly to a client. Why is this approach problematic?

A. Sierra outputs are always too long for client deliverables  
B. A polished, fluent response is not necessarily a true or accurate one — the model can generate confident incorrect output when it lacks sufficient grounding  
C. Sierra outputs are not formatted correctly for client use  
D. The team member should have used a different model

> **Answer: B** — Polished writing does not equal accuracy. Verification is always required before using Sierra output in client deliverables.

---

### Day 9 — Prompting Fundamentals

**Question 18.**
Which of the following correctly identifies the four key components of a well-structured SIERRA prompt?

A. Role, Task, Examples, Format  
B. Role, Task, Context, Format  
C. Persona, Instructions, Background, Output  
D. Intent, Scope, Data, Delivery

> **Answer: B** — The four components are Role, Task, Context, and Format.

---

**Question 19.**
How does interacting with SIERRA fundamentally differ from using a search engine like Google?

A. SIERRA only returns one result, while Google returns many  
B. Google requires an account, while SIERRA does not  
C. SIERRA allows iterative back-and-forth refinement; a search engine interaction effectively ends with the initial query result  
D. SIERRA charges per query, while Google is free

> **Answer: C** — The iterative, dialogue-based nature of AI is the key differentiator from search engines.

---

**Question 20.**
What is described as "arguably the highest-impact approach to prompting" in SIERRA?

A. Using bullet points in every prompt  
B. Always specifying an output format first  
C. Asking SIERRA itself to write the prompt based on a stream-of-consciousness description of the task  
D. Starting every prompt with a role assignment

> **Answer: C** — Having SIERRA generate the prompt from rough natural-language input is the highest-impact prompting approach.

---

### Day 10 — Structuring Complex Tasks

**Question 21.**
What is the most common mistake users make when approaching complex, multi-step tasks in SIERRA?

A. Uploading too many files at once  
B. Leading with the final deliverable step instead of working through intermediate steps sequentially  
C. Using the microphone feature instead of typing  
D. Saving prompts before they are fully tested

> **Answer: B** — The mistake is asking for the final output without first completing the upstream processing steps.

---

**Question 22.**
After successfully completing a complex, multi-step workflow in SIERRA, what is the recommended final action to preserve that workflow for future use?

A. Delete the thread to protect privacy  
B. Share the thread with a workspace  
C. Ask SIERRA to review the full conversation and produce a reusable prompt capturing all the steps taken  
D. Export the thread to PDF for record-keeping

> **Answer: C** — Asking SIERRA to synthesize the conversation into a reusable prompt allows the same workflow to be replicated on future similar tasks.

---

### Day 11 — Structuring Prompts for Data Extraction

**Question 23.**
When building a structured data extraction prompt, what is the purpose of the "evidence" field in the extraction checklist?

A. To attach supporting documents to the extraction output  
B. To ask the model to return a rationale, justification, or probability score explaining why it extracted a particular piece of data  
C. To provide the model with background information before extraction begins  
D. To record the timestamp of when the extraction was performed

> **Answer: B** — "Evidence" asks the model to return justification alongside each extracted result — such as an exact quote, clause reference, or confidence score.

---

**Question 24.**
Why is it important to explicitly define the *output format* when building a data extraction prompt?

A. SIERRA cannot produce tables without an explicit format instruction  
B. Format definitions prevent the model from accessing the internet  
C. Specifying the format reduces the model's cognitive load, freeing it to focus on precise extraction  
D. SIERRA uses fewer tokens when output is structured

> **Answer: C** — Defining the output format is a cognitive load reduction strategy so the model can concentrate on extraction rather than determining how to present results.

---

**Question 25.**
The "phased extraction" approach is recommended when working with large or complex documents. What is the purpose of including the *first-pass output* in the second extraction prompt?

A. It allows Sierra to skip re-reading the document entirely on the second pass  
B. It serves as a grounding anchor — giving the model a confirmed high-level understanding of the document before requesting more granular detail  
C. It reduces the token count needed for the second pass  
D. It prevents the model from generating duplicate fields

> **Answer: B** — The first-pass output grounds the model with confirmed high-level metadata before granular Phase 2 extraction begins.

---

### Day 12 — Working with Files, Part 1

**Question 26.**
When a file is uploaded to SIERRA, it is first converted to raw text and placed into what structure?

A. A context window buffer  
B. A vector store — a separate database from which relevant sections are retrieved based on the user's query  
C. The model's long-term memory  
D. A shared workspace file system visible to all employees

> **Answer: B** — Files go through conversion → vector store → query-based retrieval into the context window.

---

**Question 27.**
A user uploads a file in one thread, then starts a new thread and asks SIERRA about that same document. What will happen?

A. SIERRA will retrieve the file from the vector store it was previously indexed in  
B. SIERRA will not have access to the file — thread attachments do not carry over to new threads  
C. SIERRA will prompt the user to re-confirm permission to access the file  
D. SIERRA will find the file in the user's workspace automatically

> **Answer: B** — Files do not persist across threads. They must be re-uploaded in each new conversation.

---

### Day 13 — Working with Files, Part 2

**Question 28.**
When a SIERRA response based on an uploaded file seems wrong or incomplete, what should be the *first* thing a user checks?

A. Switch to a more powerful model  
B. Re-submit the same prompt with more detail  
C. Preview the file conversion to verify the document was ingested correctly before assuming the model failed  
D. Upload the file to a workspace instead of a thread

> **Answer: C** — Like the calculator rule: if the output is wrong, check the inputs first. Preview the conversion before blaming the model.

---

**Question 29.**
SIERRA offers two file conversion modes. Which of the following accurately describes the difference between them?

A. "Fast" uses GPT-4; "Full" uses Claude — selected based on document complexity  
B. "Fast" strips to raw text while preserving general structure; "Full" runs OCR and generates text descriptions of images for a more complete output  
C. "Fast" converts only the first 20 pages; "Full" processes the entire document  
D. "Fast" is for DOCX files; "Full" is required for PDF files

> **Answer: B** — Fast = text extraction with structure preserved; Full = OCR plus image description for richer, more complete conversion.

---

### Day 14 — Memories

**Question 30.**
Which of the following best describes the function of SIERRA Memories?

A. A log of past conversations stored for compliance review  
B. Persistent context — key pieces of information saved once and automatically injected into the context window across all future chats  
C. A feature that allows the model to learn and update its weights from user interactions  
D. A workspace-level record of all files uploaded by team members

> **Answer: B** — Memories are persistent context — saved once, always included in the context window without the user having to re-enter them.

---

**Question 31.**
Which of the following is the *most appropriate* type of information to store in Sierra's personal memories feature?

A. A complete copy of a current client's project scope document  
B. The full text of an ABS procedure that changes annually  
C. Your role, specialization, regional context, and preferred output format — stable background information about you and how you work  
D. The specific findings from the survey you completed last week

> **Answer: C** — Memories are best used for stable background information about the user — not project-specific or time-sensitive content.

---

### Day 15 — Workspaces

**Question 32.**
What is a key distinction between thread-level content and workspace-level content in SIERRA?

A. Thread content is shareable; workspace content is always private  
B. Thread content is private and temporary to the individual; workspace content — context, files, memories, and task modes — is shared and persistent across all members  
C. Workspace content is deleted after 30 days; thread content is permanent  
D. Thread content requires admin approval to access; workspace content does not

> **Answer: B** — Thread content stays with the individual user; everything at the workspace level is shared and persists for all members.

---

**Question 33.**
A team member uploads a reference document to a Sierra workspace's Files tab. What is the effect of this action for other workspace members?

A. They receive a notification to download and review the file locally  
B. The file is available for them to reference in their own chats within that workspace without needing to re-upload it  
C. They can view the file only if the uploader grants individual permissions  
D. The file is added to Sierra's global knowledge repository for all ABS users

> **Answer: B** — Workspace files are accessible to all members for use in their own chats — no re-upload required.

---

### Day 16 — Workspace Task Modes

**Question 34.**
What is the most useful rule of thumb for deciding whether information belongs in *workspace context* versus a *task mode*?

A. Context is for large files; task modes are for short prompts  
B. Background information (project, client, scope) belongs in context; specific, repeatable, actionable instructions belong in task modes  
C. Context is for individual users; task modes are for workspace admins only  
D. Task modes should never reference workspace files

> **Answer: B** — Background and orientation → workspace context. Specific, step-by-step repeatable instructions → task modes.

---

**Question 35.**
Task modes are most valuable for which type of work?

A. One-time, highly unique tasks that will never be repeated  
B. Ad-hoc brainstorming where the output format is flexible  
C. Specific, repeatable workflows — such as emergency response validations, compliance checks, or proposal generation — where consistent step-by-step instruction improves reliability  
D. Simple single-question queries that do not require structured output

> **Answer: C** — Task modes are designed for specific, repeatable, structured workflows where consistent instructions improve reliability.

---

### Day 17 — Workspace Walkthrough

**Question 36.**
What is the stated difference between *personal memories* and *workspace memories* in SIERRA?

A. Personal memories are visible to all users; workspace memories are private to the workspace owner  
B. Personal memories hold role- and preference-specific information about the individual; workspace memories hold project- or client-specific information accessible to all workspace members  
C. Personal memories expire after 90 days; workspace memories are permanent  
D. Workspace memories are automatically generated; personal memories must be set manually

> **Answer: B** — Personal memories are about the individual user; workspace memories are about the project or client scope and are visible to all workspace members.

---

### Day 18 — Building a Workspace: Proposal Generation

**Question 37.**
In the proposal generation walkthrough, the instructor began building the workspace in a *regular chat* rather than inside the workspace environment. What was the primary reason for this?

A. The workspace environment does not support file uploads during initial setup  
B. Regular chats have access to more powerful models than workspaces  
C. A regular chat was used to leverage Sierra's reasoning ability to analyze materials, draft context, and generate task mode prompts before moving those outputs into the workspace  
D. Building in a regular chat first is required by Sierra's technical architecture

> **Answer: C** — A regular chat was used to let Sierra analyze materials and draft workspace components before moving the finalized outputs into the workspace.

---

**Question 38.**
When starting to build a SIERRA workspace, why is it important to include information about how SIERRA workspaces are structured in the initial planning chat?

A. Because SIERRA needs the user's personal memory settings before configuring a workspace  
B. Because the frontier models have no inherent knowledge of what a SIERRA workspace is — its components must be explicitly defined  
C. Because team member names must be listed in the initial chat for access control purposes  
D. Because a web search is needed to pull in best practices before workspace design can begin

> **Answer: B** — The frontier models don't know what a SIERRA workspace is, so its structure — context, files, task modes — must be defined explicitly in the chat.

---

**Question 39.**
The phrase "bring a human into the loop" — as used in the Day 18 proposal generation example — refers to which specific design choice?

A. Having a team manager approve SIERRA's outputs before any action is taken on them  
B. Configuring the task mode to first extract and confirm all key variables with the user before generating any proposal content, rather than proceeding automatically end-to-end  
C. Requiring two people to be simultaneously logged into the workspace during task execution  
D. Limiting SIERRA to providing advisory suggestions rather than generating full document drafts

> **Answer: B** — The task mode was designed to pause at variable confirmation before generating content. This deliberate checkpoint keeps a human in the loop, ensuring the output is built on verified inputs rather than assumed ones.

---

**Question 40.**
When analyzing sample proposals and templates in the workspace development walkthrough, the instructor asked Sierra to produce a comparison table, a variable list, and a breakdown of boilerplate versus customized sections. What was the primary purpose of this analysis step?

A. To give Sierra a chance to practice formatting tables before the real work began  
B. To create a deliverable to send directly to the Bureau team  
C. To build a confirmed, shared understanding of how proposals are structured before constructing any workspace components — reducing ambiguity and missed edge cases  
D. To test whether Sierra could handle multiple files simultaneously

> **Answer: C** — Building a thorough, confirmed understanding of document structure before constructing workspace components ensures the context and task mode are grounded in reality, not assumptions.

---

### Day 19 — Plato Demo

**Question 41.**
In the Plato demo, the question asked was deliberately multi-dimensional — covering annual survey scope, suspect areas, and close-up survey expectations in a single query. What does this illustrate about how Plato should be used?

A. Plato can only handle one rule citation at a time and should not be used for compound questions  
B. Plato is designed to synthesize across multiple rules and sub-requirements to address scenario-based, multi-part questions in a single response  
C. Multi-part questions always produce inaccurate results and should be broken into separate threads  
D. Plato will only answer questions that directly quote a specific rule part and section number

> **Answer: B** — Plato is designed to synthesize across multiple rules and sub-requirements to address complex, scenario-based, multi-part questions.

---

**Question 42.**
In the Plato demo, when a prior finding of substantial corrosion and coating breakdown in a ballast tank was introduced as a follow-up scenario, what did Plato do that demonstrated its grounding in the rules?

A. It repeated the same answer as the initial query because the overall survey scope had not changed  
B. It searched the internet for general industry guidance on ballast tank corrosion  
C. It connected requirements from two different rule sections — suspect areas and ballast tank examination — and outlined a specific follow-up plan including close-up survey and thickness measurements  
D. It flagged the question as outside Plato's scope and recommended consulting the ABS website directly

> **Answer: C** — Plato connected requirements from two different subsections (suspect areas under 1.1.9 and ballast tank examination under 1.1.10) and built a specific, actionable follow-up plan from them — demonstrating scenario-based reasoning grounded in the rules.

---

### Day 20 — Workspaces Demo: Environmental Plan Reviews

**Question 43.**
In the workspaces demo, the instructor created one workspace called "Environmental Plan Reviews" but built multiple task modes within it — one per type of review. What principle does this design reflect?

A. Each type of review requires a separate workspace to maintain data isolation  
B. General context and style settings are shared at the workspace level, while specific step-by-step review instructions are isolated within individual task modes — eliminating the need for a separate workspace per task  
C. Task modes are only useful when a workspace contains fewer than five members  
D. Workspace context is regenerated from scratch each time a new task mode is invoked

> **Answer: B** — Shared context lives at the workspace level; specific instructions live in individual task modes — one workspace serves many task types.

---

**Question 44.**
When building the SOPEP task mode, the instructor started in a regular chat rather than the workspace Task Modes editor. Why?

A. Task modes cannot be created directly inside a workspace — they must always be built externally first  
B. The workspace environment does not support Sierra's more advanced models  
C. Sierra was used in a regular chat to generate the task mode instructions from the 34 review questions, which were then copied and pasted into the workspace — leveraging Sierra to build the instructions rather than writing them manually  
D. Regular chats have a larger context window than workspace chats, which was needed for the 34-question input

> **Answer: C** — Sierra was used in a regular chat to generate task mode instructions from the review questions — then the output was moved into the workspace.

---

**Question 45.**
In the SOPEP Review task mode output, what feature was included specifically to support human oversight of SIERRA's review?

A. A confidence score from 0–100% for each answer provided by SIERRA  
B. A compliance checklist with yes/no flags, findings, source references within the document, and a reviewer check column for the user to manually confirm each item  
C. An automated email alert sent to the team lead whenever SIERRA marks an item as non-compliant  
D. A locked, read-only format to prevent users from altering SIERRA's conclusions

> **Answer: B** — The compliance checklist with yes/no flags, findings, source references, and a reviewer check column is a deliberate human oversight mechanism. It makes it easy for a reviewer to audit SIERRA's work item by item.

---

### Day 21 — Web Search & Deep Research Demo

**Question 46.**
What is the key distinction between Sierra's standard *web search* and its *deep research* feature?

A. Web search only retrieves results from ABS-approved websites; deep research accesses all public sources  
B. Web search is faster and produces a structured summary with citations; deep research conducts a more comprehensive multi-source investigation and generates a detailed, downloadable technical report  
C. Deep research disables citation linking to prevent users from following sources that may be inaccurate  
D. Web search and deep research are functionally identical — deep research simply repeats the same query three times

> **Answer: B** — Web search is faster and produces a structured summary; deep research conducts a more comprehensive investigation and generates a detailed downloadable technical report.

---

**Question 47.**
A user needs to quickly compare regulatory timelines, infrastructure status, and commercial readiness across three alternative maritime fuels for an upcoming client presentation. Which SIERRA capability is best suited to reduce the time spent gathering and synthesizing this information?

A. Uploading a single industry whitepaper and asking SIERRA to summarize it  
B. Using SIERRA's web search to run multiple targeted searches simultaneously, producing a structured comparison table with source citations  
C. Asking SIERRA to answer from its internal training data alone, since maritime fuel regulations are well-documented in public sources  
D. Using the HR Policy Repository to check ABS's internal fuel strategy documentation

> **Answer: B** — Web search runs multiple targeted searches and synthesizes results into a structured comparison table with citations — exactly suited for multi-fuel, multi-dimension research.

---

### Day 22 — HR Policy Repository Demo

**Question 48.**
What makes the HR Policy Repository in Sierra distinct from simply uploading an HR policy document and asking a question?

A. The repository only works for managers and HR business partners, not individual contributors  
B. Sierra automatically identifies the user's entity and home country and retrieves the applicable policy without the user needing to specify it  
C. The repository is read-only and cannot be queried through natural language — users must search by document name  
D. HR policy documents are not permitted for upload under the ABS data policy, so the repository is the only compliant access method

> **Answer: B** — The HR repository auto-identifies the user's entity and home country, applying the correct policy without the user needing to specify it.

---

**Question 49.**
A US-based ABS Group employee and a Norway-based ABS Bureau employee both ask Sierra the exact same question: *"How many days of PTO do I get?"* What will happen?

A. Both employees will receive the same answer, since Sierra applies one global policy  
B. Sierra will return an error because the question does not specify a country  
C. Each employee will receive an answer tailored to their own entity and home country — Sierra automatically applies the relevant policy for each user's profile  
D. Sierra will ask a clarifying question before retrieving any policy information

> **Answer: C** — Sierra automatically applies the relevant policy for each user's entity and home country — each employee receives a personalized answer.

---

**Question 50.**
If an employee asks Sierra a detailed HR question and the answer is not covered in the policy repository, what does Sierra do?

A. It generates a best-guess response based on comparable policies from similar companies  
B. It performs a web search for general HR guidance and presents that as the answer  
C. It clearly states that the policy is not in the repository and directs the user to their HR business partner, rather than filling gaps with approximations  
D. It escalates the question automatically to the user's manager

> **Answer: C** — When a policy is not in the repository, Sierra clearly states this and directs the user to their HR business partner — it does not fill gaps with approximations.

---

---

## Question Distribution by Day

| Day | Topic | Questions | Count |
|-----|-------|-----------|-------|
| 1 | Why Sierra | 1–2 | 2 |
| 2 | Privacy, Security & Data Governance | 3–5 | 3 |
| 3 | What Are Large Language Models? | 6–7 | 2 |
| 4 | What the Model Knows | 8–9 | 2 |
| 5 | Context | 10–11 | 2 |
| 6 | SIERRA's Tools for Adding Context | 12–13 | 2 |
| 7 | Tokens & Context Windows | 14–15 | 2 |
| 8 | Hallucinations | 16–17 | 2 |
| 9 | Prompting Fundamentals | 18–20 | 3 |
| 10 | Structuring Complex Tasks | 21–22 | 2 |
| 11 | Structuring Prompts for Data Extraction | 23–25 | 3 |
| 12 | Working with Files, Part 1 | 26–27 | 2 |
| 13 | Working with Files, Part 2 | 28–29 | 2 |
| 14 | Memories | 30–31 | 2 |
| 15 | Workspaces | 32–33 | 2 |
| 16 | Workspace Task Modes | 34–35 | 2 |
| 17 | Workspace Walkthrough | 36 | 1 |
| 18 | Building a Workspace: Proposal Generation | 37–40 | 4 |
| 19 | Plato Demo | 41–42 | 2 |
| 20 | Workspaces Demo: Environmental Plan Reviews | 43–45 | 3 |
| 21 | Web Search & Deep Research Demo | 46–47 | 2 |
| 22 | HR Policy Repository Demo | 48–50 | 3 |
| **Total** | | | **50** |

---

*End of Quiz — 50 Questions*
