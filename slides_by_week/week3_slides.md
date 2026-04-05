# SIERRA Literacy Month — Week 3 Slides
## Days 9–13: Prompting & How Sierra Works

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 9: Prompting Fundamentals*

---

**Day 9: Prompting Fundamentals**

- Vague in = vague out — specificity is the single biggest lever you have
- Four ingredients of a strong prompt:
  - **Role** — tell Sierra what it is: *"You are a technical reviewer..."*
  - **Tasks** — say exactly what you want: summarize, draft, compare, extract, rewrite
  - **Context** — give it raw material: paste the document, describe the project, name the client
  - **Format** — tell it how to respond: bullet list, executive summary, table, plain language

> **Weak:** "Summarize this report."
> **Strong:** "You are reviewing a marine survey report. Summarize the top 3 findings in plain language for a non-technical client. Use bullet points."

**Your first prompt is a starting point, not a final answer.**
- When Sierra misses: tell it what was wrong and add what it was missing with example
- When a thread has gone sideways: start fresh in a new thread
- Don't know how to prompt it? Ask Sierra! *"I need to [rough description]. Write me a clean prompt I can use."*

[Visual: Four labeled blocks — ROLE | TASKS | CONTEXT | FORMAT — each with a one-line example. Weak vs. Strong comparison. Bottom: "Your first prompt is a starting point, not a final answer."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 10: Structuring Complex Tasks*

---

**Day 10: Structuring Complex Tasks**

**You are the expert | You architect, SIERRA executes**

**YOU ARE THE SME**
- The models lack big picture thinking and cannot grasp full architecture of your problem without explicit instruction.
- SIERRA does not know your process, your project, your systems. Nor does it have your professional judgement.
- Your job is ultimately to provide the information it needs and communicate the steps for it to take.

**GUIDE THE PROCESS**
Break it into steps the way you'd brief an intern.
- One massive prompt = one shot at getting it right
- Sequential steps = review each before the next

ABS example:
- Step 1: *"Extract the key findings from this survey data."*
- Step 2: *"Rank by severity and client impact."*
- Step 3: *"Write an executive summary for a non-technical client covering the top 3."*

[Visual: Two-column layout — YOU ARE THE SME (left) | GUIDE THE PROCESS (right). Header: "You are the expert | You architect, SIERRA executes."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 11: Context Engineering*

---

**Day 11: Memories & Customization**

*Opening note: "I mentioned context engineering at the end of last time — we'll get there, but I want to cover something that'll actually make that concept land better when we do."*

**Stop re-explaining yourself. Every thread shouldn't start from zero.**

**What memories do:**
- Memories are persistent context — they carry into every thread automatically, without you typing them
- Sierra uses them as background when forming responses
- The response improves before you type a single word

**What to put in them:**
Things you'd otherwise repeat at the start of every prompt:
- Your role and specialization: *"I'm a marine surveyor, primarily hull and machinery"*
- Your audience: *"I typically write for non-technical clients or port state inspectors"*
- Your preferences: *"Keep responses concise. Use bullet points by default."*
- Your team/group context: *"I work in ABS Offshore, primarily MODU and FPSO work"*

**How to set them:**
Tell Sierra directly — *"Remember that I..."* — or add them in your profile settings.

**Personal vs. Workspace memories:**
- Personal memories: yours alone — follow you across all your standard threads
- Workspace memories: shared across a team — covered next week with Workspaces

**Set it once. Stop repeating it every thread.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 12: Working with Files — Part 1*

---

**Day 12: Working with Files — Part 1**

**How file retrieval works:**
- You can upload documents directly into a thread — Sierra does not read the whole file into the chat
- Sierra extracts text from the file, indexes it in retrievable sections, and retrieves the most relevant passages based on your query — those passages enter the context window
- The quality of retrieval depends on the quality of the source — clearly formatted, text-based documents retrieve more reliably than image-heavy or poorly structured ones

**How to prompt when working with a file:**
- **Your query drives what gets retrieved** — vague questions surface vague content; specific questions surface specific content
- Don't ask: *"Summarize this report"* — Ask: *"What are the top findings related to hull condition in section 3?"*
- Reference sections, topics, or names directly — it helps Sierra retrieve the right chunk
- If Sierra misses something you know is in the file, restate the question with more specificity or quote a term from the document

**Thread attachments are temporary** — Sierra does not carry them into new threads. For files shared across a team, use workspace files instead.

[Visual: File upload flow — FILE → EXTRACT TEXT → INDEX SECTIONS → RETRIEVE (based on query) → CONTEXT WINDOW → RESPONSE. Callout: "Sierra retrieves what your question points to — ask specifically."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 13: Working with Files — Part 2*

---

**Day 13: Working with Files — Part 2**

**Getting structured output:**
- Sierra can generate summaries, extracted data, reformatted content, and comparisons from files
- **Give it a template** — paste an example of the output you want and say *"match this structure"*; don't describe the format in the abstract when you can just show it
- **Break it into steps** (Day 10 applies here): extract first, then rank, then write — don't ask for the finished deliverable in one shot

**Prompting for output quality:**
- Be explicit about audience and purpose: *"Write this for a non-technical port state inspector, one page, plain language"*
- Ask it to flag uncertainty: *"Note any areas where the document was unclear or where you had to make assumptions"*
- If the first output misses: don't start over — tell it what was wrong: *"Too general — go back to section 4 and pull the specific deficiency findings"*

**What Sierra produces vs. what you finish:**
- Sierra gives you content to work with, not finished deliverables — apply final formatting, branding, and production in your document tools
- The habit that stays constant: direct the output, then shape it into the final form yourself

[Visual: Prompt → Output → Refine loop. Callout: "Show it the template. Break it into steps. Tell it what was wrong." Below: "Sierra produces the content. You handle the final form."]

**ABS & Affiliated Companies**

---
