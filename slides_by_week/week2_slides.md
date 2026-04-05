# SIERRA Literacy Month — Week 2 Slides
## Days 4–8: AI Fundamentals
*Days 4, 5, 8 locked. Days 6 and 7 being re-recorded.*

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 4: What the Model Knows — and Where It Stops*

---

**Day 4: What the Model Knows — and Where It Stops**

[Diagram: Concentric circles diagram.
- Outer Circle (Dashed): Boundary of "Internal Knowledge"
- Middle Circle: Public Knowledge / Historical Events / General Logic
- Inner Circle (Blue): Deep Domain Knowledge (engineering, law, science, etc.)
- Separate circle clearly outside the boundary: **ABS Data** (projects, clients, procedures, people — never on the public internet)]

**What Internal Knowledge Does NOT Include:**
- Anything that was never on the public internet — corporate IP, internal project data, unpublished work
- Events after the model's training cutoff *(current Sierra models: late 2024 to mid-2025)*
- ABS: its rules, procedures, clients, projects, or people

**What It Does Include:**
- Publicly available knowledge, historical events, general logic, deep domain expertise

**Rule of thumb: if it was never on the public internet, it is not in the model's internal knowledge.**

**All non-public data must come from you — through context.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 5: Context — The Lever You Control*

---

**Day 5: Context — The Lever You Control**

[Diagram: Two circles side by side — no overlap, no third source implied.
- Left Circle (Blue, larger): **Context** — your prompt text / files you upload / conversation history
- Right Circle (Yellow): **Internal LLM Knowledge** — what the model was trained on (fixed)
Nothing exists outside these two. Internal knowledge is outside your control. Context is not.]

**Core Ideas**
- The model reasons over the information you provide using its internal patterns (reasoning)
- **Context is the lever you control** — internal knowledge is set; context is not
- Context includes: what you type in your prompt, files you attach, and the conversation history
- Sierra cannot help with ABS-specific work unless you provide ABS-specific context

**Your job as a SIERRA user: load up the context with what the model can't know on its own.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 6: SIERRA's Tools for Adding Context*

---

**Day 6: SIERRA's Tools for Adding Context**

| Tool | What it does |
|---|---|
| **File Attachments** | SIERRA converts, reads, and brings information in from documents you provide |
| **Web Search** | Targeted queries to bring more current or additional information into context |
| **Knowledge Repositories** | Curated ABS-specific data sets that SIERRA can query automatically |

**Example:** Ask SIERRA about ABS vacation policy. SIERRA retrieves info from an ABS-built knowledge repo, reasons over it, and responds.

**Core Ideas**
- SIERRA is not a model — it provides secure access to frontier models with additional tools
- These tools bring in information the models don't already have
- The additional information enters the context window and the model reasons over it to produce output

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 7: Tokens & Context Windows*

---

**Day 7: Tokens & Context Windows**

**Why can't we simply make ALL information available to the model?**

**The Constraint in Practice**
- The model can only process so much information at once — this is called its context window
- Context window = working memory = max processing load
- This constraint is measured in tokens
- Tokens are chunks of text — each one is processed as a mathematical representation of language
- Roughly 666 tokens per page of text
- Large, but not infinite
- Focused threads = better answers
- Noise degrades quality: long, scattered threads force the model to sift through everything in its window to find what matters
- Long conversations with huge amounts of information (via upload or retrieval) will push earlier content out

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 8: What is a Hallucination?*

---

**Day 8: What is a Hallucination?**

**Core Ideas**
- A "hallucination" is a confident, fluent output not grounded in truth.
- Models are trained to produce the most probable continuation of text, not necessarily the most truthful continuation.
- This often occurs with insufficient context and edges of training data where it's filling a gap based on patterns but not on real data.
- This is why much of our focus is on building internal knowledge systems and why you should always verify outputs.

**ABS & Affiliated Companies**

---
