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
*Day 11: Structuring Prompts for Data Extraction*

---

**Day 11: Structuring Prompts for Data Extraction**

*What you're leveraging here is processing power, not reasoning — Sierra's ability to read and ingest massive amounts of information and pull out key data at scale.*

**Before you write the prompt, define the target.**

| Question | What to specify |
|---|---|
| **Field** | What am I extracting? |
| **Definition** | What exactly counts? |
| **Exclusions** | What should not count? |
| **Location** | Where in the document is it likely found? |
| **Decision rules** | How do I handle multiple candidates? |
| **Evidence** | What proof should Sierra return? |
| **Output format** | How should the result be structured? |

**Five practical moves:**
1. **Define the field** — name it precisely, not generically
2. **Tell Sierra where to look** — section, heading, schedule, clause number
3. **Set the boundaries** — spell out what counts and what doesn't
4. **Extract in phases** — coarse pass first, then fine pass grounded by the anchors you confirmed
5. **Ask for evidence and a set format** — return the clause, the exact text, one row per item

**Phased extraction:**
- **Pass 1:** Pull high-level anchors — party names, vessel type, contract structure, applicable schedule
- **Pass 2:** Inject those anchors back into the prompt with the same file + precise instruction — the model is now working from confirmed ground truth, not guessing

**ABS example:**
- Pass 1: *"Identify the contracting party, contract type, and which pricing schedule applies."*
- Pass 2: *"Under Schedule B as confirmed above, extract the day-rate for each vessel class as defined in Clause 4. List any exclusions. Return one row per vessel class with: vessel class | day-rate | applicable clause | exclusions."*

**The goal: reduce ambiguity enough that less thinking is left to the model — the less it has to figure out, the more it can focus on the extraction itself.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 12: Working with Files — Part 1*

---

**Day 12: Working with Files — Part 1**

[Visual: FILE → CONVERSION → STORE → RETRIEVE → RESPOND. Note under CONVERSION: "preview available before attaching"]

**Common misconceptions:**
- Once you upload a file, SIERRA now "knows" it
- The entire file's contents are brought into context
- SIERRA reads and understands all content always
- SIERRA can answer questions on data even when it doesn't have the data

**How SIERRA actually handles files:**
- Files are converted to raw text — you can preview before attaching
- Once attached, all files in the thread are pooled into a shared store (a separate database, not the context window)
- When you send a query, Sierra pulls the most relevant sections into context and sends those — along with your question — to the model
- The entirety of the file is not in the context window; different questions surface different sections
- Source quality matters — clean, structured text converts more reliably

**Thread attachments are temporary** — Sierra does not carry them into new threads. For files shared across a team, use workspace files instead.

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 13: Working with Files — Part 2*

---

**Day 13: Working with Files — Part 2**

*"There's no amount of prompting that can compensate for data simply not being read in correctly."*

**File format — the number one thing to consider:**
- Is it text-based or image-heavy?
- Is it a scanned PDF or a DOCX?
- Is it tabular or diagram-heavy?
- All of these impact the conversion — the model is reading text, so images and diagrams get converted to text descriptions; complexity affects quality

**Conversion quality — preview it before you attach:**
- When you upload a file, you can preview the conversion before attaching it to a thread
- By default Sierra runs **fast conversion** — strips out text, maintains general structure
- If the preview looks incomplete or mangled, switch to **full conversion** — runs OCR, looks at images and generates descriptions, produces a more complete structured format
- Check it. If the conversion is wrong, the prompt won't fix it.

**The inputs are what shape the outputs.**
- We don't naturally apply the same logic to AI that we apply to a calculator — when we get a wrong answer, our first instinct isn't to check the inputs
- Start there. The problem is usually in the data that was ingested, not the model.

[Visual: PROMPT → OUTPUT → REFINE → REPEAT loop. Two panels: FILE FORMAT (text-based vs. image-heavy, scanned vs. DOCX, tabular/diagram-heavy) | CONVERSION QUALITY (preview, fast vs. full/OCR). Callout: "Inputs shape outputs."]

**ABS & Affiliated Companies**

---
