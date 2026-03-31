# Video Review Notes — Days 1–8
*Updated after review of reference/docs_coe.md*

---

## Key Issues

### 1. "Neural nets fed text to find patterns" — said 5 times
Days 3, 4, 5, 6, and 8 all re-explain how LLMs were trained. Each time it was used as a setup before getting to the actual new topic. By Day 8 the audience has heard it five times. It was never egregious in isolation but it accumulates badly.

### 2. The apologetic "concepts not features" framing — said 4 times
Days 1, 3, 7, and 8 all include some version of: "we're focusing on fundamentals because the tech evolves fast and features could be obsolete." Said once in Day 1 it's a legitimate framing. Said four times it reads as defensive and makes the conceptual content feel like an apology rather than a deliberate choice. Drop it entirely from Day 9 onward.

### 3. Day 2 is structurally loose
The three-layer pyramid is a decent framework but the bottom layer (IT infrastructure) is a direct repeat of Day 1. The web search privacy detail is good but randomly placed inside the App Design layer. The Policy Compliance section punts to an exercise instead of delivering real content. Ends weakly.

### 4. Days 4 and 5 are both "what LLMs know" — one too many
Day 4 introduces the two-source framework (context vs. internal knowledge). Day 5 maps the specifics of what's inside internal knowledge. Each adds something new, but Day 5 opens with *another* training re-explanation before getting to the new content. The redundancy is worst here.

---

## Days Worth Redoing

### Day 4 — Recommended redo (goes out April 7)
**Problem:** Opens with a full re-explanation of how LLMs were trained before getting to the actual topic.
**Fix:** Open immediately with the framework — "There are exactly two types of knowledge available to the model. Here's what they are." Cut the training backstory entirely. The sky color example is good, keep it. The "no third source" close is good, keep it. This video should be 2 minutes, not 4.

### Day 5 — Recommended redo (goes out April 8)
**Problem:** Worst offender. The first half re-explains training *again* as setup. The real content — corporate IP, cutoff dates, what models don't know — is important and gets buried.
**Fix:** Open with the destination, not the backstory. "Models have real knowledge limits. Here's what they don't know and why it matters for your work at ABS." Lead with corporate IP. Cutoff dates. Deep domain knowledge creeping toward internal knowledge. No training recap.

### Day 2 — Redo only if time allows today (goes out April 2)
**Problem:** Structural looseness, repeats Day 1's IT layer, punts on policy compliance content.
**Fix:** Lead directly with the three layers as a crisp framework. Make IT Infrastructure one sentence (already covered in Day 1). Spend real time on policy compliance — what categories of content are restricted, what client contractual terms actually mean for day-to-day use. End clean.

---

## Days to Leave Alone

| Day | Reason |
|-----|--------|
| 1 | Good. Clean opening, right themes, strong close. |
| 3 | Training explanation IS the point on Day 3 — that's the lesson. |
| 6 | Best content of the batch. Static model point, HR RAG example, knowledge systems — all earned. |
| 7 | Least redundant. Tokens content is fine, the "start a new thread" advice is practical. |
| 8 | Hallucination content is solid. Close ("this is why we build internal knowledge systems") is the perfect setup for Week 4. |

---

## How to Cut the Redundancy Going Forward

**Rule for Days 9–22: never re-explain how LLMs were trained. Full stop.**

Day 9 opens with a transition, not a recap. Something like: "You now understand what Sierra is, how these models work, and their limits. That foundation is what makes everything from here practical rather than arbitrary. Let's use it." Then move directly into prompting.

When callbacks to earlier concepts are needed (e.g., "remember that context is all the model has — this is why specificity in prompting matters"), make them one sentence and forward-looking, not re-explanations.

**Drop the apologetic framing entirely.** The course is shifting to pragmatic content in Week 3. Don't announce it, don't apologize for the prior weeks, don't frame it as a contradiction. Just do it. The audience will appreciate both halves.

---

## Findings from docs_coe.md

### Factual issues in already-delivered videos

**Day 2 — data policy was too vague.** The actual policy has three specific categories:
- **Never permitted:** PII, ITAR/Export Restricted Data, Government Classified Data (any level)
- **Sometimes permitted:** Client data — depends on whether client accepted ABS T&Cs without modification. If on client paper, check with legal.
- **Always permitted:** ABS IP and internal data — BUT if produced under a client contract, may be considered client data (check with legal)

Patrick said "certain files are permitted, some aren't, check the exercise." Not enough. A redo should use these actual categories.

**Day 2 — audit point was never mentioned.** From the docs: *"Your prompts and responses are available only to you; however, they are monitored by system administrators and can be audited for proper business use."* Users should know this.

**Day 7 — cost framing should be rebalanced.** The docs explicitly say: *"Tokens are cheap. You can get a lot of work done for a few dollars."* The primary reason to start fresh threads is output quality (focused context = better answers), not cost. Cost should be secondary.

### What's confirmed correct
- ~4 chars per token / 0.75 words per token ✓
- Models are static, don't learn from conversations ✓
- OpenAI, Anthropic, xAI as providers ✓ (note: Google is not in the current model table)
- Web search uses targeted queries, doesn't dump full chat context to the web ✓
- Docs add one more detail: if Sierra suspects a web search query may contain confidential info, it asks for approval before sending — good detail for Day 12

### What's missing from the curriculum entirely

**eCFR — not in curriculum at all.** The Electronic Code of Federal Regulations knowledge repository is in Sierra (preview). For a maritime classification society, 46 CFR (shipping) and 33 CFR (Coast Guard) are core regulatory sources. Potentially one of the highest-value tools for ABS surveyors and engineers. Should be added to Days 17-18 alongside Plato (both are regulatory knowledge bases).

### Availability caveats the curriculum doesn't address
- **Plato:** "in preview and only available for some users" — curriculum dedicates two days to it. Slides need a caveat.
- **eCFR:** same, preview only.
- **SkillShare:** "by default, only enabled for ABS Group employees" — not Bureau, not Wavesight. Day 19 never mentions this. It needs to.

### If redoing Day 2, use this structure
1. Three layers (brief — bottom layer in one sentence, already covered Day 1)
2. Three data policy categories with specifics (PII, ITAR, Classified; client contract nuance; ABS IP)
3. Audit point — chats are private from other users but can be reviewed by admins
4. "Do I need to tell clients I'm using Sierra?" — check your contract or ask legal
5. Close: "Now that you know what's permitted and what's protected, the rest of this course is about how to use it."
