# Content Systems Architecture: The Engineering of Information

### 🏗️ Repository Overview
**Role:** Principal Systems Architect  
**Status:** Production / Legacy (2023-Present)  
**Focus:** Agentic Workflows, Deterministic GenAI, and Automated Supply Chains.

This repository documents the **"Content Engineering"** frameworks developed to operationalize Large Language Models (LLMs) for commercial scalability. Unlike standard "prompt engineering," which focuses on singular outputs, these architectures utilize **XML-based logic gates**, **stateful execution**, and **human-in-the-loop (HIL) protocols** to treat natural language as executable code.

---

## 📂 1. Agentic Editorial Engine (`/agentic-editorial-engine`)

**The Problem:** Commercial digital product creation (ebooks, whitepapers) is historically bottlenecked by manual drafting, formatting consistency, and "hallucination" risks in long-form generation.

**The Architecture:**
A **"Prompt-as-Code" pipeline** that encapsulates persona, tone, and strict DOM (Document Object Model) constraints within a single execution environment.

* **XML Encapsulation:** Utilizes `<TaskDefinition>` and `<ContextAndData>` tags to create pseudo-namespaces, preventing logic bleed between creative and structural instructions.
* **Stateful Iteration:** Implements a "Wait for Next" protocol, forcing the model to hold state (Outline → Draft → Review) in memory before committing to the next phase.
* **Schema Enforcement:** Compels the model to output raw HTML (`h1`, `div`, `li`) rather than markdown, allowing for direct compilation into production-ready formats (`.docx`, `.epub`).

**Commercial Artifact:**
* **Product:** *The ABCs of Raising a Puppy* (Commercial Lead Magnet)
* **Performance:** 100% Sell-Through Rate; Reduced Time-to-Market by 95% (Weeks → Hours).

---

## 📂 2. Deterministic SEO Agents (`/deterministic-seo-agents`)

**The Problem:** High-volume content generation often suffers from "drift," losing brand voice or SEO intent over time. Standard chatbots lack the rigor for enterprise compliance.

**The Architecture:**
A **Human-in-the-Loop (HIL) Orchestrator** designed for the **NewsFLASH** and **SocialBLITZ** commercial SaaS products.

* **Chain-of-Thought (CoT) Injection:** Embedded reasoning steps within the system prompt force the agent to validate keyword density and tone *before* generating text.
* **Logic Gates:** Implements strict `<CLARITY>` and `[WAIT FOR USER APPROVAL]` checkpoints. The system pauses execution at critical failure points (Analysis, Outlining, Drafting) to ensure off-nominal behavior is caught immediately.
* **Context Injection:** dynamically references static knowledge bases (`.txt` rule sets, Hemingway Rules) to ground probabilistic outputs in deterministic best practices.

**Commercial Artifact:**
* **Product:** NewsFLASH & SocialBLITZ (SaaS Subscriptions)
* **Scale:** Deployed to 400+ active users; consistently maintained >4.8/5.0 satisfaction ratings over 12 months.

---

## 📂 3. Automated Media Rendering Pipeline (`/media-supply-chain`)

**The Problem:** Video content scaling is limited by manual rendering time. "Guru" solutions rely on expensive software, ignoring low-code integration possibilities.

**The Architecture:**
A **Self-Correcting ETL (Extract, Transform, Load) Pipeline** that bridges the gap between text generation and visual rendering engines.

* **Quality Assurance (QA) Loops:** The generative prompt includes a recursive `<REVIEW>` tag, forcing the LLM to critique and score its own output (1-10 scale) against specific criteria. Data is only serialized if it meets a "9/10" threshold.
* **CSV Middleware:** outputs structured data compatible with **Canva's Bulk Create API**, automating the rendering of 100+ unique video assets in a single batch operation.
* **Zero-Cost Infrastructure:** Architected entirely on "Free Tier" tools (ChatGPT, Google Sheets, Canva), demonstrating enterprise-grade automation without enterprise-grade overhead.

**Commercial Artifact:**
* **Metric:** Production rate increased to **100 videos/hour** (vs. 1 video/hour manual).
* **Impact:** Methodology published as an open-source guide, adopted by thousands of users for rapid social scaling.

---

### 🛠️ Technical Philosophy
This repository operates on the principle of **Deterministic AI**:
1.  **Context is Code:** Prompts are structured with the same rigor as software classes.
2.  **Trust but Verify:** Every automated step includes a validation gate (HIL or Self-Correction).
3.  **Ship the Machine:** The value isn't the content; it's the pipeline that produces it.

---

*This portfolio represents a transition from "using tools" to "architecting systems." For inquiries regarding specific implementations or consulting, please contact via LinkedIn.*
