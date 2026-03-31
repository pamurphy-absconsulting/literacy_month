# SIERRA Literacy Month — Week 3 Slides
## Days 9–13: Prompting & How Sierra Works

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 9: Prompting Fundamentals*

---

**Day 9: Prompting Fundamentals**

- A prompt is everything you send Sierra — the more intentional, the better the output
- Four ingredients of a strong prompt: **Role · Task · Context · Format**
- Vague in = vague out — specificity is the single biggest lever you have
- Prompting is iterative — one exchange rarely gets you there; refine and build

> **Weak:** "Summarize this report."
> **Strong:** "You are reviewing a marine survey report. Summarize the top 3 findings in plain language for a non-technical client."

[Visual: Two-column comparison — left column "Vague" (red/orange), right column "Specific" (blue/green). Below both: four labeled blocks in a row — ROLE | TASK | CONTEXT | FORMAT — each with a one-line description. Clean, minimal layout.]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 10: Advanced Prompting Techniques*

---

**Day 10: Advanced Prompting Techniques**

- Voice-to-text: speak your prompt — faster, more natural, often more detailed
- Meta-prompting: ask Sierra to rewrite your rough idea as a clean, reusable prompt
- Know when to continue vs. start fresh — scattered threads produce scattered answers
- Iterative loop: prompt → review output → refine the ask → repeat

> **Meta-prompt example:** *"Summarize what I've been asking you to do as a clear, specific prompt I could reuse next time."*

[Visual: A circular loop diagram — four nodes connected by arrows: PROMPT → REVIEW → REFINE → REPEAT → back to PROMPT. Separate callout box to the side: meta-prompt concept shown as "You → Sierra → Better Prompt → You."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 11: The Context Window — What Sierra Sees*

---

**Day 11: The Context Window — What Sierra Sees**

- The LLM only processes what's in its context window at the moment of each response — nothing more
- Several sources inject content into that window:
  - **Your prompt** — what you write explicitly
  - **System prompt** — Sierra's base instructions, set at the application level
  - **Memories** — personal persistent context, injected automatically into every thread
  - **Workspace context & memories** — team-level persistent context, injected for every workspace thread
  - **Retrieved chunks** — relevant content pulled in via RAG from files, knowledge bases, or the web
  - **Conversation history** — prior turns in the thread (this is why longer threads cost more)
- Persistent vs. ephemeral: memories and workspace context survive across threads; uploads and retrieved content do not
- Important: personal memories do not apply inside workspaces — workspace memories replace them there

[Visual: A central box labeled "CONTEXT WINDOW — What Sierra Sees." Six labeled arrows flowing into it from outside: YOUR PROMPT, SYSTEM PROMPT, MEMORIES (personal or workspace), WORKSPACE CONTEXT, RAG RESULTS, CONVERSATION HISTORY. Below the box: a horizontal divider — left side "Persistent (survives across threads)" showing Memories + Workspace Context; right side "Ephemeral (this thread only)" showing RAG Results + Conversation History. Clean, layered diagram.]

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
- RAG is the mechanism behind all of Sierra's knowledge tools — file uploads, workspace files, Plato, SkillShare, HR — same pipeline, different sources
- Web search works the same way — same retrieval model, pulling from the live web instead of an internal knowledge base

[Visual: A pipeline diagram — left to right: YOUR QUERY → SEMANTIC SEARCH → CHUNKS RETRIEVED → CONTEXT WINDOW → MODEL → RESPONSE. Below the "SEMANTIC SEARCH" step: a fork showing three source options: "Your Files" (thread attachments), "Workspace / Knowledge Bases" (Plato, workspace files, HR, SkillShare), "Web Search" (live web). All three are labeled as flavors of the same retrieval process.]

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
