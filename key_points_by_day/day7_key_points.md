# Day 7 Redo — Key Points
**Topic: Tokens & Context Windows**
*Day 6 closed with: "retrieved content enters the context window and the model reasons over it." Day 7 builds out what the context window actually is and why it's a constraint. Day 8 opens with: "in the last one I was focusing on how it processes information — working token by token." Must deliver that.*

---

## The one idea to land

The model can only hold so much at once. That limit — the context window — is why you can't just make everything available. Understanding it changes how you work.

---

## What to cover (in order)

**1. Open with the question the audience is already asking**
We understand what the model is doing — processing text. We understand it needs relevant information to do that well. We've got tools to bring more in. So you might be asking — why not just make everything available? The answer is constraints. The model can only hold so much at once. That limit is called the context window.

**2. Tokens — one paragraph, no more**
To understand the constraint, you need to know how we measure text. The model doesn't measure in words or pages — it measures in tokens. Small chunks of text — words, parts of words, punctuation — roughly 666 per page. Each token gets represented as a mathematical coordinate — that's how the model understands relationships between words. You don't need to go deeper than that. What matters: 666 tokens per page, and there's a cap on how many fit.

**3. Context window = working memory**
Everything the model can hold and process at once — your prompt, conversation history, files you attached, anything retrieved from a knowledge repo. Large, but not infinite. Do NOT cite specific token counts — they're model-dependent, version-dependent, and Sierra starts degrading well before any advertised ceiling. The point is the constraint, not the number. "Large, but not infinite" is enough.

**4. The quality constraint**
It's not just about hitting a hard limit. The model processes everything in that window on every message. Fill it with irrelevant content — old topics, tangents, noise — and it has to sift through all of that to find what actually matters. That degrades the response. Focused, relevant context gets better results.

**5. The practical habit: focused threads**
Start a new chat when you switch topics. Keep threads tight and on one subject. Not a rule — just how you get better answers.

**6. The failure mode — handoff to Day 8**
Long conversations push earlier content out of the window — the model loses context it once had. Key information introduced early may be gone by the time you reference it later. That's one of the ways things go wrong — and that's what we cover next.

---

## How this fits the course progression

| Day | Concept | Relationship |
|---|---|---|
| Day 4 | What the model knows vs. doesn't | Establishes the gap |
| Day 5 | Context is the lever you control | You fill the gap |
| Day 6 | Sierra's tools for adding context | Sierra helps fill the gap automatically |
| **Day 7** | **Context window — the constraint on all of it** | **Why you can't just add everything** |
| Day 8 | Hallucinations | What happens when the constraint isn't managed |
| Day 9+ | Prompting, files, workspaces | How to work well within these constraints |

Day 7 is the hinge. Days 4-6 build up the idea that context matters and that tools exist to bring it in. Day 7 explains why you still have to be deliberate about it — there's a limit, noise costs you quality, and failure to manage it leads directly to the problems Day 8 describes. Everything from Day 9 onward (prompting strategy, file handling, workspaces) is essentially answering: "given these constraints, how do you work effectively?"

---

## What to cut vs. original
- Cut: extended embeddings visual and coordinate number display
- Cut: specific token count ranges — "large, but not infinite" only
- Cut: "I know I'm bringing this in last minute" framing
- Keep: 666 tokens per page anchor
- Keep: mathematical coordinate reference — one clause, not explained
- Keep: working memory analogy
- Keep: noise/quality argument
- Keep: focused threads habit
- Keep: failure mode — direct setup for Day 8

---

## Tone
Direct. Lead with the question, answer it cleanly. Don't over-explain tokens — get to the constraint fast and spend most of the time on what it means in practice.

## Length target
~3.5 minutes
