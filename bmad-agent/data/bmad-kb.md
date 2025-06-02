# BMAD Knowledge Base

## INDEX OF TOPICS

- [BMAD Knowledge Base](#bmad-knowledge-base)
  - [INDEX OF TOPICS](#index-of-topics)
  - [BMAD METHOD - CORE PHILOSOPHY](#bmad-method---core-philosophy)
  - [BMAD METHOD - AGILE METHODOLOGIES OVERVIEW](#bmad-method---agile-methodologies-overview)
    - [CORE PRINCIPLES OF AGILE](#core-principles-of-agile)
    - [KEY PRACTICES IN AGILE](#key-practices-in-agile)
    - [BENEFITS OF AGILE](#benefits-of-agile)
  - [BMAD METHOD - ANALOGIES WITH AGILE PRINCIPLES](#bmad-method---analogies-with-agile-principles)
  - [BMAD METHOD - TOOLING AND RESOURCE LOCATIONS](#bmad-method---tooling-and-resource-locations)
  - [BMAD METHOD - COMMUNITY AND CONTRIBUTIONS](#bmad-method---community-and-contributions)
    - [Licensing](#licensing)
  - [BMAD METHOD - ETHOS \& BEST PRACTICES](#bmad-method---ethos--best-practices)
  - [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities)
  - [NAVIGATING THE BMAD WORKFLOW - INITIAL GUIDANCE](#navigating-the-bmad-workflow---initial-guidance)
    - [STARTING YOUR PROJECT - ANALYST OR PM?](#starting-your-project---analyst-or-pm)
    - [UNDERSTANDING EPICS - SINGLE OR MULTIPLE?](#understanding-epics---single-or-multiple)
  - [GETTING STARTED WITH BMAD](#getting-started-with-bmad)
    - [Initial Project Setup](#initial-project-setup)
    - [Exporting Artifacts from AI Platforms](#exporting-artifacts-from-ai-platforms)
    - [Document Sharding](#document-sharding)
    - [Utilizing Dedicated IDE Agents (SM and Dev)](#utilizing-dedicated-ide-agents-sm-and-dev)
    - [When to Use the BMAD IDE Orchestrator](#when-to-use-the-bmad-ide-orchestrator)
  - [SUGGESTED ORDER OF AGENT ENGAGEMENT (TYPICAL FLOW)](#suggested-order-of-agent-engagement-typical-flow)
  - [HANDLING MAJOR CHANGES](#handling-major-changes)
  - [IDE VS UI USAGE - GENERAL RECOMMENDATIONS](#ide-vs-ui-usage---general-recommendations)
    - [CONCEPTUAL AND PLANNING PHASES](#conceptual-and-planning-phases)
    - [TECHNICAL DESIGN, DOCUMENTATION MANAGEMENT \& IMPLEMENTATION PHASES](#technical-design-documentation-management--implementation-phases)
    - [BMAD METHOD FILES](#bmad-method-files)
  - [LEVERAGING IDE TASKS FOR EFFICIENCY](#leveraging-ide-tasks-for-efficiency)
    - [PURPOSE OF IDE TASKS](#purpose-of-ide-tasks)
    - [EXAMPLES OF TASK FUNCTIONALITY](#examples-of-task-functionality)

## BMAD METHOD - CORE PHILOSOPHY

**STATEMENT:** "Vibe CEO'ing" is about embracing the chaos, thinking like a CEO with unlimited resources and a singular vision, and leveraging AI as your high-powered team to achieve ambitious goals rapidly. The BMAD Method (Breakthrough Method of Agile (ai-driven) Development), with the integrated "Bmad Agent", elevates "vibe coding" to advanced project planning, providing a structured yet flexible framework to plan, execute, and manage software projects using a team of specialized AI agents.

**DETAILS:**

- Focus on ambitious goals and rapid iteration.
- Utilize AI as a force multiplier.
- Adapt and overcome obstacles with a proactive mindset.

## BMAD METHOD - AGILE METHODOLOGIES OVERVIEW

### CORE PRINCIPLES OF AGILE

- Individuals and interactions over processes and tools.
- Working software over comprehensive documentation.
- Customer collaboration over contract negotiation.
- Responding to change over following a plan.

### KEY PRACTICES IN AGILE

- Iterative Development: Building in short cycles (sprints).
- Incremental Delivery: Releasing functional pieces of the product.
- Daily Stand-ups: Short team meetings for synchronization.
- Retrospectives: Regular reviews to improve processes.
- Continuous Feedback: Ongoing input from stakeholders.

### BENEFITS OF AGILE

- Increased Flexibility: Ability to adapt to changing requirements.
- Faster Time to Market: Quicker delivery of valuable features.
- Improved Quality: Continuous testing and feedback loops.
- Enhanced Stakeholder Engagement: Close collaboration with users/clients.
- Higher Team Morale: Empowered and self-organizing teams.

## BMAD METHOD - ANALOGIES WITH AGILE PRINCIPLES

The BMAD Method, while distinct in its "Vibe CEO'ing" approach with AI, shares foundational parallels with Agile methodologies:

- **Individuals and Interactions over Processes and Tools (Agile) vs. Vibe CEO & AI Team (BMAD):**

  - **Agile:** Emphasizes the importance of skilled individuals and effective communication.
  - **BMAD:** The "Vibe CEO" (you) actively directs and interacts with AI agents, treating them as a high-powered team. The quality of this interaction and clear instruction ("CLEAR_INSTRUCTIONS", "KNOW_YOUR_AGENTS") is paramount, echoing Agile's focus on human elements.

- **Working Software over Comprehensive Documentation (Agile) vs. Rapid Iteration & Quality Outputs (BMAD):**

  - **Agile:** Prioritizes delivering functional software quickly.
  - **BMAD:** Stresses "START_SMALL_SCALE_FAST" and "ITERATIVE_REFINEMENT." While "DOCUMENTATION_IS_KEY" for good inputs (briefs, PRDs), the goal is to leverage AI for rapid generation of working components or solutions. The focus is on achieving ambitious goals rapidly.

- **Customer Collaboration over Contract Negotiation (Agile) vs. Vibe CEO as Ultimate Arbiter (BMAD):**

  - **Agile:** Involves continuous feedback from the customer.
  - **BMAD:** The "Vibe CEO" acts as the primary stakeholder and quality control ("QUALITY_CONTROL," "STRATEGIC_OVERSIGHT"), constantly reviewing and refining AI outputs, much like a highly engaged customer.

- **Responding to Change over Following a Plan (Agile) vs. Embrace Chaos & Adapt (BMAD):**

  - **Agile:** Values adaptability and responsiveness to new requirements.
  - **BMAD:** Explicitly encourages to "EMBRACE_THE_CHAOS," "ADAPT & EXPERIMENT," and acknowledges that "ITERATIVE_REFINEMENT" means it's "not a linear process." This directly mirrors Agile's flexibility.

- **Iterative Development & Incremental Delivery (Agile) vs. Story-based Implementation & Phased Value (BMAD):**

  - **Agile:** Work is broken down into sprints, delivering value incrementally.
  - **BMAD:** Projects are broken into Epics and Stories, with "Developer Agents" implementing stories one at a time. Epics represent "significant, deployable increments of value," aligning with incremental delivery.

- **Continuous Feedback & Retrospectives (Agile) vs. Iterative Refinement & Quality Control (BMAD):**
  - **Agile:** Teams regularly reflect and adjust processes.
  - **BMAD:** The "Vibe CEO" continuously reviews outputs ("QUALITY_CONTROL") and directs "ITERATIVE_REFINEMENT," serving a similar function to feedback loops and process improvement.

## BMAD METHOD - TOOLING AND RESOURCE LOCATIONS

Effective use of the BMAD Method relies on understanding where key tools, configurations, and informational resources are located and how they are used. The method is designed to be tool-agnostic in principle, with agent instructions and workflows adaptable to various AI platforms and IDEs.

- **BMAD Knowledge Base:** This document (`bmad-agent/data/bmad-kb.md`) serves as the central repository for understanding the BMAD method, its principles, agent roles, and workflows.
- **Orchestrator Agents:** A key feature is the Orchestrator agent (AKA "BMAD"), a master agent capable of embodying any specialized agent role.
  - **Web Agent Orchestrator:**
    - **Setup:** Utilizes a Node.js build script (`build-web-agent.js`) configured by `build-web-agent.cfg.js`.
    - **Process:** Consolidates assets (personas, tasks, templates, checklists, data) from an `/bmad-agent` into a `build_dir`, default: `/build/`.
    - **Output:** Produces bundled asset files (e.g., `personas.txt`, `tasks.txt`), an `agent-prompt.txt` (from `orchestrator_agent_prompt`), and an `agent-config.txt` (from `agent_cfg` like `web-bmad-orchestrator-agent.cfg.md`).
    - **Usage:** The `agent-prompt.txt` is used for the main custom web agent instruction set (e.g., Gemini 2.5 Gem or OpenAI Custom GPT), and the other build files are attached as knowledge/files.
  - **IDE Agent Orchestrator (`ide-bmad-orchestrator.md`):**
    - **Setup:** Works without a build step, dynamically loading its configuration.
    - **Configuration (`ide-bmad-orchestrator.cfg.md`):** Contains a `Data Resolution` section (defining base paths for assets like personas, tasks) and `Agent Definitions` (Title, Name, Customize, Persona file, Tasks).
    - **Operation:** Loads its config, lists available personas, and upon user request, embodies the chosen agent by loading its persona file and applying customizations.
    - The `ide-bmad-orchestrator` file contents can be used as the instructions for a custom agent mode. The agent supports a `*help` command that can help guide the user. The agent relies on the existence in the bmad-agent folder being at the root of the project.
    - The `ide-bmad-orchestrator` is not recommended for generating stories or doing development. While it CAN become those agents, its HIGHLY recommended to instead use the dedicated dev.ide.md or sm.ide.md as individual dedicated agents. The will use up less context overhead and are going to be used the most frequently.
- **Standalone IDE Agents:**
  - Optimized for IDE environments (e.g., Windsurf, Cursor), often under 6K characters (e.g., `dev.ide.md`, `sm.ide.md`).
  - Can directly reference and execute tasks.
- **Agent Configuration Files:**
  - `web-bmad-orchestrator-agent.cfg.md`: Defines agents the Web Orchestrator can embody, including references to personas, tasks, checklists, and templates (e.g., `personas#pm`, `tasks#create-prd`).
  - `ide-bmad-orchestrator.cfg.md`: Configures the IDE Orchestrator, defining `Data Resolution` paths (e.g., `(project-root)/bmad-agent/personas`) and agent definitions with persona file names (e.g., `analyst.md`) and task file names (e.g., `create-prd.md`).
  - `web-bmad-orchestrator-agent.md`: Main prompt for the Web Orchestrator.
  - `ide-bmad-orchestrator.md`: Main prompt/definition of the IDE Orchestrator agent.
- **Task Files:**
  - Located in `bmad-agent/tasks/` (and sometimes `bmad-agent/checklists/` for checklist-like tasks).
  - Self-contained instruction sets for specific jobs (e.g., `create-prd.md`, `checklist-run-task.md`).
  - Reduce agent bloat and provide on-demand functionality for any capable agent.
- **Core Agent Definitions (Personas):**
  - Files (typically `.md`) defining core personalities and instructions for different agents.
  - Located in `bmad-agent/personas/` (e.g., `analyst.md`, `pm.md`).
- **Project Documentation (Outputs):**
- **Project Briefs:** Generated by the Analyst agent.
- **Product Requirements Documents (PRDs):** Produced by the PM agent, containing epics and stories.
- **UX/UI Specifications & Architecture Documents:** Created by Design Architect and Architect agents.
- The **POSM agent** is crucial for organizing and managing these documents.
- **Templates:** Standardized formats for briefs, PRDs, checklists, etc., likely stored in `bmad-agent/templates/`.
- **Data Directory (`bmad-agent/data/`):** Stores persistent data, knowledge bases (like this one), and other key information for the agents.

## BMAD METHOD - COMMUNITY AND CONTRIBUTIONS

The BMAD Method thrives on community involvement and collaborative improvement.

- **Getting Involved:**
  - **GitHub Discussions:** The primary platform for discussing potential ideas, use cases, additions, and enhancements to the method.
  - **Reporting Bugs:** If you find a bug, check existing issues first. If unreported, provide detailed steps to reproduce, along with any relevant logs or screenshots.
  - **Suggesting Features:** Check existing issues and discussions. Explain your feature idea in detail and its potential value.
- **Contribution Process (Pull Requests):**
  1. Fork the repository.
  2. Create a new branch for your feature or bugfix (e.g., `feature/your-feature-name`).
  3. Make your changes, adhering to existing code style and conventions. Write clear comments for complex logic.
  4. Run any tests or linting to ensure quality.
  5. Commit your changes with clear, descriptive messages (refer to the project's commit message convention, often found in `docs/commit.md`).
  6. Push your branch to your fork.
  7. Open a Pull Request against the main branch of the original repository.
- **Code of Conduct:** All participants are expected to abide by the project's Code of Conduct.
- **Licensing of Contributions:** By contributing, you agree that your contributions will be licensed under the same license as the project (MIT License).

### Licensing

The BMAD Method and its associated documentation and software are distributed under the **MIT License**.

Copyright (c) 2025 Brian AKA BMad AKA Bmad Code

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## BMAD METHOD - ETHOS & BEST PRACTICES

- **CORE_ETHOS:** You are the "Vibe CEO." Think like a CEO with unlimited resources and a singular vision. Your AI agents are your high-powered team. Your job is to direct, refine, and ensure quality towards your ambitious goal. The method elevates "vibe coding" to advanced project planning.
- **MAXIMIZE_AI_LEVERAGE:** Push the AI. Ask for more. Challenge its outputs. Iterate.
- **QUALITY_CONTROL:** You are the ultimate arbiter of quality. Review all outputs.
- **STRATEGIC_OVERSIGHT:** Maintain the high-level vision. Ensure agent outputs align.
- **ITERATIVE_REFINEMENT:** Expect to revisit steps. This is not a linear process.
- **CLEAR_INSTRUCTIONS:** The more precise your requests, the better the AI's output.
- **DOCUMENTATION_IS_KEY:** Good inputs (briefs, PRDs) lead to good outputs. The POSM agent is crucial for organizing this.
- **KNOW_YOUR_AGENTS:** Understand each agent's role (see [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities) or below). This includes understanding the capabilities of the Orchestrator agent if you are using one.
- **START_SMALL_SCALE_FAST:** Test concepts, then expand.
- **EMBRACE_THE_CHAOS:** Pioneering new methods is messy. Adapt and overcome.
- **ADAPT & EXPERIMENT:** The BMAD Method provides a structure, but feel free to adapt its principles, agent order, or templates to fit your specific project needs and working style. Experiment to find what works best for you. **Define agile the BMad way - or your way!** The agent configurations allow for customization of roles and responsibilities.

## AGENT ROLES AND RESPONSIBILITIES

Understanding the distinct roles and responsibilities of each agent is key to effectively navigating the BMAD workflow. While the "Vibe CEO" provides overall direction, each agent specializes in different aspects of the project lifecycle. V3 introduces Orchestrator agents that can embody these roles, with configurations specified in `web-bmad-orchestrator-agent.cfg.md` for web and `ide-bmad-orchestrator.cfg.md` for IDE environments.

- **Orchestrator Agent (BMAD):**

  - **Function:** The primary orchestrator, initially "BMAD." It can embody various specialized agent personas. It handles general BMAD queries, provides oversight, and is the go-to when unsure which specialist is needed.
  - **Persona Reference:** `personas#bmad` (Web) or implicitly the core of `ide-bmad-orchestrator.md` (IDE).
  - **Key Data/Knowledge:** Accesses `data#bmad-kb-data` (Web) for its knowledge base.
  - **Types:**
    - **Web Orchestrator:** Built using a script, leverages large context windows of platforms like Gemini 2.5 or OpenAI GPTs. Uses bundled assets. Its behavior and available agents are defined in `web-bmad-orchestrator-agent.cfg.md`.
    - **IDE Orchestrator:** Operates directly in IDEs like Cursor or Windsurf without a build step, loading persona and task files dynamically based on its configuration (`ide-bmad-orchestrator.cfg.md`). The orchestrator itself is defined in `ide-bmad-orchestrator.md`.
  - **Key Feature:** Simplifies agent management, especially in environments with limitations on the number of custom agents.

- **Analyst:**

  - **Function:** Handles research, requirements gathering, brainstorming, and the creation of Project Briefs.
  - **Web Persona:** `Analyst (Mary)` with persona `personas#analyst`. Customized to be "a bit of a know-it-all, and likes to verbalize and emote." Uses `templates#project-brief-tmpl`.
  - **IDE Persona:** `Analyst (Larry)` with persona `analyst.md`. Similar "know-it-all" customization. Tasks for Brainstorming, Deep Research Prompt Generation, and Project Brief creation are often defined within the `analyst.md` persona itself ("In Analyst Memory Already").
  - **Output:** `Project Brief`.

- **Product Manager (PM):**

  - **Function:** Responsible for creating and maintaining Product Requirements Documents (PRDs), overall project planning, and ideation related to the product.
  - **Web Persona:** `Product Manager (John)` with persona `personas#pm`. Utilizes `checklists#pm-checklist` and `checklists#change-checklist`. Employs `templates#prd-tmpl`. Key tasks include `tasks#create-prd`, `tasks#correct-course`, and `tasks#create-deep-research-prompt`.
  - **IDE Persona:** `Product Manager (PM) (Jack)` with persona `pm.md`. Focused on producing/maintaining the PRD (`create-prd.md` task) and product ideation/planning.
  - **Output:** `Product Requirements Document (PRD)`.

- **Architect:**

  - **Function:** Designs system architecture, handles technical design, and ensures technical feasibility.
  - **Web Persona:** `Architect (Fred)` with persona `personas#architect`. Uses `checklists#architect-checklist` and `templates#architecture-tmpl`. Tasks include `tasks#create-architecture` and `tasks#create-deep-research-prompt`.
  - **IDE Persona:** `Architect (Mo)` with persona `architect.md`. Customized to be "Cold, Calculating, Brains behind the agent crew." Generates architecture (`create-architecture.md` task), helps plan stories (`create-next-story-task.md`), and can update PO-level epics/stories (`doc-sharding-task.md`).
  - **Output:** `Architecture Document`.

- **Design Architect:**

  - **Function:** Focuses on UI/UX specifications, front-end technical architecture, and can generate prompts for AI UI generation services.
  - **Web Persona:** `Design Architect (Jane)` with persona `personas#design-architect`. Uses `checklists#frontend-architecture-checklist`, `templates#front-end-architecture-tmpl` (for FE architecture), and `templates#front-end-spec-tmpl` (for UX/UI Spec). Tasks: `tasks#create-frontend-architecture`, `tasks#create-ai-frontend-prompt`, `tasks#create-uxui-spec`.
  - **IDE Persona:** `Design Architect (Millie)` with persona `design-architect.md`. Customized to be "Fun and carefree, but a frontend design master." Helps design web apps, produces UI generation prompts (`create-ai-frontend-prompt.md` task), plans FE architecture (`create-frontend-architecture.md` task), and creates UX/UI specs (`create-uxui-spec.md` task).
  - **Output:** `UX/UI Specification`, `Front-end Architecture Plan`, AI UI generation prompts.

- **Product Owner (PO):**

  - **Function:** Agile Product Owner responsible for validating documents, ensuring development sequencing, managing the product backlog, running master checklists, handling mid-sprint re-planning, and drafting user stories.
  - **Web Persona:** `PO (Sarah)` with persona `personas#po`. Uses `checklists#po-master-checklist`, `checklists#story-draft-checklist`, `checklists#change-checklist`, and `templates#story-tmpl`. Tasks include `tasks#story-draft-task`, `tasks#doc-sharding-task` (extracts epics and shards architecture), and `tasks#correct-course`.
  - **IDE Persona:** `Product Owner AKA PO (Curly)` with persona `po.md`. Described as a "Jack of many trades." Tasks include `create-prd.md`, `create-next-story-task.md`, `doc-sharding-task.md`, and `correct-course.md`.
  - **Output:** User Stories, managed PRD/Backlog.

- **Scrum Master (SM):**

  - **Function:** A technical role focused on helping the team run the Scrum process, facilitating development, and often involved in story generation and refinement.
  - **Web Persona:** `SM (Bob)` with persona `personas#sm`. Described as "A very Technical Scrum Master." Uses `checklists#change-checklist`, `checklists#story-dod-checklist`, `checklists#story-draft-checklist`, and `templates#story-tmpl`. Tasks: `tasks#checklist-run-task`, `tasks#correct-course`, `tasks#story-draft-task`.
  - **IDE Persona:** `Scrum Master: SM (SallySM)` with persona `sm.ide.md`. Described as "Super Technical and Detail Oriented," specialized in "Next Story Generation" (likely leveraging the `sm.ide.md` persona's capabilities).

- **Developer Agents (DEV):**
  - **Function:** Implement user stories one at a time. Can be generic or specialized.
  - **Web Persona:** `DEV (Dana)` with persona `personas#dev`. Described as "A very Technical Senior Software Developer."
  - **IDE Personas:** Multiple configurations can exist, using the `dev.ide.md` persona file (optimized for <6K characters for IDEs). Examples:
    - `Frontend Dev (DevFE)`: Specialized in NextJS, React, Typescript, HTML, Tailwind.
    - `Dev (Dev)`: Master Generalist Expert Senior Full Stack Developer.
  - **Configuration:** Specialized agents can be configured in `ide-bmad-orchestrator.cfg.md` for the IDE Orchestrator, or defined for the Web Orchestrator. Standalone IDE developer agents (e.g., `dev.ide.md`) are also available.
  - **When to Use:** During the implementation phase, typically working within an IDE.

## NAVIGATING THE BMAD WORKFLOW - INITIAL GUIDANCE

### STARTING YOUR PROJECT - ANALYST OR PM?

- Use Analyst if unsure about idea/market/feasibility or need deep exploration.
- Use PM if concept is clear or you have a Project Brief.
- Refer to [AGENT ROLES AND RESPONSIBILITIES](#agent-roles-and-responsibilities) (or section within this KB) for full details on Analyst and PM.

### UNDERSTANDING EPICS - SINGLE OR MULTIPLE?

- Epics represent significant, deployable increments of value.
- Multiple Epics are common for non-trivial projects or a new MVP (distinct functional areas, user journeys, phased rollout).
- Single Epic might suit very small MVPs, or post MVP / brownfield new features.
- The PM helps define and structure epics.

## GETTING STARTED WITH BMAD

This section provides guidance for new users on how to set up their project with the BMAD agent structure and manage artifacts.

### Initial Project Setup

To begin using the BMAD method and its associated agents in your project, you need to integrate the core agent files:

- **Copy `bmad-agent` Folder:** The entire `bmad-agent` folder should be copied into the root directory of your project. This folder contains all the necessary personas, tasks, templates, and configuration files for the BMAD agents to function correctly.

### Exporting Artifacts from AI Platforms

Once an AI agent (like those in Gemini or ChatGPT) has generated a document (e.g., Project Brief, PRD, Architecture Document), you'll need to save it into your project:

- **Gemini:**
  - After the document is produced, click the `...` (more options) menu typically found near the response.
  - Select "Copy". The content will be copied as Markdown.
  - Paste this content into a new `.md` file within your project's `docs` folder (or a similar designated location).
  - **Passing to a new chat instance:** Gemini's chat interface may not directly support pasting Markdown with full fidelity in all scenarios.
    - You can paste the raw Markdown content directly.
    - Alternatively, save the content as a `.txt` file and paste from there.
    - For sharing or preserving formatting in Google Docs: Create a new Google Doc, right-click, and select "Paste without formatting" if pasting directly, or look for options to import/paste Markdown. Some browser extensions can facilitate Markdown rendering in Google Docs.
- **ChatGPT:**
  - ChatGPT generally handles Markdown well. You can copy the generated Markdown output directly.
  - Paste it into a `.md` file in your project's `docs` folder.
  - Sharing `.md` files or their content with new ChatGPT instances (e.g., by uploading the file or pasting the text) is typically straightforward.

### Document Sharding

Large documents like PRDs or Architecture Documents can become unwieldy for AI agents to process efficiently, especially in environments with context window limitations. The `doc-sharding-task.md` is designed to break these down:

- **Purpose:** The sharding task splits a large document (e.g., PRD, Architecture, Front-End Architecture) into smaller, more granular sections or individual user stories. This makes it easier for subsequent agents, like the SM (Scrum Master) or Dev Agents, to work with specific parts of the document without needing to process the entire thing.
- **How to Use:**
  1.  Ensure the large document you want to shard (e.g., `prd.md`, `architecture.md`) exists in your project's `docs` folder.
  2.  Instruct your active IDE agent (e.g., PO, SM, or the BMAD Orchestrator embodying one of these roles) to run the `doc-sharding-task.md`.
  3.  You will typically specify the _source file_ to be sharded. For example: "Run the `doc-sharding-task.md` against `docs/prd.md`."
  4.  The task will guide the agent to break down the document. The output might be new smaller files or instructions on how the document is logically segmented.

### Utilizing Dedicated IDE Agents (SM and Dev)

While the BMAD IDE Orchestrator can embody any persona, for common and intensive tasks like story generation (SM) and code implementation (Dev), it's highly recommended to use dedicated, specialized agents:

- **Why Dedicated Agents?**
  - **Context Efficiency:** Dedicated agents (e.g., `sm.ide.md`, `dev.ide.md`) are leaner as their persona files are smaller and more focused. This is crucial in IDEs where context window limits can impact performance and output quality.
  - **Performance:** Less overhead means faster responses and more focused interactions.
- **Recommendation:**
  - Favor using `sm.ide.md` for Scrum Master tasks (like generating the next story).
  - Favor using `dev.ide.md` (or specialized versions like `dev-frontend.ide.md`) for development tasks.
- **Creating Your Own Dedicated Agents:**
  - If your IDE supports more than a few custom agent modes (unlike Cursor's typical limit of 5 without paying for more), you can easily create your own specialized agents.
  - Take the content of a base persona file (e.g., `bmad-agent/personas/architect.md`).
  - Optionally, integrate the content of frequently used task files directly into this new persona file.
  - Save this combined content as a new agent mode in your IDE (e.g., `my-architect.ide.md`). This approach mirrors how the `sm.ide.md` agent is structured.

### When to Use the BMAD IDE Orchestrator

The BMAD IDE Orchestrator (`ide-bmad-orchestrator.md` configured by `ide-bmad-orchestrator.cfg.md`) provides flexibility but might not always be the most efficient choice.

- **Useful Scenarios:**
  - **Cursor IDE with Agent Limits:** If you're using an IDE like Cursor and frequently need to switch between many different agent personalities (Analyst, PM, Architect, etc.) beyond the typical free limit for custom modes, the Orchestrator allows you to access all configured personas through a single agent slot.
  - **Unified Experience (Gemini/ChatGPT Parity):** If you prefer to interact with the BMAD agent system in your IDE in the same way you would in a web UI like Gemini (using the BMAD Orchestrator to call upon different specialists), and you are not concerned about context limits or potential costs associated with larger LLM models that can handle the Orchestrator's broader context.
  - **Access to all Personas:** You want quick access to any of the defined agent personas without setting them up as individual IDE modes.
- **Potentially Unnecessary / Less Optimal Scenarios:**
  - **Simple Projects / Feature Additions (Caution Advised):** For very simple projects or when adding a small feature to an existing codebase, you _might_ consider a streamlined flow using the Orchestrator to embody the PM, generate a PRD with epics/stories, and then directly move to development, potentially skipping detailed architecture.
    - In such cases, the PM persona might be prompted to ask more technical questions to ensure generated stories are sufficiently detailed for developers.
    - **This is generally NOT recommended** as it deviates from the robust BMAD process and is not yet a fully streamlined or validated path. It risks insufficient planning and lower quality outputs.
  - **Frequent SM/Dev Tasks:** As mentioned above, for regular story creation and development, dedicated SM and Dev agents are more efficient due to smaller context overhead.

Always consider the trade-offs between the Orchestrator's versatility and the efficiency of dedicated agents, especially concerning your IDE's capabilities and the complexity of your project.

## SUGGESTED ORDER OF AGENT ENGAGEMENT (TYPICAL FLOW)

**NOTE:** This is a general guideline. The BMAD method is iterative; phases/agents might be revisited.

1. **Analyst** - brainstorm and create a project brief.
2. **PM (Product Manager)** - use the brief to produce a PRD with high level epics and stories.
3. **Design Architect UX UI Spec for PRD (If project has a UI)** - create the front end UX/UI Specification.
4. **Architect** - create the architecture and ensure we can meet the prd requirements technically - with enough specification that the dev agents will work consistently.
5. **Design Architect (If project has a UI)** - create the front end architecture and ensure we can meet the prd requirements technically - with enough specification that the dev agents will work consistently.
6. **Design Architect (If project has a UI)** - Optionally create a prompt to generate a UI from AI services such as Lovable or V0 from Vercel.
7. **PO**: Validate documents are aligned, sequencing makes sense, runs a final master checklist. The PO can also help midstream development replan or course correct if major changes occur.
8. **PO or SM**: Generate Stories 1 at a time (or multiple but not recommended) - this is generally done in the IDE after each story is completed by the Developer Agents.
9. **Developer Agents**: Implement Stories 1 at a time. You can craft different specialized Developer Agents, or use a generic developer agent. It is recommended to create specialized developer agents and configure them in the `ide-bmad-orchestrator.cfg`.

## HANDLING MAJOR CHANGES

Major changes are an inherent part of ambitious projects. The BMAD Method embraces this through its iterative nature and specific agent roles:

- **Iterative by Design:** The entire BMAD workflow is built on "ITERATIVE_REFINEMENT." Expect to revisit previous steps and agents as new information emerges or requirements evolve. It's "not a linear process."
- **Embrace and Adapt:** The core ethos includes "EMBRACE_THE_CHAOS" and "ADAPT & EXPERIMENT." Major changes are opportunities to refine the vision and approach.
- **PO's Role in Re-planning:** The **Product Owner (PO)** is key in managing the impact of significant changes. They can "help midstream development replan or course correct if major changes occur." This involves reassessing priorities, adjusting the backlog, and ensuring alignment with the overall project goals.
- **Strategic Oversight by Vibe CEO:** As the "Vibe CEO," your role is to maintain "STRATEGIC_OVERSIGHT." When major changes arise, you guide the necessary pivots, ensuring the project remains aligned with your singular vision.
- **Re-engage Agents as Needed:** Don't hesitate to re-engage earlier-phase agents (e.g., Analyst for re-evaluating market fit, PM for revising PRDs, Architect for assessing technical impact) if a change significantly alters the project's scope or foundations.

## IDE VS UI USAGE - GENERAL RECOMMENDATIONS

The BMAD method can be orchestrated through different interfaces, typically a web UI for higher-level planning and an IDE for development and detailed developer story generation. The most general recommendation is to do all document generation from the brief, PRD, Architecture, Design Architecture, and potentially UI Prompts. Also use the PO to run the full final checklist to ensure all documents are aligned with various changes. For example, did the architect discover something that requires an update to a epic or story sequence in the PRD? The PO will help you there. Once done, then export the documents to the IDE. If documents have been modified, you can ask the specific proper agents in Gemini or chatGPT to give you the final unredacted complete document. Save these into the docs folder of your project.

### CONCEPTUAL, PLANNING PHASES and TECHNICAL DESIGN

- **Interface:** Often best managed via a Web UI (leveraging the **Web Agent Orchestrator** with its bundled assets and `agent-prompt.txt`) or dedicated project management tools where orchestrator agents can guide the process.
- **Agents Involved:**
  - **Analyst:** Brainstorming, research, and initial project brief creation.
  - **PM (Product Manager):** PRD development, epic and high-level story definition.
  - **Architect / Design Architect (UI):** Detailed technical design and specification.
  - **PO:** Checklist runner to make sure all of the documents are aligned.
- **Activities:** Defining the vision, initial requirements gathering, market analysis, high-level planning. The `web-bmad-orchestrator-agent.md` and its configuration likely support these activities.

### DOCUMENTATION MANAGEMENT & IMPLEMENTATION PHASES

- **Interface:** Primarily within the Integrated Development Environment (IDE), leveraging specialized agents (standalone or via the **IDE Agent Orchestrator** configured with `ide-bmad-orchestrator.cfg.md`).
- **Agents Involved:**
  - "**PO or SM or BMad Agent:** Run the doc sharing task to split the large files that have been created (PRD, Architecture etc...) into smaller granular documents that are easier for the SM and Dev Agents to work with.
  - **SM (Scrum Master):** Detailed story generation, backlog refinement, often directly in the IDE or tools integrated with it.
  - **Developer Agents:** Code implementation for stories, working directly with the codebase in the IDE.
- **Activities:** Detailed architecture, front-end/back-end design, code development, testing, leveraging IDE tasks (see "LEVERAGING IDE TASKS FOR EFFICIENCY"), using configurations like `ide-bmad-orchestrator.cfg.md`.

### BMAD METHOD FILES

Understanding key files helps in navigating and customizing the BMAD process:

- **Knowledge & Configuration:**
  - `bmad-agent/data/bmad-kb.md`: This central knowledge base.
  - `ide-bmad-orchestrator.cfg.md`: Configuration for IDE developer agents.
  - `ide-bmad-orchestrator.md`: Definition of the IDE orchestrator agent.
  - `web-bmad-orchestrator-agent.cfg.md`: Configuration for the web orchestrator agent.
  - `web-bmad-orchestrator-agent.md`: Definition of the web orchestrator agent.
- **Task Definitions:**
  - Files in `bmad-agent/tasks/` or `bmad-agent/checklists/` (e.g., `checklist-run-task.md`): Reusable prompts for specific actions and also used by agents to keep agent persona files lean.
- **Agent Personas & Templates:**
  - Files in `bmad-agent/personas/`: Define the core behaviors of different agents.
  - Files in `bmad-agent/templates/`: Standard formats for documents like Project Briefs, PRDs that the agents will use to populate instances of these documents.
- **Project Artifacts (Outputs - locations vary based on project setup):**
  - Project Briefs
  - Product Requirements Documents (PRDs)
  - UX/UI Specifications
  - Architecture Documents
  - Codebase and related development files.

## LEVERAGING IDE TASKS FOR EFFICIENCY

### PURPOSE OF IDE TASKS

- **Reduce Agent Bloat:** Avoid adding numerous, rarely used instructions to primary IDE agent modes (Dev Agent, SM Agent) or even the Orchestrator's base prompt. Keeps agents lean, beneficial for IDEs with limits on custom agent complexity/numbers.
- **On-Demand Functionality:** Instruct an active IDE agent (standalone or an embodied persona within the IDE Orchestrator) to perform a task by providing the content of the relevant task file (e.g., from `bmad-agent/tasks/checklist-run-task.md`) as a prompt, or by referencing it if the agent is configured to find it (as with the IDE Orchestrator).
- **Versatility:** Any sufficiently capable agent can be asked to execute a task. Tasks can handle specific functions like running checklists, creating stories, sharding documents, indexing libraries, etc. They are self-contained instruction sets.

### EXAMPLES OF TASK FUNCTIONALITY

**CONCEPT:** Think of tasks as specialized, callable mini-agents or on-demand instruction sets that main IDE agents or the Orchestrator (when embodying a persona) can invoke, keeping primary agent definitions streamlined. They are particularly useful for operations not performed frequently. The `docs/instruction.md` file provides more details on task setup and usage.

Here are some examples of functionalities provided by tasks found in `bmad-agent/tasks/`:

- **`create-prd.md`:** Guides the generation of a Product Requirements Document.
- **`create-next-story-task.md`:** Helps in defining and creating the next user story for development.
- **`create-architecture.md`:** Assists in outlining the technical architecture for a project.
- **`create-frontend-architecture.md`:** Focuses specifically on designing the front-end architecture.
- **`create-uxui-spec.md`:** Facilitates the creation of a UX/UI Specification document.
- **`create-ai-frontend-prompt.md`:** Helps in drafting a prompt for an AI service to generate UI/frontend elements.
- **`doc-sharding-task.md`:** Provides a process for breaking down large documents into smaller, manageable parts.
- **`library-indexing-task.md`:** Assists in creating an index or overview of a code library.
- **`checklist-run-task.md`:** Executes a predefined checklist (likely using `checklist-mappings.yml`).
- **`correct-course.md`:** Provides guidance or steps for when a project needs to adjust its direction.
- **`create-deep-research-prompt.md`:** Helps formulate prompts for conducting in-depth research on a topic.

These tasks allow agents to perform complex, multi-step operations by following the detailed instructions within each task file, often leveraging templates and checklists as needed.
