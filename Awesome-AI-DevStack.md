# 🚀 Awesome AI DevStack

A curated, open-source collection of AI tools, large language model (LLM) libraries, and autonomous agents designed to accelerate software development, automate workflows, and enhance applications.

---

## 📋 Table of Contents
- [LLMs & Fine-Tuning](#llms--fine-tuning)
- [Autonomous Agents & Orchestration](#autonomous-agents--orchestration)
- [Development Tools & CLI](#development-tools--cli)
- [Data Processing & RAG](#data-processing--rag)
- [Sensors & Hardware Integrations](#sensors--hardware-integrations)
- [Virtual Characters & Avatars](#virtual-characters--avatars)
- [Collections & Templates](#collections--templates)

---

## 🧠 LLMs & Fine-Tuning

### [Unsloth](https://github.com/unslothai/unsloth)
* **What it does:** A library and framework for fine-tuning large language models. It uses advanced math to speed up training by 2x to 5x while significantly reducing VRAM usage.
* **Applications & Examples:**
  * **Enterprise Expert Models:** Taking an open-source model (like Llama 3) and fine-tuning it on company procedures, historical logs, or user manuals to create a specialized local model.
  * **Edge Device Optimization:** Shrinking and training models to run efficiently on local servers or low-power hardware for real-time sensor analysis without losing accuracy.

---

## 🤖 Autonomous Agents & Orchestration

### [Open SWE](https://github.com/langchain-ai/open-swe)
* **What it does:** An open-source Software Engineering Agent built on LangChain. You provide a GitHub issue or bug description, and the agent autonomously reads the source code, writes a fix, and submits a Pull Request.
* **Applications & Examples:**
  * **Automated UI Maintenance:** Assigning the agent to fix minor frontend bugs (e.g., misaligned React components) while developers focus on core business logic.
  * **Automated Testing:** Dispatching the agent to write unit tests for existing backend Python scripts.

### [Superset](https://github.com/superset-sh/superset)
* **What it does:** An IDE and central orchestrator designed specifically for the AI agent era. It allows you to run an "army" of AI coding agents (like Claude Code, Codex, Cursor Agent) simultaneously on your local machine.
* **Applications & Examples:**
  * **Parallel Development:** Managing multiple coding agents through a single interface, isolating their worktrees so they do not overwrite each other's code during complex development cycles.

### [memU](https://github.com/NevaMind-AI/memU)
* **What it does:** A long-term memory system designed for 24/7 proactive AI agents. It acts as a memory file system that absorbs long conversations, identifies intents, extracts facts, and categorizes data automatically.
* **Applications & Examples:**
  * **Contextual Persistence:** Allowing conversational agents to maintain long-term user context over months of interaction without sending massive chat histories back to the LLM, significantly reducing token costs.

---

## 🛠️ Development Tools & CLI

### [Get Shit Done (GSD)](https://github.com/gsd-build/get-shit-done)
* **What it does:** An AI-powered CLI tool aimed at simplifying and accelerating backend development tasks. It uses simple prompts to scaffold entire projects, run scripts, and wire up developer tools automatically.
* **Applications & Examples:**
  * **Rapid Microservice Scaffolding:** Generating folder structures, configuration files, and database connections for new Python microservices in seconds.
  * **Deployment Automation:** Building automated scripts that package and deploy application updates to a server with a single command.

---

## 📊 Data Processing & RAG

### [OpenDataLoader PDF](https://github.com/opendataloader-project/opendataloader-pdf)
* **What it does:** A powerful tool for extracting structured data (text, tables, images) from complex PDF files, specifically optimized for feeding data into RAG (Retrieval-Augmented Generation) pipelines and LLMs.
* **Applications & Examples:**
  * **Financial Automation:** Reading scanned invoices or complex PDF reports, accurately extracting table data so an AI agent can analyze monthly expenses.
  * **Contract Digitization:** Parsing scanned documents and seamlessly feeding the structured text into a CRM database.

---

## 📡 Sensors & Hardware Integrations

### [WiFi DensePose](https://github.com/ruvnet/wifi-densepose)
* **What it does:** A system that turns commodity WiFi signals into real-time human pose estimation, without requiring a single pixel of video.
* **Applications & Examples:**
  * **Privacy-Preserving Monitoring:** Enabling presence detection, fall detection, and vital sign monitoring through walls, making it ideal for smart home environments where privacy is a priority.

---

## 🎭 Virtual Characters & Avatars

### [Airi](https://github.com/moeru-ai/airi)
* **What it does:** A self-hosted, open-source platform for running AI-driven virtual characters (VTubers or digital companions). 
* **Applications & Examples:**
  * **Autonomous Virtual Agents:** Creating virtual characters capable of real-time voice chat, expressing emotions via 3D models, and autonomously playing environments like Minecraft or Factorio.

---

## 📚 Collections & Templates

### [Awesome LLM Apps](https://github.com/Shubhamsaboo/awesome-llm-apps)
* **What it does:** A rich collection of ready-made apps, templates, and code for building LLM applications with AI Agents and RAG architectures (supporting OpenAI, Anthropic, Gemini, and open-source models).
* **Applications & Examples:**
  * **Rapid Prototyping:** Serving as a toolbox for developers to quickly integrate voice capabilities, enterprise data search, or agentic workflows into new projects.

---
*Built and maintained as an open-source knowledge base for the developer community.*