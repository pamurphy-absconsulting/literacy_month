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
  - **Task** — say exactly what you want: summarize, draft, compare, extract, rewrite
  - **Context** — give it the raw material: paste the document, describe the project, name the client
  - **Format** — tell it how to respond: bullet list, executive summary, table, plain language

> **Weak:** "Summarize this report."
> **Strong:** "You are reviewing a marine survey report. Summarize the top 3 findings in plain language for a non-technical client. Use bullet points."

**Your first prompt is a starting point, not a final answer.**
- When Sierra misses: tell it what was wrong and add what it was missing — *"Too long, cut to 3 bullets"* / *"Here's an example of what I actually want: [paste it]"*
- When a thread has gone sideways: start fresh with a better prompt — don't fight a bad thread
- Don't know how to prompt it? Ask Sierra: *"I need to [rough description]. Write me a clean prompt I can use."*

[Visual: Two-column comparison — Vague vs. Specific example. Below: four labeled blocks — ROLE | TASK | CONTEXT | FORMAT — each with a one-line example. Bottom callout: "First prompt = starting point. Refine until it's right."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 10: Advanced Prompting Techniques*

---

**Day 10: Controlling How Sierra Thinks**

**Chain of thought — ask Sierra to reason before it concludes**
- Add *"think through this step by step"* or *"walk me through your reasoning before giving an answer"*
- Forces the model to show its work — more accurate on complex problems, easier to spot where it went wrong
- ABS example: *"Walk through whether this vessel configuration meets each relevant SOLAS requirement before giving your conclusion."*

**Task decomposition — break complex asks into steps**
- One massive prompt on a complex task = one shot at getting it right
- Sequential prompts = each step is reviewable before the next
- ABS example: Step 1: *"Extract the key findings from this survey data."* → Step 2: *"Rank by severity and client impact."* → Step 3: *"Write an executive summary for a non-technical client covering the top 3."*

**Guide the reasoning — be explicit about approach**
- *"Be conservative — flag any uncertainty rather than assuming compliance"*
- *"Consider both the technical requirements and the client relationship before recommending"*
- *"Approach this as a senior ABS surveyor reviewing for class renewal"*

[Visual: Three labeled sections — CHAIN OF THOUGHT / TASK DECOMPOSITION / GUIDE THE REASONING — each with a one-line ABS example. Connecting theme at bottom: "You're not just telling Sierra what to produce — you're directing how it thinks."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 11: The Context Window — What Sierra Sees*

---

**Day 11: The Context Window — What Sierra Sees**

- The context window is the maximum amount of text the model can process at one time — it determines everything Sierra can "see" when generating a response
- Several sources inject content into that window:
  - **Your prompt** — what you write explicitly
  - **System prompt** — Sierra's base instructions, set at the application level
  - **Personal memories** — your persistent context, injected automatically in standard threads
  - **Workspace context & workspace memories** — team-level persistent context, injected for every workspace thread
  - **Retrieved chunks** — relevant content pulled in via RAG from files, knowledge bases, or the web
  - **Conversation history** — prior turns in the thread (this is why longer threads cost more)
- Persistent vs. ephemeral: memories and workspace context survive across threads; uploads and retrieved content do not
- Important: personal memories do not apply inside workspaces — workspace memories replace them; workspace memories do not carry over to regular chats
- This is the mental model behind all of Sierra's features — workspaces, memories, and retrieval tools all exist to put the right information in front of the model automatically

[Visual: A central box labeled "CONTEXT WINDOW — What Sierra Sees." Six labeled arrows flowing into it from outside: YOUR PROMPT, SYSTEM PROMPT, PERSONAL MEMORIES, WORKSPACE CONTEXT & MEMORIES, RAG RESULTS, CONVERSATION HISTORY. Below the box: a horizontal divider — left side "Persistent (survives across threads)" showing Personal Memories + Workspace Context & Memories; right side "Ephemeral (this thread only)" showing RAG Results + Conversation History. Clean, layered diagram.]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 12: How Sierra Retrieves Information (RAG)*

---

**Day 12: How Sierra Retrieves Information (RAG)**

- RAG in practice: your query → semantic search → relevant chunks retrieved → added to context window → model responds
- The model only sees what gets retrieved — not the entire knowledge base
- This means: **specific queries = better retrieval = better answers** (same principle as Day 9 prompting)
- RAG is the mechanism behind all of Sierra's knowledge tools — file uploads, workspace files, Plato, eCFR, SkillShare, HR — same pipeline, different sources
- Web search works the same way — live web instead of an internal knowledge base; if Sierra thinks a query may contain confidential information, it will ask for your approval before sending

[Visual: A pipeline diagram — left to right: YOUR QUERY → SEMANTIC SEARCH → CHUNKS RETRIEVED → CONTEXT WINDOW → MODEL → RESPONSE. Below the "SEMANTIC SEARCH" step: a fork showing three source options: "Your Files" (thread attachments), "Workspace / Knowledge Bases" (Plato, eCFR, workspace files, HR, SkillShare), "Web Search" (live web, with approval for sensitive queries). All three are labeled as flavors of the same retrieval process.]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 13: Working with Files — Part 1*

---

**Day 13: Working with Files — Part 1**

- Upload documents directly into a thread — Sierra converts them to text, chunks the content, and retrieves relevant sections via RAG (the same pipeline from Day 12)
- File-friendly: text-based PDFs, Word docs, Excel spreadsheets — structured, selectable text works best
- File-unfriendly: scanned documents, image-heavy PDFs, complex nested tables — extraction quality drops significantly
- Files uploaded to a thread are temporary — Sierra does not carry them into new threads
- Thread attachments vs. workspace files: thread attachments stay isolated to a single thread; workspace files are persistent and shared across every user in the workspace

[Visual: Two-column table. Left — "Works Well" (green): text-based PDF, .docx, .xlsx, .txt. Right — "Watch Out" (orange/red): scanned PDF, image-heavy doc, complex table. Below the table: the RAG pipeline applied to files — FILE UPLOAD → CONVERT TO TEXT → CHUNK → VECTOR STORE → RETRIEVE → CONTEXT WINDOW. A callout at the bottom: "Thread attachment = temporary and isolated. Workspace file = persistent and shared."]

**ABS & Affiliated Companies**

---
