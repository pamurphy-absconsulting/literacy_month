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
*Day 10: Structuring Complex Tasks*

---

**Day 10: Structuring Complex Tasks**

**Structured analysis — ask for a clear sequence, not just an answer**
- On complex problems, specify the output structure: criteria → assessment → uncertainty → conclusion
- This makes responses easier to review and easier to push back on
- ABS example: *"Assess this vessel configuration against the relevant SOLAS requirements. For each requirement, state: requirement, whether it appears met, any uncertainty, and recommended follow-up. Then give a final conclusion."*

**Task decomposition — break complex asks into steps**
- One massive prompt on a complex task = one shot at getting it right
- Sequential prompts = each step is reviewable before the next
- ABS example: Step 1: *"Extract the key findings from this survey data."* → Step 2: *"Rank by severity and client impact."* → Step 3: *"Write an executive summary for a non-technical client covering the top 3."*

**Guide the approach — be explicit about how to evaluate**
- *"Be conservative — flag any uncertainty rather than assuming compliance"*
- *"Consider both the technical requirements and the client communication risk"*
- *"Use the perspective of a senior ABS reviewer — flag what needs human verification"*

[Visual: Three labeled sections — STRUCTURED ANALYSIS / TASK DECOMPOSITION / GUIDE THE APPROACH — each with a one-line ABS example. Connecting theme at bottom: "You're not just telling Sierra what to produce — you're directing how it evaluates."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 11: Context Engineering*

---

**Day 11: Context Engineering**

[Visual: Context Engineering diagram — prompt + thread history + past tool responses flow in from the left; system prompt + memories + style + user info flow in from the right; workspace instructions from the top. All feed into the Large Language Model. Response exits at the bottom.]

- Everything in that diagram is the context window — your prompt is one input among many
- **Left side (you control per thread):** prompt, thread history, past tool responses
- **Right side (persistent, automatic):** system prompt, memories, style, user info
- **Top (workspace-level):** workspace instructions — shared context that applies across threads in that workspace
- Responses may draw on the broader context, not just your latest message — though not every piece of context carries equal weight
- Context shifts depending on where you're working — in a workspace, workspace-level instructions and shared context shape every thread automatically
- Context engineering = being deliberate about what's in that window. Prompting controls the left side. Memories and workspaces engineer the right. RAG fills it with retrieved knowledge.

**Sierra isn't a chat box. It's a system you can configure.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 12: How Sierra Retrieves Information (RAG)*

---

**Day 12: Working with Files — Part 1**

- You can upload documents directly into a thread — Sierra does not read the whole file into the chat
- In simplified terms: Sierra extracts text from the file, indexes it in retrievable sections, and retrieves the most relevant passages based on your query — those passages enter the context window
- **Specific questions get better results than vague ones** — Sierra retrieves what your query points to, not everything in the file
- The quality of retrieval depends on the quality of the source — clearly formatted, text-based documents tend to extract more reliably than image-heavy or poorly structured ones; extraction capabilities are actively improving
- Thread attachments are temporary — Sierra does not carry them into new threads
- Thread attachments vs. workspace files: isolated to one thread vs. persistent and shared across every user in the workspace

[Visual: File upload flow — FILE → EXTRACT TEXT → INDEX SECTIONS → RETRIEVE (based on query) → CONTEXT WINDOW → RESPONSE. Callout: "Sierra doesn't read the whole file. It retrieves the parts your question points to." Below: "Source quality affects retrieval quality — the clearer the document, the better the extraction."]

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 13: Working with Files — Part 2*

---

**Day 13: Working with Files — Part 2**

- Sierra can generate structured output from files: summaries, extracted data, reformatted content, comparisons
- If output format matters, give Sierra a template — paste an example of what you want and ask it to match the structure
- Ask targeted questions rather than "summarize everything" — retrieval is query-driven, so specific asks surface specific content
- Sierra gives you content to work with, not finished deliverables — apply final formatting, branding, and production in your document tools
- Capabilities here are actively expanding; the habit that stays constant is: direct the output, then shape it into the final form yourself

[Visual: Before/after diagram. Left: "Messy or Raw Input" (rough text, inconsistent formatting). Center: arrow through "SIERRA + Template." Right: "Clean, Structured Output." Callout below: "Sierra produces the content. You handle the final formatting." Second callout: "Specific question → specific retrieval → better output."]

**ABS & Affiliated Companies**

---
