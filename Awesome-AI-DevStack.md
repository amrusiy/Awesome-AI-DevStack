# 🚀 Awesome AI DevStack

Welcome to **Awesome AI DevStack**! 👋

This is a curated, open-source collection of AI tools, large language model (LLM) libraries, autonomous agents, and developer utilities.

Whether you are building complex backend microservices, maintaining web frontends, or optimizing models to run locally, this repository is designed to help you find the right tools to accelerate your development, automate workflows, and enhance your applications.

---

## 🌟 How to Use This Guide

1. **Browse by Category:** Use the Table of Contents below to jump straight to the type of tool you need.
2. **Read the Examples:** Every tool includes practical, real-world applications so you can instantly see if it fits your current project.
3. **Feed it to your AI:** You can easily point your own AI agents (like Claude or ChatGPT) to the raw version of this file so they can search for tools on your behalf. Just use this link: `[INSERT_RAW_GITHUB_LINK_HERE]`

---

## 📋 Table of Contents

- [🧠 AI Models, Fine-Tuning & Infrastructure](#-ai-models-fine-tuning--infrastructure)
- [🤖 Autonomous Agents & Orchestration](#-autonomous-agents--orchestration)
- [🧠 Agent Memory Systems](#-agent-memory-systems)
- [🛠️ Development Tools, Infrastructure & CLI](#-development-tools-infrastructure--cli)
- [📊 Data Processing, RAG & Visualization](#-data-processing-rag--visualization)
- [🎨 UI Frameworks & Frontend](#-ui-frameworks--frontend)
- [🔐 Security, OSINT & Penetration Testing](#-security-osint--penetration-testing)
- [🎬 Media, 3D & Audio Generation](#-media-3d--audio-generation)
- [🌐 APIs, Networking & Web Scraping](#-apis-networking--web-scraping)
- [💼 Business, Finance & Operations](#-business-finance--operations)
- [📡 Sensors & Hardware Integrations](#-sensors--hardware-integrations)
- [🎭 Virtual Characters & Avatars](#-virtual-characters--avatars)
- [📚 Learning, Collections & Templates](#-learning-collections--templates)

---

## 🧠 AI Models, Fine-Tuning & Infrastructure

### [LiteLLM](https://github.com/BerriAI/litellm)

- **What it does:** An API Gateway that allows you to call over 100 different LLMs (Claude, Gemini, Llama) using the standard OpenAI API format. It handles load balancing, fallbacks, authentication, and cost tracking.
- **Use Cases:** Setting up real-time model fallbacks (e.g., routing to Anthropic if OpenAI fails) without changing application code; enforcing team budget controls and rate limits for internal developers.

### [TimesFM](https://github.com/google-research/timesfm)

- **What it does:** A pre-trained foundation model by Google Research specifically designed for time-series forecasting. Unlike LLMs, it analyzes historical numerical trends to predict future values with high accuracy (Zero-shot).
- **Use Cases:** Forecasting server traffic and load spikes to trigger proactive auto-scaling; analyzing historical e-commerce sales trends to predict future product demand.

### [Unsloth](https://github.com/unslothai/unsloth)

- **What it does:** A library for fine-tuning large language models. It uses advanced math to speed up training by 2x to 5x while significantly reducing VRAM usage.
- **Use Cases:** Fine-tuning open-source models on enterprise data; optimizing models to run efficiently on edge devices or low-power hardware.

### [BitNet](https://github.com/microsoft/BitNet)

- **What it does:** A framework by Microsoft for training and running 1-bit LLMs. It drastically reduces compute and memory requirements.
- **Use Cases:** Running highly capable language models entirely on standard CPUs without the need for expensive GPUs.

### [LMCache](https://github.com/LMCache/LMCache)

- **What it does:** A caching layer for LLM execution engines (like vLLM) that saves internal KV cache computations to RAM or disk.
- **Use Cases:** Enabling near-instant responses for RAG systems reading massive codebases or huge PDF files; reducing token computation costs.

### [vLLM-Omni](https://github.com/vllm-project/vllm-omni)

- **What it does:** An extension for the popular vLLM engine that adds highly efficient, official support for multimodal models (processing text and images together at high throughput).
- **Use Cases:** Setting up high-volume internal APIs for automated visual analysis; deploying technical support chatbots capable of analyzing user screenshots.

### [RuView](https://github.com/ruvnet/RuView)

- **What it does:** A visualization and analysis tool for LLM inference data. It lets developers inspect model token probabilities and thought processes in real-time.
- **Use Cases:** Debugging complex prompts; identifying model hallucinations by monitoring token confidence levels.

### [MiniMind](https://github.com/jingyaogong/minimind)

- **What it does:** Provides the full source code to train a tiny LLM (~20M parameters) entirely from scratch.
- **Use Cases:** Hands-on AI education for understanding model architecture; deploying basic NLP capabilities to offline IoT microcontrollers.

---

## 🤖 Autonomous Agents & Orchestration

### [Block Goose](https://github.com/block/goose)

- **What it does:** An open-source, autonomous AI development agent created by Block. Unlike standard autocomplete extensions, Goose runs directly on your machine (via CLI or Desktop app). It can read/write files, execute system commands, identify and fix bugs, and verify results. It is LLM-agnostic and fully supports the Model Context Protocol (MCP) for seamless integration with external tools.
- **Use Cases:** \* **Terminal Debugging Automation:** Trigger the agent when a build crashes. It reads the error logs, resolves dependency conflicts, modifies the source code, and recompiles the project to verify the fix.
  - **Rapid Project Scaffolding:** Request a complete backend setup (e.g., a Node.js server with PostgreSQL and CRUD endpoints) via natural language, and the agent will generate the folder structure, logic, configs, and unit tests.
  - **MCP Workflow Integration:** Connect the agent to internal MCP servers so it can read product requirements directly from Jira tickets, translate them into code, and push the final commits to Git.

### [OpenAI Codex CLI](https://github.com/openai/codex)

- **What it does:** The official coding agent by OpenAI that runs directly in your local terminal. It can execute complex file reads, write code, run system commands, and debug using natural language.
- **Use Cases:** Automating project management by having the agent locate and fix compilation errors across multiple files simultaneously; rapidly scaffolding new projects (like Node.js) by verbally commanding the agent to install dependencies and write configurations.

### [Oh My Codex](https://github.com/Yeachan-Heo/oh-my-codex)

- **What it does:** An orchestration and workflow layer built on top of the official OpenAI Codex terminal agent. It adds persistent memory, predefined persona prompts (e.g., "Architect" or "Executor"), and automated skills.
- **Use Cases:** Establishing a "brain folder" so the agent remembers previous bugs, command history, and coding standards across sessions; orchestrating virtual automation teams by splitting large development tasks among multiple synchronized agent instances.

### [AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2)

- **What it does:** A groundbreaking framework enabling AI models to conduct fully autonomous scientific research. It generates hypotheses, writes code for experiments, analyzes results, and drafts full academic papers.
- **Use Cases:** Automated algorithm benchmarking and performance comparisons; conducting autonomous literature reviews to distill conclusions for product planning.

### [ChatDev](https://github.com/OpenBMB/ChatDev)

- **What it does:** A virtual software company simulation. It utilizes multiple AI agents playing different roles (CEO, PM, Dev, QA) who collaborate and converse to write and compile working software from a single prompt.
- **Use Cases:** Rapid prototyping to generate folder structures, basic logic, and documentation in minutes; experimenting with multi-agent communication architectures to reduce LLM hallucinations.

### [Oh My ClaudeCode](https://github.com/Yeachan-Heo/oh-my-claudecode)

- **What it does:** An orchestration system for running multiple Claude Code developer agents in parallel. It supports hierarchical team structures (e.g., a "Project Manager" agent dividing tasks between "Frontend" and "Backend" agents).
- **Use Cases:** Large-scale project development where agents work concurrently (e.g., building APIs while writing tests); massive legacy code refactoring without collision.

### [Open SWE](https://github.com/langchain-ai/open-swe)

- **What it does:** An open-source Software Engineering Agent that reads GitHub issues, scans source code, writes a fix, and submits Pull Requests autonomously.
- **Use Cases:** Automating routine UI maintenance; writing unit tests for existing backend code.

### [Superset](https://github.com/superset-sh/superset)

- **What it does:** An IDE and central orchestrator designed for running an "army" of AI coding agents simultaneously on a local machine with isolated worktrees.
- **Use Cases:** Managing parallel development tasks where multiple agents write code without overwriting each other's work.

### [AgentScope](https://github.com/agentscope-ai/agentscope)

- **What it does:** A multi-agent framework tailored for production environments. It includes a secure execution sandbox, a visual monitoring studio, and memory management.
- **Use Cases:** Safely executing AI-generated code on local systems; building enterprise AI microservices.

### [Agency Agents](https://github.com/msitarzewski/agency-agents)

- **What it does:** A repository featuring 51 specialized AI agent personas (e.g., "Frontend Dev", "Legal Reviewer"), each with precise configurations and workflows.
- **Use Cases:** Assigning specific, well-defined professional tasks to specialized agents rather than relying on generic LLM prompts.

### [deepagents](https://github.com/langchain-ai/deepagents)

- **What it does:** A LangChain framework for building "Deep Research" agents that can break down open-ended queries, browse the web, synthesize information, and write reports.
- **Use Cases:** Automating hardware comparison research; generating monthly competitive intelligence reports.

### [Browser Use](https://github.com/browser-use/browser-use)

- **What it does:** A library that gives AI models the ability to control a web browser like a human to click buttons, fill out forms, and handle complex SPA sites (React/Vue).
- **Use Cases:** Advanced web scraping behind authenticated business portals; creating personal shopping/booking agents.

### [OpenClaw](https://github.com/openclaw/openclaw)

- **What it does:** A fully open-source, locally hosted autonomous AI assistant designed to integrate with standard messaging apps.
- **Use Cases:** Creating a private messaging assistant to transcribe and log voice notes; running remote DevOps commands via secure chat.

### [AstrBot](https://github.com/AstrBotDevs/AstrBot)

- **What it does:** A lightweight LLM bot platform supporting various social and messaging apps via local deployment or Docker.
- **Use Cases:** Self-hosting a private digital assistant; piping automated system crash alerts directly to developer messaging channels.

### [Flowise](https://github.com/FlowiseAI/Flowise)

- **What it does:** An open-source drag-and-drop platform for visually designing LLM workflows and RAG pipelines.
- **Use Cases:** Rapidly prototyping AI applications and deploying them to web frontends without writing complex infrastructure code.

---

## 🧠 Agent Memory Systems

### [Supermemory](https://github.com/supermemoryai/supermemory)

- **What it does:** An open-source "Second Brain" for personal knowledge management. It saves articles, tweets, videos, and notes, with an integrated AI agent for natural language querying.
- **Use Cases:** Academic/technical research summarization; intelligent bookmarking that retrieves exact context.

### [memU](https://github.com/NevaMind-AI/memU)

- **What it does:** A long-term memory system for 24/7 proactive AI agents that categorizes conversations and extracts facts to maintain context over time.
- **Use Cases:** Reducing token costs for continuous conversational agents by intelligently managing chat history.

### [Cognee](https://github.com/topoteretes/cognee)

- **What it does:** A Knowledge Graph-based memory system that maps logical relationships between entities, allowing AI to understand complex data connections.
- **Use Cases:** Helping personal assistants identify recurring scheduling patterns; managing complex enterprise CRM data relationships.

### [Hindsight](https://github.com/vectorize-io/hindsight)

- **What it does:** An advanced memory system that learns from past interactions, deduces new insights, and actively shifts the agent's behavior over time based on user feedback.
- **Use Cases:** Building smart customer service bots that remember user preferences; personal assistants that adapt to specific workflow habits.

### [Claude-Mem](https://github.com/thedotmack/claude-mem)

- **What it does:** A tool utilizing the Model Context Protocol (MCP) to give Claude a persistent local memory file.
- **Use Cases:** Saving preferred tech stacks and coding styles; securely referencing local API keys without pasting them into every chat.

---

## 🛠️ Development Tools, Infrastructure & CLI

### [Fastfetch](https://github.com/fastfetch-cli/fastfetch)

- **What it does:** A CLI tool written in C that displays system information (hardware, OS, kernel, RAM) instantly with aesthetic ASCII art. It is the modern, highly performant successor to Neofetch.
- **Use Cases:** Configuring Linux servers to display a quick visual summary of system health upon SSH login; appending hardware specs automatically to crash report logs.

### [systemd](https://github.com/systemd/systemd)

- **What it does:** The foundational init system and service manager for modern Linux operating systems.
- **Use Cases:** Ensuring high availability by automatically restarting crashed server applications; replacing traditional Cron jobs with precise systemd timers.

### [Protocol Buffers (protobuf)](https://github.com/protocolbuffers/protobuf)

- **What it does:** A language-neutral, platform-neutral extensible mechanism by Google for serializing structured data. Highly compressed and binary.
- **Use Cases:** Establishing strict, high-speed data contracts between microservices; optimizing payload sizes for IoT telemetry.

### [Get Shit Done (GSD)](https://github.com/gsd-build/get-shit-done)

- **What it does:** An AI CLI tool that uses simple prompts to scaffold projects, run scripts, and automate backend developer environments.
- **Use Cases:** Rapidly generating microservice folder structures; automating deployment scripts.

### [promptfoo](https://github.com/promptfoo/promptfoo)

- **What it does:** A CLI tool for evaluating, testing, and optimizing LLM prompts and outputs to prevent hallucinations.
- **Use Cases:** Writing safety tests for AI-generated SQL queries; automating QA checks for enterprise chatbots.

### [workerd](https://github.com/cloudflare/workerd)

- **What it does:** The open-source, V8-based runtime that powers Cloudflare Workers, allowing you to run serverless JavaScript/Wasm locally.
- **Use Cases:** Handling high-volume webhooks instantly before passing filtered data to backend servers.

### [Project Nomad](https://github.com/Crosstalk-Solutions/project-nomad)

- **What it does:** An automation script for instantly deploying and configuring WireGuard VPN servers.
- **Use Cases:** Establishing secure remote access to local development servers; creating closed encrypted networks for field devices.

### [Last 30 Days Skill](https://github.com/mvanhorn/last30days-skill)

- **What it does:** A plugin/skill designed for AI agents to retrieve, summarize, and analyze data or logs strictly from the last 30 days.
- **Use Cases:** Generating automated monthly developer reports; quickly analyzing monthly user support traffic trends.

---

## 📊 Data Processing, RAG & Visualization

### [Apache Superset](https://github.com/apache/superset)

- **What it does:** An enterprise-grade, open-source data exploration and visualization platform. It connects to nearly any SQL database to create interactive dashboards (an alternative to Tableau/PowerBI).
- **Use Cases:** Creating complex business dashboards for real-time sales and network performance; embedding analytics charts directly into customer-facing SaaS products.

### [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)

- **What it does:** A production-grade Optical Character Recognition (OCR) framework by Baidu. It supports 80+ languages with incredible accuracy for extracting text from images and complex documents.
- **Use Cases:** Automating KYC workflows by parsing IDs and licenses directly into databases; deploying lightweight models to mobile/edge devices to read barcodes in poor lighting conditions.

### [Onyx](https://github.com/onyx-dot-app/onyx)

- **What it does:** An enterprise RAG search platform (formerly Danswer) that connects to 40+ corporate data sources (GitHub, Slack, Notion, Jira) with strict access control.
- **Use Cases:** Creating an internal developer knowledge portal for instant code and documentation queries; streamlining customer support ticket resolution.

### [Chandra](https://github.com/datalab-to/chandra)

- **What it does:** An advanced Vision/OCR model specializing in extracting text from highly complex documents (dense tables, structured forms, handwriting).
- **Use Cases:** Digitizing accounting workflows by extracting table data from scanned invoices into JSON; harvesting legacy archival data for RAG models.

### [LightRAG](https://github.com/HKUDS/LightRAG)

- **What it does:** An advanced RAG architecture combining vector retrieval with a Knowledge Graph to rapidly understand deep connections across multiple documents.
- **Use Cases:** Building internal search engines capable of synthesizing answers from disparate PDFs and emails; creating legal review systems for identifying precedents.

### [OpenDataLoader PDF](https://github.com/opendataloader-project/opendataloader-pdf)

- **What it does:** Extracts structured data (text, tables, images) from complex PDFs, optimized for RAG pipelines.
- **Use Cases:** Parsing financial reports; digitizing scanned contracts for database ingestion.

### [MarkItDown](https://github.com/microsoft/markitdown)

- **What it does:** A Microsoft tool that converts Word, Excel, PowerPoint, PDF, HTML, and images into clean Markdown format.
- **Use Cases:** Prepping enterprise documents for AI digestion; converting legacy technical documentation into Git formats.

### [OpenRAG](https://github.com/langflow-ai/openrag)

- **What it does:** A framework for visually designing, testing, and optimizing advanced RAG pipelines.
- **Use Cases:** Building interactive enterprise knowledge bases; integrating smart data-retrieval widgets into web applications.

---

## 🎨 UI Frameworks & Frontend

### [shadcn/ui](https://github.com/shadcn-ui/ui)

- **What it does:** A collection of highly customizable, accessible React components that you copy and paste directly into your project.
- **Use Cases:** Rapidly building premium-looking admin dashboards; standardizing internal enterprise application designs.

---

## 🔐 Security, OSINT & Penetration Testing

### [Sherlock](https://github.com/sherlock-project/sherlock)

- **What it does:** A powerful Open-Source Intelligence (OSINT) CLI tool. It takes a username and concurrently scans over 300 social networks and websites to locate registered accounts.
- **Use Cases:** Brand protection and tracking down impersonators across platforms; assisting InfoSec teams in gathering intelligence or conducting background checks.

### [Strix](https://github.com/usestrix/strix)

- **What it does:** An open-source autonomous "hacker" agent for penetration testing. It scans vulnerabilities in web apps/infrastructure and generates practical Proof of Concepts (PoC).
- **Use Cases:** Integrating automated pentesting into CI/CD pipelines to catch vulnerabilities before deployment; mapping exposed enterprise infrastructure.

### [CyberStrikeAI](https://github.com/Ed1s0nZ/CyberStrikeAI)

- **What it does:** An AI-powered penetration testing platform (written in Go) that orchestrates over 100 security tools to simulate attack chains and generate reports.
- **Use Cases:** Running automated vulnerability scans against API environments.

---

## 🎬 Media, 3D & Audio Generation

### [OpenScreen](https://github.com/siddharthvaddem/openscreen)

- **What it does:** An open-source alternative to premium screen recording software for creating professional-grade video demonstrations. It provides automatic zoom-ins, cursor tracking, and styled backgrounds.
- **Use Cases:** Recording sleek, aesthetic onboarding tutorials for internal enterprise platforms; creating high-quality demo animations for landing pages and marketing.

### [Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam)

- **What it does:** A real-time face swap tool requiring only a single image. Supports both video generation (Deepfake) and live webcam streaming.
- **Use Cases:** Scaling video content production for marketing/tutorials without reshoots; QA testing biometric security systems against visual impersonation.

### [VibeVoice](https://github.com/microsoft/VibeVoice)

- **What it does:** Open models by Microsoft for highly expressive Text-to-Speech (TTS) and Automatic Speech Recognition (ASR). Capable of generating up to 90-minute multi-speaker conversations.
- **Use Cases:** Generating automated podcasts from text scripts with natural breathing and pauses; narrating long-form audiobooks or documentation.

### [Pascal Editor](https://github.com/pascalorg/editor)

- **What it does:** A minimalist, fast 3D architecture editor running directly in the browser using React and WebGPU.
- **Use Cases:** Rapid architectural floor plan prototyping; embedding lightweight 3D drafting tools into real estate web platforms.

### [MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo)

- **What it does:** An automated video generator. You input an idea, and it uses AI to write a script, generate voiceovers, source B-Roll, and output a short vertical video.
- **Use Cases:** Mass-producing niche marketing content; rapidly generating A/B test variations for digital ad campaigns.

### [Arnis](https://github.com/louis-e/arnis)

- **What it does:** A CLI tool that generates 3D city models based on real-world map data (like OpenStreetMap) for export to Blender or game engines.
- **Use Cases:** Procedurally generating accurate city maps for game environments; creating rapid ArchViz context models.

### [Fish Speech](https://github.com/fishaudio/fish-speech)

- **What it does:** An open-source TTS model capable of high-quality voice cloning (Zero-shot) with very short audio samples.
- **Use Cases:** Generating clear voice alerts for custom hardware projects; creating professional AI voiceovers.

---

## 🌐 APIs, Networking & Web Scraping

### [Axios](https://github.com/axios/axios)

- **What it does:** One of the most popular promise-based HTTP clients for JavaScript. It facilitates client-server communication with built-in features for intercepting requests, error handling, and JSON transformation.
- **Use Cases:** Handling client-server communication in React applications to fetch database records; centralizing authentication by using interceptors to automatically attach JWT tokens to outgoing API requests.

### [Lightpanda Browser](https://github.com/lightpanda-io/browser)

- **What it does:** An ultra-fast, headless browser written in Zig, designed specifically for AI web scraping to bypass heavy overhead.
- **Use Cases:** Supplying real-time web context to AI agents; scraping competitor pricing data instantly.

---

## 💼 Business, Finance & Operations

### [Twenty](https://github.com/twentyhq/twenty)

- **What it does:** A modern, open-source CRM platform built as a self-hostable alternative to giants like Salesforce and HubSpot, ensuring total data ownership.
- **Use Cases:** Establishing a secure, internal CRM to handle sensitive customer data while eliminating per-seat licensing costs; building custom automations via its GraphQL API to sync internal apps with client records.

### [Dexter](https://github.com/virattt/dexter)

- **What it does:** An autonomous AI agent designed specifically for financial research. It pulls market data (P&L, balance sheets), reflects on the numbers, and outputs verified conclusions.
- **Use Cases:** Generating automated comparative financial research reports; continuously gathering macroeconomic intelligence.

### [TradingAgents](https://github.com/TauricResearch/TradingAgents)

- **What it does:** A multi-agent simulation environment based on LLMs designed for financial research.
- **Use Cases:** Backtesting new trading algorithms in a simulated environment; stress-testing portfolios.

### [TradingAgents-CN](https://github.com/hsliuping/TradingAgents-CN)

- **What it does:** A fork of TradingAgents tailored for the Chinese development ecosystem and local LLMs.
- **Use Cases:** Building financial simulations focused on Asian markets and reading local social media sentiment.

### [TaxHacker](https://github.com/vas3k/TaxHacker)

- **What it does:** An open-source system designed to calculate, compare, and optimize tax scenarios across different jurisdictions.
- **Use Cases:** Evaluating the economic viability of corporate relocation; simulating global net salary outcomes for remote freelancers.

---

## 📡 Sensors & Hardware Integrations

### [WiFi DensePose](https://github.com/ruvnet/wifi-densepose)

- **What it does:** Turns commodity WiFi signals into real-time human pose estimation and vital sign monitoring without cameras.
- **Use Cases:** Privacy-preserving presence detection and fall monitoring for smart environments.

---

## 🎭 Virtual Characters & Avatars

### [Airi](https://github.com/moeru-ai/airi)

- **What it does:** A self-hosted platform for running AI-driven virtual characters (VTubers) that can chat via voice and act autonomously in games.
- **Use Cases:** Creating interactive 3D avatars capable of autonomous gameplay.

---

## 📚 Learning, Collections & Templates

### [System Prompts Leaks](https://github.com/asgeirtj/system_prompts_leaks)

- **What it does:** A popular archive compiling leaked or extracted system prompts from major industry AI models (ChatGPT, Claude, Gemini, Copilot).
- **Use Cases:** Researching how tech giants formulate guardrails and behavior constraints to apply similar techniques to private AI apps; red-teaming internal chatbots to prevent prompt injection attacks.

### [freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp)

- **What it does:** The complete open-source codebase for one of the world's largest free coding platforms, including its curriculum, automated testing engine, and site architecture.
- **Use Cases:** Forking the repository to build custom internal training and onboarding portals for junior developers; gaining practical experience contributing to a massive Node/React codebase.

### [Coding Interview University](https://github.com/jwasham/coding-interview-university)

- **What it does:** A comprehensive, multi-month syllabus designed to prepare developers (even without a CS degree) for rigorous technical interviews at FAANG companies. Covers data structures, algorithms, and system design.
- **Use Cases:** Self-studying fundamental CS theory to improve daily coding efficiency; structuring fair, challenging, and well-rounded technical assessments for hiring processes.

### [Claude How-to](https://github.com/luongnv89/claude-howto)

- **What it does:** A centralized repository containing guides, optimized prompts, and best-practice workflows for getting the most out of Anthropic's Claude models.
- **Use Cases:** Utilizing prompt templates to guide Claude through complex debugging tasks without hallucinating; learning techniques to manage massive context windows (e.g., hundreds of files) effectively.

### [Claude Code Best Practice](https://github.com/shanraisshan/claude-code-best-practice)

- **What it does:** A dedicated repository for best practices when using the autonomous `claude-code` CLI agent. Covers configuration, safe environment management, and automation tips.
- **Use Cases:** Setting up robust `.claudesignore` files to prevent the agent from accidentally modifying sensitive configurations or build folders; breaking down large test-driven refactoring jobs safely.

### [Everything Claude Code](https://github.com/affaan-m/everything-claude-code)

- **What it does:** A community repository collecting tips, configurations, prompts, and workflows for Anthropic's terminal-based Claude Code agent.
- **Use Cases:** Finding pre-built prompts to automate unit test creation; integrating Claude Code into CI/CD pipelines.

### [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code)

- **What it does:** A structured "Awesome" list curating extensions, libraries, and Model Context Protocol (MCP) servers to expand Claude Code.
- **Use Cases:** Finding an MCP server to let Claude connect directly to local databases; expanding CLI capabilities to manage cloud resources.

### [Awesome LLM Apps](https://github.com/Shubhamsaboo/awesome-llm-apps)

- **What it does:** A rich collection of ready-made apps, templates, and code for building LLM applications with AI Agents and RAG architectures.
- **Use Cases:** Rapid prototyping for developers wanting to integrate voice or agentic workflows quickly.

### [Google Cloud Generative AI](https://github.com/GoogleCloudPlatform/generative-ai)

- **What it does:** The official GCP repository containing notebooks and code samples for integrating Google's Gen AI.
- **Use Cases:** Adding advanced image-to-text scanning to mobile applications.

---

## 🤝 Contributing

Found a cool AI tool that speeds up your workflow? We'd love to add it! Feel free to open a Pull Request with the tool's link, what it does, and a quick example of how you use it.

_Built and maintained as an open-source knowledge base for the developer community._
