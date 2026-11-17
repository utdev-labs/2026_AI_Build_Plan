# 2026 AI Build Plan

> **Updated 14-Week Step-by-Step Build Plan** — MIT Rigor + Columbia Tooling

## Key Topics & Tools from the Columbia / Simplilearn Curriculum

The Columbia University (School of Professional Studies) / Simplilearn **Certificate in Agentic AI Engineering** focuses heavily on applied agent orchestration, runtime harness engineering, and production deployment. That makes it a strong tactical complement to the formal specification methodology of the **MIT CSAIL** program.

- **Core Cognitive & Prompting Foundations:** Transformers, reasoning models, ReAct (Reason + Act), Chain-of-Thought (CoT), Reflection loops, context engineering, and structured prompt optimization.
- **Rapid Workflow Automation & Prototyping:** n8n (visual event-driven triggers, app integrations, AI nodes), Gradio, and Hugging Face Spaces for rapid UI validation.
- **Model Layer, Tooling & Retrieval:** OpenAI APIs (multimodal text/image/audio/video), LangChain, function calling, Model Context Protocol (MCP), Agentic RAG, and RAGAS (automated RAG evaluation).
- **Multi-Agent Orchestration & Protocols:** LangGraph (stateful graph workflows), CrewAI (role-based collaboration), supervisor/handoff architectures, and Agent-to-Agent (A2A) communication protocols.
- **Harness Engineering & Autonomous Loops:** Designing the deterministic runtime wrapper around an LLM: managing policy/instruction files (`AGENTS.md`, `SOUL.md`, `USER.md`), memory, skill layers, tool approval gates, and audit trails using OpenAI Agents SDK, Hermes, OpenClaw, Claude Code, and Codex CLI.
- **Agent Swarms & Asynchronous Routines:** Dynamic task decomposition, parallel execution, plan → act → observe → refine loops, and scheduled cron/heartbeat routines.
- **Production Hardening & Deployment:** Input/output/tool-use guardrails, FastAPI, Docker, AWS / Azure, CI/CD regression gates, golden test sets, distributed tracing, and incident response.

## 14-Week Build Plan

This integrated schedule keeps the MIT CSAIL concept-driven design in Weeks 1–6, so you never build brittle "spaghetti agents", while weaving Columbia's concrete tooling stack (n8n, MCP, LangGraph, CrewAI, RAGAS, Harness Engineering, FastAPI/Docker) into the build and hardening phases.

| Week | Phase | Integrated Focus & Concrete Deliverables |
|:----:|-------|------------------------------------------|
| 1 | Design | **System Scope & Refusal Boundaries:** Define target users, the 4-layer GenAI stack, and explicit refusal rules for your Multi-Source Due Diligence & Deal Underwriting Engine. |
| 2 | Design | **Concept Decomposition:** Isolate 4–6 independent concepts (Document Ingestion, Ledger Normalization, Scenario Modeling, Risk Flagging, Memo Synthesis). Define state schemas and operational principles. |
| 3 | Design | **Synchronization & Low-Code Prototyping:** Define state synchronization rules. Build a rapid non-LLM state simulation in Python alongside a quick n8n trigger/webhook prototype to validate end-to-end data flow. |
| 4 | Build Bridge | **Spec-to-Prompt & Cognitive Loops:** Translate concept specs into structured prompts using ReAct, CoT, and Reflection patterns. Establish a 20-case golden evaluation dataset. |
| 5 | Build Bridge | **Harness Engineering Foundations:** Build your agent runtime harness (`AGENTS.md` / policy instruction files, memory layer, and audit logging) using Claude Code / OpenAI Agents SDK and stand up MCP tool interfaces. |
| 6 | Build Bridge | **Failure Mode Stress-Testing:** Run adversarial inputs against your harness. Tighten concept boundaries, tool-use approval rules, and refusal triggers where boundaries bleed. |
| 7 | Systems | **Multi-Agent Architecture Mapping:** Implement your orchestration layer in LangGraph (for strict state-machine concepts) and CrewAI (for collaborative research/verification roles), wiring A2A handoffs with written ADRs. |
| 8 | Systems | **Agentic RAG & Evaluation:** Implement hybrid vector/graph storage and Agentic RAG for lease/financial document traversal. Benchmark retrieval faithfulness and context recall using RAGAS. |
| 9 | Systems | **Loop Engineering & Swarm Execution:** Add iterative plan → act → observe → refine loops and parallel sub-agent swarms to process multi-document data rooms concurrently. Wrap in FastAPI + Gradio for stakeholder testing. |
| 10 | Engineering | **Threat Modeling & Least Privilege:** Audit trust boundaries against the OWASP LLM Top 10. Enforce scoped MCP credentials, human-in-the-loop approval gates, and tool-abuse defenses. |
| 11 | Engineering | **Defense-in-Depth Guardrails:** Implement deterministic input/output guardrails to neutralize indirect prompt injections hidden inside uploaded financial PDFs or seller disclosures. |
| 12 | Engineering | **Observability & Telemetry:** Instrument distributed tracing across LangGraph nodes and MCP tool calls. Profile p50/p95 latency, token burn per concept, and failure modes. |
| 13 | Engineering | **Model Routing & CI/CD Gates:** Implement dynamic model routing inside your harness (simple extraction to smaller models, complex synthesis to reasoning models) and automate RAGAS + golden dataset regression gates in CI/CD. |
| 14 | Portfolio | **Containerized Deployment & Case Study:** Containerize with Docker, deploy to AWS or Azure with scheduled monitoring routines, and publish your architecture case study with benchmark metrics. |

## Strategic Takeaway: Combining Both Curricula

- **Where MIT CSAIL leads:** Formal system specification (*The Essence of Software*), avoiding premature framework lock-in, and mathematical/architectural justification before writing code.
- **Where Columbia / Simplilearn leads:** Hands-on execution with modern orchestration frameworks (LangGraph, CrewAI, MCP, A2A), Harness Engineering (wrapping models in deterministic policies, memory, and audit trails), and production DevOps (RAGAS, FastAPI, Docker, AWS/Azure).
