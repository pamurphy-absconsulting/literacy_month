Skip to main content
Docs
API reference
Blog
Log Out
Try SIERRA

Search...
Ctrl K

Getting started
Welcome
Feedback
SIERRA
About & FAQ
Data Policy
Releases
SIERRA Learning Series
Tango
About
Installation Guide
Releases
Watch a Demo
AI Tools
Code Generation

Getting started
Welcome!

Copy page

Welcome to the AI Center of Excellence Portal — your one-stop hub for practical AI at ABS.

Welcome Banner
This website exists to accelerate, guide, and consolidate the use of AI tools across ABS. The intended audience is threefold:
Frontline staff who want access to AI-powered tools
Coders who want to tap into production-ready AI models, agents, and knowledge repos
ABS leadership who want to see what we’re doing
If you work with data, models, integrations, or automation inside ABS, this is your source for code, APIs, models, documentation, and release notes — no presentations or marketing content here.
​
What you’ll find here
This website will provide the following content:
Announcements and release notes: timely posts about new AI services and endpoints, API and SDK updates, model deployments, and deprecations.
Technical documentation
API key management
Links to AI apps, tools, and training
Blog-style articles for inspiration
​
What we’re asking for
We hope that this site will help you access the power that AI brings. A few simple asks:
Try the apps that we build and promote — real adoption surfaces real problems and real wins. (It also helps us manage AI governance!)
Use the APIs in your solutions. Not a programmer? SIERRA can help you script basic solutions using the APIs without deep coding.
Tell us what breaks. If something is rough, we need to know — silence slows progress.
​
Our vision for this site
This website was originally conceived as a hub for ABS Consulting’s AI solutions. This scope expanded when Matthew Mowrer was nominated to lead the ABS-wide AI Center of Excellence. The vision remains the same: provide robust, generalized, modular solutions that enable AI-powered operations across the enterprise. AI is everywhere. At the AI Center of Excellence, we invest in best available solutions that we expect to produce a commercial return on investment. In some cases, these solutions may come from external vendors. In other cases, we will build our own. Regardless, we will use this site to help staff find the AI tools they need.
We have many upgrades and releases planned.
Was this page helpful?


Yes

No
Feedback
Next
Powered by
This documentation is built and hosted on Mintlify, a developer documentation platform
Assistant


Responses are generated using AI and may contain mistakes.
Suggestions

Is SIERRA safe for confidential information?
How do I get access to Tango?
What tools and apis are available for developers?
Ask a question...


Contact support

---


Skip to main content
Docs
API reference
Blog
Log Out
Try SIERRA

Search...
Ctrl K

Getting started
Welcome
Feedback
SIERRA
About & FAQ
Data Policy
Releases
SIERRA Learning Series
Tango
About
Installation Guide
Releases
Watch a Demo
AI Tools
Code Generation

SIERRA
About & FAQ

Copy page

Learn about our internal AI assistant and explore tips and tricks for getting the most out of it.

​
What is SIERRA?
SIERRA is an AI chat assistant designed to support the employees of ABS. The AI Center of Excellence developed SIERRA to provide employees with secure access to private large-language models (LLMs). Wherever feasible, we will identify opportunities to expand SIERRA’s capabilities in ways that are specific to our operations and expertise.
Contextualized
Access to ABS tools and data
Secure & Private
Isolation from the outside world
​
Training Videos
​
SIERRA Learning Series
These videos are designed to empower learners with practical skills in using SIERRA, covering everything from foundational concepts to advanced techniques. Dive in and elevate your productivity!
Watch SIERRA Learning Series
​
How to Research and Write Using Generative AI Tools
This LinkedIn Learning video provides a great overview of how to work with ChatGPT generate content. In particular, Section 1: Overview of Working with AI is essential viewing, particularly the framework he introduced for writing an effective prompt for AI. If you only watch one thing, it should be this section.
Watch on LinkedIn Learning
​
Learning ChatGPT for Business Analysis
This LinkedIn Learning video provides an overview of ChatGPT basics before introducing several common business use cases. While generic, it should give you some ideas about what is possible with ChatGPT and how you can tailor it to your work.
Watch on LinkedIn Learning
​
Prompt Engineering: How to Talk to the AIs
This LinkedIn Learning video provides a good summary of the core concepts of large-language models (LLMs) before diving into a detailed exploration of how to develop prompts for various applications.
Watch on LinkedIn Learning
​
Models
SIERRA makes the latest models from frontier providers such as OpenAI, Anthropic, and xAI available to ABS employees in a private environment in Microsoft Azure. Below is a table of the models currently available.
Model	Description	Reasoning	Context
(tokens)	Training
Cutoff	Input
per 1M tokens	Output
per 1M tokens
gpt-5-1	OpenAI’s most capable model	Yes	400K	September 2024	$1.25	$10.00
claude-sonnet-4-5	Anthropic’s balanced model	Yes	200K	January 2025	$3.00	$15.00
claude-opus-4-5	Anthropic’s most capable model	Yes	1M	March 2025	$15.00	$75.00
grok-4-fast-non-reasoning	xAI’s model tuned for speed and large context	No	2M	May 2025	$0.43	$1.73
​
What are tokens?
Tokens are the basic units of text that AI models process. ABS pays for tokens, not words. Roughly, 1 token equals 4 characters or 0.75 words in English. For example, “Hello world” is about 2 tokens. One page of size 12 Arial font is ~666 tokens. The pricing shown is per 1 million tokens, which is approximately 750,000 words or 4 million characters.
Tokens are cheap. You can get a lot of work done for a few dollars.
​
What is the context window?
A model’s context window is the maximum amount of text or data (usually measured in tokens) that it can process at one time, including both input and output. It determines how much information the model can “remember” or consider when generating a response. For example, a larger context window allows the model to handle longer conversations or documents, while a smaller one limits it to shorter inputs.
​
What is the training cutoff date?
The training cutoff date indicates when the model’s training data ends. Models cannot access information or events that occurred after this date. For example, a model with an April 2024 cutoff won’t know about events, news, or developments that happened after April 2024.
​
Tools
Tools extend SIERRA’s capabilities by allowing it to access ABS knowledge repositories and take actions. SIERRA does its best to determine if it should use a tool for a given task, but you can always ask it to use or not use a tool directly.
​
Memories
The memories tool allows SIERRA to record information to a database that you ask it to remmeber. That way it will retain that context across the boundary of threads and workspaces.
​
File Search
Several file search tools allow SIERRA to list the files available to its current context, read the content of individual files, and search all files on a thread or workspace.
​
Web Search
The web search tools allow SIERRA to crawl individual URLs, execute web searches, and spawn asynchronous research report generation. If SIERRA thinks a query that’s about to be sent to the search API may contain confidential information, it will ask you to approve or discard the search.
​
SkillShare Knowledge Repository
The SkillShare tool allows SIERRA to search ABS Group’s skillset and resume database to find employees with specific qualifications, experience, or skills. By default, it is only enabled for ABS Group employees.
​
HR Knowledge Repository
Search for information inside HR policy documents and benefits guides, specific to a company (Bureau/Group/Wavesight) and country.
​
Plato Knowledge Repository
Search ABS rules and maritime regulations. This tool is in preview and is only available for some users.
​
eCFR Knowledge Repository
Search a curated index of the Electronic Code of Federal Regulations. This tool is in preview and is only available for some users.
If you have an idea for a new tool, please let us know.
​
Workspaces
Workspaces provide a streamlined interface for managing workflows you frequently perform. Workspaces offer several features that are not available in regular chats:
Files: Attachments that are consistently used within workspace chats.
Instructions: Prompt instructions or specialized knowledge applied to every chat within the workspace.
Sharing: Workspaces can be shared with anyone who has access to SIERRA. (Note: Individual chats are not shared.)
Task Prompts: Specific, reusable instructions built by workspace users to perform repeatable actions consistently.
Read more about workspaces in SIERRA here.
​
Possible Use Cases
Project Content Management: Store and reference files and information related to a specific project.
Repetitive Document Extractions: Save commonly used prompts in the instructions box. For example, instead of repeatedly typing the same prompt, store it in the instructions and submit each document to a thread with a simple command like “analyze this.”
Topic-Specific Knowledge Repository: Use workspaces to query large sets of files related to a topic. SIERRA can apply search algorithms to summarize information based on your query.
Personal Trainer/Advisor: Provide a workspace with information about yourself (e.g., results from a personality or professional strengths assessment) to receive personalized advice.
Whether to take advice from a computer is up to you.
​
Important Guidelines
When working with workspaces, keep these best practices in mind:
Instructions Placement: Only include instructions in the instructions box. SIERRA will probably not follow instructions embedded within workspace files.
Instruction Length: Shorter instructions tend to perform better than very long ones.
​
Privacy
​
Is the information I provide in prompts to SIERRA available to anyone else?
The inputs and outputs you provide to SIERRA are NOT available to Microsoft, OpenAI, Meta, xAI, or any other company. Your prompts and responses are NOT used to improve the models, and they are NOT used to improve any Microsoft or 3rd party products or services. Your prompts and responses are available only to you; however, they are monitored by system administrators and can be audited for proper business use.
​
Is SIERRA suitable for ABS or client proprietary data?
Yes – SIERRA is hosted in a secure environment where you can provide ABS and client information in the prompts if it complies with the Data Policy.
​
Do I need to inform customers that I am using SIERRA?
Check with your manager or ask the legal department if there are any contractual provisions restricting use of AI or requiring disclosure of use of AI.
​
Risks
Inaccurate Responses
Even though it sounds authoritative, SIERRA may not always provide accurate or contextually appropriate responses. These are called “hallucinations” and are a major challenge when using LLMs. You must review all content generated by SIERRA.
Irrelevant Responses
SIERRA may not fully understand the context or nuances of a specific situation, particularly in some of the niche domains where we operate. This can lead to responses that are not relevant. You can provide additional information in the prompt to provide more context and instructions.
Data Leakage
Sharing sensitive or confidential information with SIERRA. Refer to the data policy before using it in prompts.
Out-of-date Responses
The models used by SIERRA are trained on a diverse range of internet data up until each model’s respective cutoff date. It lacks knowledge of recent events. This is particularly important when using in research tasks or on emerging topics.
Was this page helpful?


Yes

No
Feedback
Previous
Data Policy
Next
Powered by
This documentation is built and hosted on Mintlify, a developer documentation platform
Assistant


Responses are generated using AI and may contain mistakes.
Suggestions

Is SIERRA safe for confidential information?
How do I get access to Tango?
What tools and apis are available for developers?
Ask a question...


Contact support

About & FAQ - ABS AI Center of Excellence

---


> ## Documentation Index
> Fetch the complete documentation index at: https://docs.absconsulting.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Data Policy

> It is up to you to ensure that you are only inputting data which we are permitted to use in the operation of this tool.

There are three categories of use permissions to be aware of:

1. **Never permitted for use**

   Special categories of data which are regulated by law, which we are never permitted to use in this tool include:

   * Personally Identifiable Information (PII)
   * ITAR or other Export Restricted Data
   * Government Classified Data (any level of classification)
   * If the client has accepted the current ABS T\&Cs, without modification, then use is permitted
   * If the contract is on client paper, please check with legal
2. **Sometimes permitted for use**
   * Whether or not we can use client data in this tool will be governed by the terms of the applicable client contract. Additionally, the contract may permit some forms of use within the tool, but not others
3. **Always permitted for use**
   * It is always permissible to use ABS intellectual property or internal data in this tool
   * HOWEVER, please be sure that the data in question is in fact ABS data. If the data was produced in the performance of a client contract, then it may be considered client data. Please check with legal if you are unsure


Built with [Mintlify](https://mintlify.com).


---

> ## Documentation Index
> Fetch the complete documentation index at: https://docs.absconsulting.ai/llms.txt
> Use this file to discover all available pages before exploring further.

# Releases

> Product updates and bug fixes.

## What's Next?

We're continuously working on improvements. Have a feature request? Is something not working as expected? Please <span class="white-link">[let us know](/feedback)</span>.

<div class="release-update">
  <Update label="March 16, 2026" tags={["Model Upgrades", "Plato", "Knowledge Repos", "Images", "Improvements"]}>
    * Gated Release: Plato UAT
    * Gated Release: image generation/interpretation capability
    * Refreshed models (GPT 5-4, Claude Sonnet 4-6, Claude Opus 4-6)
    * Updated and consolidated chatbar UI to accomodate new features
    * Distinguished modes from knowledge bases in UI
  </Update>
</div>

<div class="release-update">
  <Update label="February 26, 2026" tags={["Workspaces", "Bug Fixes"]}>
    * Added warning message to workspace memories
    * Improved saving functionality of workspace settings
    * Bug fix: Improved handling of declined memories
    * Bug fix: Fixed issue where saved settings overwrite workspace context
  </Update>
</div>

<div class="release-update">
  <Update label="February 25, 2026" tags={["Workspaces"]}>
    * Added workspace memories and task prompts
    * UX updates to improve workspace settings, context, and files
  </Update>
</div>

<div class="release-update">
  <Update label="February 13, 2026" tags={["Analytics", "Bug Fixes"]}>
    * Improved analytics leaderboard with department and company filtering
    * Admin leaderboard view with advanced filtering and data views
    * Admin tab with cost, user, and detailed token views
    * Live data across tabs for current date ranges
    * Bug fix: SIERRA stability enhancements
  </Update>
</div>

<div class="release-update">
  <Update label="December 12, 2025" tags={["Tools", "Knowledge Repos"]}>
    * Added HR knowledge repository
    * Added research report generation to web tools
    * Added eCFRs knowledge repository (in preview, only accessible to some users)
  </Update>
</div>

<div class="release-update">
  <Update label="December 2, 2025" tags={["Plato", "Improvements", "Bug Fixes"]}>
    * Added Plato knowledge repository (in preview, only accessible to some users)
    * Added context used donut to chatbar
    * Fixed context trimming when context overflows the selected model's capability
  </Update>
</div>

<div class="release-update">
  <Update label="November 27, 2025" tags={["Model Upgrades", "Tools", "Workspaces"]}>
    * Refreshed models (GPT 5-1, Claude Sonnet 4-5, Claude Opus 4-5, Grok 4 Fast)
    * Added web search and web crawl tools
    * Improved agentic loop of workspaces
  </Update>
</div>

<div class="release-update">
  <Update label="November 26, 2025" tags={["Tools"]}>
    * Moved thread and workspace file handling to Documents Service
    * Improved file search tools
  </Update>
</div>

<div class="release-update">
  <Update label="August 15, 2025" tags={["Model Upgrades", "Improvements"]}>
    * Added gpt-auto, gpt-5-thinking, and gpt-5-mini models
    * Improved copy message to clipboard functionality
  </Update>
</div>

<div class="release-update">
  <Update label="July 25, 2025" tags={["Model Upgrades", "Personalization"]}>
    * Modify appearance, style, default tools, and more in user settings
    * Create and manage memories to help SIERRA remember important information
    * Added Claude Sonnet 4 and Claude Opus 4 models
  </Update>
</div>

<div class="release-update">
  <Update label="July 22, 2025" tags={["Analytics"]}>
    * View analytics for your requests and token usage
    * Minor bug fixes and improvements
  </Update>
</div>

<div class="release-update">
  <Update label="July 18, 2025" tags={["Improvements"]}>
    * Move chats in and out of workspaces via button or drag & drop
    * Upload files to chatbar via drag and drop
    * Upload files to workspace file dialog via drag and drop
    * Minor bug fixes and improvements
  </Update>
</div>

<div class="release-update">
  <Update label="July 15, 2025" tags={["Analytics"]}>
    * View the top 50 users by request count in the leaderboard
  </Update>
</div>

<div class="release-update">
  <Update label="July 10, 2025" tags={["Bug Fixes"]}>
    * Bug Fix: Empty ai messages in chat
    * Bug Fix: Inability to grab scrollbar under chatbar
    * Bug Fix: Table and code block styles in non-default mode
  </Update>
</div>

<div class="release-update">
  <Update label="July 07, 2025" tags={["Model Upgrades", "Improvements", "Bug Fixes"]}>
    * Added grok-3 and grok-3-mini models
    * Added regenerate button to chat
    * Updated system prompt to include more context about SIERRA's environment
    * Added ability to disable tools and removed "@" tool referencing
    * Fresh UI and look and feel
    * Bug fix: chat "hanging" in streaming state after completing response
  </Update>
</div>


Built with [Mintlify](https://mintlify.com).

---



