# SIERRA Literacy Month — Live Demo Arc
## Days 17–22

---

## Overview

Days 1–16 are instructional videos with exercises. Days 17–22 are live screen recordings inside Sierra — no slides, no lecture. Each demo is a real workflow solved in real time.

**Key principle:** The audience has already covered all the concepts. These demos are not re-explanations. They are the concepts applied to work that looks like their work.

**Workspace note:** Workspaces and task modes are built live during the relevant demos. The live build is the demonstration — it shows the audience exactly how to replicate it, and it lets the meta-prompt shortcut from Demo 1 pay off later (use Sierra to write the task mode instructions from a rough description).

---

## Demo 1 — Prompting Fundamentals

**What it covers:** Days 9, 10

**The arc:**
1. Start with a vague, real work question — the kind someone would actually type
2. Show how the output falls short
3. Rebuild the prompt using the four ingredients: role, task, context, format
4. Show the difference in output
5. End with the meta-prompt shortcut — describe the task rough, ask Sierra to structure the prompt

**No workspace. No files.** Just the basic skill that underlies everything else.

**Key teaching moment:** The meta-prompt shortcut. Describe what you need in rough stream-of-consciousness language, ask Sierra to structure it into a clean prompt. This is how most prompts should be written.

**Note:** This demo will feel simpler than what follows. Acknowledge it — "this is the foundation; keep it in mind as we get into more complex work."

---

## Demo 2 — Context and Memories

**What it covers:** Days 5, 14

**The arc:**
1. Run a real work prompt in a cold thread — Sierra knows nothing about you
2. Note where the output is generic or off-target
3. Set memories: role, team/division, output preferences, operating context
4. Run the same prompt again
5. Show how the output is grounded and tailored before you typed a single extra word

**Key teaching moment:** "Context is the lever you control" becomes visible. The improvement happens before the prompt, not inside it.

**Note:** This is a shorter demo. Could be tightened into a segment within Demo 1, or kept as a standalone if the before/after contrast is strong enough to carry it.

---

## Demo 3 — Working with an Uploaded Document

**What it covers:** Days 11, 12, 13

**The arc:**
1. Upload a real operational document (ideally one with complexity — messy tables, a schedule, or a scanned section)
2. Preview the conversion before attaching — show the audience what Sierra actually ingested
3. Run several different queries against the same file
4. Show how different questions surface different sections — the whole file is not in every response
5. If possible: show the same prompt against a cleaner vs. messier version of the same content

**Key teaching moment:** The conversion preview. Most people have never seen what their PDF becomes. If the conversion is incomplete or garbled, the prompt won't fix it — check your inputs.

**Note:** Consider including a phased extraction segment here — one pass for high-level anchors, a second pass with those anchors injected back in for granular fields. This is the Day 11 content and it's conspicuously absent from the other demos. Even a short sequence (2 passes on a contract or scope of work) closes that loop.

---

## Demo 4 — Root Cause Analysis, Start to Finish

**What it covers:** Days 10, 14, 15, 16

**The arc:**

*Part A — Build the workspace live*
1. Open a new workspace for an incident investigation context
2. Set workspace context (background, methodology, output standards)
3. Upload relevant files (incident report, witness statements, logs, procedure)
4. Write the RCA task mode — use the meta-prompt shortcut: describe the workflow rough, ask Sierra to structure the task mode instructions
5. Brief the audience on what was just built and why

*Part B — Run it*
1. Invoke the RCA task mode on the incident file
2. Walk through the structured output: incident classification, 5 Whys, regulatory gaps, corrective actions
3. Review the output as you would in practice — show the "you review before the next step begins" habit

*Part C — Sequential follow-ups*
1. Turn the RCA into a formal investigation report
2. Draft specific SMS procedure updates based on the findings
3. Produce a one-page fleet safety circular for crew

**Key teaching moment:** The sequential workflow in action. Each output is reviewed before the next prompt is issued. This is Day 10's "you architect, Sierra executes" made concrete and visible across a realistic 4-step deliverable chain.

---

## Demo 5 — Procedure Gap Analysis

**What it covers:** Days 9, 10, 11, 15, 16

**The arc:**

*Part A — Build the workspace and validator task mode live*
1. Set up workspace context for emergency response procedure review
2. Write the gap analysis task mode — structured against 11 completeness elements: triggering conditions, roles, communications, escalation, drills, regulatory references, etc.
3. Upload the procedure to be reviewed

*Part B — Run the validator*
1. Run the procedure through the task mode
2. Walk through the prioritized gap list
3. Show how the structured extraction pattern (Day 11) is being applied to a document review task

*Part C — The rewrite step*
1. Accept or modify the gap list
2. Ask Sierra to thread the accepted changes into the procedure with markers showing exactly what was added
3. Show the output — tracked changes, auditable, ready for review

**Key teaching moment:** Structured extraction applied to document review. The output isn't prose — it's a prioritized list tied to specific elements, followed by a controlled rewrite. The markers are the evidence-backed output principle from Day 11 made practical.

---

## Demo 6 — Training Requirements from a Crew Roster

**What it covers:** Days 9, 10, 11, 12, 15, 16

**The arc:**

*Part A — Build the workspace live*
1. Set up workspace context for crew certification and training compliance
2. Upload reference material to ground the output (STCW requirements table or certification reference document — critical for accuracy)
3. Write the training matrix task mode: by rank, vessel type, certification requirements, refresh intervals, gap analysis

*Part B — Run it*
1. Upload the crew roster
2. Invoke the task mode
3. Walk through the full STCW training matrix: certifications required by rank, vessel-type-specific training, refresh intervals, who is missing what, what is expiring

**Key teaching moment:** Output that would take significant manual research time, produced in a single structured workflow. The audience will immediately recognize this as real, useful work product.

**Important:** Ground this with an attached reference document. STCW requirements are specific and a confident hallucination is a real risk if Sierra is working from training data alone. The reference doc is not optional — it's the Day 13 lesson ("inputs shape outputs") applied in practice.

---

## Teaching Lines

Short, memorable lines to narrate during recordings. These should be said out loud while working, not as lecture — just as natural asides.

- *"The model is not the product. Sierra is the product."*
- *"If it was never on the public internet, the model doesn't know it."*
- *"Context is the lever we control."*
- *"The goal is not one perfect mega-prompt — it's a controlled sequence."*
- *"Evidence first. Interpretation second."*
- *"If the output is wrong, check the source before blaming the model."*
- *"Fluent is not the same as correct."*
- *"A focused thread beats a sprawling one."*
- *"If I'm going to do this workflow twice, it should probably become a task mode."*
- *"I'm reviewing this before I move to the next step — that's the habit."*

---

## What Not to Demo

- Generic email drafting
- "Summarize this article"
- Brainstorming with no context
- Simple one-file Q&A with a clean document
- "Write 10 bullet points about X"
- Anything where the setup and the output are roughly equivalent in complexity

---

## Production Notes

- **Each demo that involves a workspace should build it live.** The live build shows the audience how to replicate it. Pre-built workspaces look like magic and undercut the point.
- **Each complex demo needs a clear "setup is done, now watch" transition.** Building workspace context, memories, and a task mode takes time — give the audience a verbal signal before you run the actual workflow so they know what phase they're in.
- **The meta-prompt shortcut from Demo 1 should recur.** When writing task mode instructions in Demos 4, 5, and 6, use Sierra to structure them from a rough description. This makes Demo 1 pay off later.
- **Demos 4, 5, and 6 are the strongest material.** If bandwidth is limited, prioritize these.
