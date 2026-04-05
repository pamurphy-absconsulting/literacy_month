# Day 6 Redo — Key Points
**Slide title: "SIERRA's Tools for Adding Context"**
*Day 5 closed with: "we'll talk about strategies the CoE uses to bolster internal knowledge systems that the models can pull from." This day delivers on that — and corrects a misconception that's been implicit since Day 1.*

---

## The one idea to land

Sierra is not a model. It's a platform with secure access to various models — and a set of tools built around them to bring in the information those models don't have on their own.

---

## What to cover (in order)

**1. Correct the framing first (30 seconds)**
Sierra is not a model. The LLMs — Claude, GPT, and others — are what Sierra sends your information to for processing. Sierra is the platform: secure container, access layer, and a set of tools built specifically to make those models more useful in an ABS context.

Suggested line:
> "Sierra is not a model — it's a platform. It's what we built around the models to give you secure access and a set of tools. The model processes what you give it. Sierra's job is to make sure it has the right information to work with."

**2. The gap (one sentence)**
The models were trained on public data up to a cutoff. ABS-specific work — projects, rules, client data, internal procedures — none of that is in there by default. So Sierra has tools to fill that gap.

**3. The three tools — this is the core of the slide**

- **Web search** — Sierra can query the web for current or external information and pull it into context. You don't have to do this manually — Sierra handles the query and brings the result back in.

- **File attachments** — You upload a document, Sierra pulls from it to answer your question. The model isn't reading the whole file — it retrieves what's relevant based on what you ask. (More on this in a later video.)

- **Knowledge repositories** — CoE-built data sets Sierra can search automatically. When you ask something that relates to one of these sources, Sierra retrieves the relevant content and reasons over it — as if you had uploaded it yourself. HR is the one everyone can test right now.

**4. HR example — keep it concrete**
Ask Sierra about the ABS vacation policy. The model has no idea — that was never in its training data. But because we've built an HR knowledge repository, Sierra retrieves the relevant policy and answers correctly. That's the tool working. Try it.

**5. Close with the bridge**
In all three cases, the model only processes what's in front of it — what's in its context window. These tools exist to make sure the right information gets there. Next we'll talk about where all that information actually goes and what the constraint on it is.

---

## Slide layout suggestion
- **Title:** SIERRA's Tools for Adding Context
- **Replace the flow diagram** with a clean 3-item visual: Web Search / File Attachments / Knowledge Repositories — each with a one-line description
- **Keep the HR example** exactly as-is
- **Core Ideas box — rewrite to:**
  - Sierra is not a model — it's a platform built around the models with tools to bring in what they can't know on their own
  - These tools are expanding — the series covers how to use each of them

---

## What to cut vs. original
- Cut: training recap opener
- Cut: fine-tuning explanation
- Cut: "knowledge architectural approach" language
- Cut: the existing flow diagram (or repurpose it to show the 3 tools instead of the RAG-only flow)
- Keep: HR example
- Keep: the idea that Sierra retrieves and reasons, not just retrieves

---

## Tone
Direct. You're correcting a misconception and then explaining a system. Not academic — just clear. "Here's what Sierra actually is, here's what it has, here's what that looks like."

## Length target
~3.5 minutes
