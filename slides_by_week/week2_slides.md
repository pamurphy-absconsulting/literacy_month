# SIERRA Literacy Month — Week 2 Slides
## Days 4–8: AI Fundamentals
*Already recorded and delivered. Do not modify unless course requires serious reorganization.*

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

**Everything ABS-specific must come from you — through context.**

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
- Two and only two sources: internal knowledge (fixed, comes with the model) and context (what you provide)
- **Context is the lever you control** — internal knowledge is set; context isn't
- Context includes: what you type in your prompt, files you attach, and the conversation history
- The model works with both simultaneously — your context shapes what it reasons over
- Sierra cannot help with ABS-specific work unless you provide ABS-specific context

**Your job as a Sierra user: load up the context with what the model can't know on its own.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 6: How Sierra Bridges the Gap*

---

**Day 6: How Sierra Bridges the Gap**

[Diagram: Three-step flow.
1. **You ask** — an ABS-specific question Sierra can't know internally
2. **Sierra retrieves** — searches a curated ABS-built knowledge system for relevant content
3. **Sierra answers** — retrieved content enters the context; Sierra reasons over it and responds]

**Core Ideas**
- **LLMs are static** — parameters are set at training and never change. The model does not learn, adapt, or evolve as you use it.
- **Sierra does not learn from your conversations** — your chats do not modify the model in any way
- ABS does NOT train its own LLMs — too expensive, and a trained model is still static
- So how does Sierra know ABS-specific things? **We build knowledge systems** — curated repositories Sierra can search and retrieve from on demand

**Example:** Ask Sierra about ABS vacation policy. It doesn't know the answer internally — it retrieves it from an HR knowledge base ABS built, reasons over it, and responds. As policy changes, ABS updates the knowledge system. The model never needs to be retrained.

**Sierra's knowledge of ABS comes from systems we build and maintain — not from what it was trained on. More on how this works in Week 3.**

**ABS & Affiliated Companies**

---

**ABS & Affiliated Companies**
**SIERRA Literacy Month**
*Day 7: Tokens, Cost & Context Window*

---

**Day 7: Tokens, Cost & Context Window**

- Tokens are small pieces of text — words, parts of words, punctuation (~4 characters, ~0.75 words; about 666 tokens per page)
- Every LLM request is priced on tokens processed — both input and output; tokens are inexpensive, ABS absorbs significant usage
- Models reprocess the entire conversation history with each message
- Long, scattered threads degrade answer quality — the model has to sort through noise to find what matters
- Focused threads = better answers. Cost savings is a secondary benefit.

**About tokens...**
Language models break text into smaller chunks (tokens) before processing it.
- Example: "language models" → [**Lan**][**guage**][**_mod**][**els**]
- One page ≈ 666 tokens

**Context window = working memory**
Think of the context window as the model's working memory — everything it can hold in mind at once while generating a response. Every token in your thread (prompts, responses, attached files, system instructions) counts against it.
- Current Sierra models: 200,000 to 2,000,000 tokens (~300 to 3,000 pages)
- A focused thread keeps working memory on what matters — a noisy thread wastes it on what doesn't
- *(We'll go deeper on what fills the context window in Week 3)*

**When switching topics, start a new thread — primarily for better answers, and secondarily to keep costs down.**

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
- This often occurs with insufficient context — it fills a gap based on patterns, not real data.
- This is why much of our focus is on building internal knowledge systems.

**Also watch for:**
- **Out-of-date responses** — Sierra can't know about events after its training cutoff; verify anything time-sensitive
- **Irrelevant responses** — if Sierra misses the point, it usually means more context is needed, not a smarter question

**Always review Sierra outputs before sending to clients — fluent does not mean accurate.**

[Diagram: Smiling face with star-shaped eyes inside a yellow circle, flanked by a blue input arrow on the left and an orange output arrow with an exclamation mark on the right.]

**ABS & Affiliated Companies**

---
