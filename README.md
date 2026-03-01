# Awesome AI Software Engineering

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A curated list of tools, frameworks, and resources for AI-powered software engineering.

Modern software development is being transformed by AI agents, coding copilots, and spec-driven workflows. This repository collects the best resources for developers who want to leverage AI as a true engineering partner.

## Contents

- [Philosophy](#philosophy)
- [Quick Start](#quick-start)
- [AI Coding Agents](#ai-coding-agents)
- [Coding Copilots](#coding-copilots)
- [Multi-Agent Frameworks](#multi-agent-frameworks)
- [Agent SDKs](#agent-sdks)
- [LLM Observability & Gateways](#llm-observability--gateways)
- [LLM Inference Engines](#llm-inference-engines)
- [Spec-Driven Development](#spec-driven-development)
- [Skills & Plugins](#skills--plugins)
- [Methodologies](#methodologies)
- [Learning Resources](#learning-resources)

---

## Philosophy

AI-powered software engineering isn't about replacing developers—it's about amplifying their capabilities. The most effective approach combines:

1. **Specifications before code** - Clear intent leads to better outcomes
2. **AI as collaborator** - Leverage AI for execution while you focus on architecture
3. **Living documentation** - Keep context fresh and accessible
4. **Iterative refinement** - Build in feedback loops

Read more in our [Philosophy Guide](concepts/philosophy.md).

---

## Quick Start

**Step 1:** Choose your primary tool
- New to AI coding? Start with [Claude Code](https://github.com/anthropics/claude-code) or [Cursor](https://cursor.sh)
- Want maximum control? Try [Aider](https://github.com/paul-gauthier/aider) or [OpenCode](https://github.com/anomalyco/opencode)
- Building custom agents? Use [Claude Agent SDK](https://platform.claude.com/docs/en/agent-sdk/overview)

**Step 2:** Adopt a spec-driven workflow
- Write a brief PRD before starting any feature
- Use the [PRD template](patterns/spec-templates/PRD.md.template) to structure your requirements

**Step 3:** Iterate and refine
- Review AI-generated code critically
- Build your prompt library for common patterns
- Track what works in your CONTEXT.md

See our full [Getting Started Guide](guides/getting-started.md).

---

## AI Coding Agents

Autonomous agents that can plan, write, and debug code with minimal supervision.

| Name | Author | Description |
|------|--------|-------------|
| [Claude Code](https://github.com/anthropics/claude-code) | Anthropic | Official CLI for Claude that handles complex software engineering tasks autonomously |
| [Codex CLI](https://github.com/openai/codex) | OpenAI | Terminal-based coding agent powered by GPT models |
| [OpenCode](https://github.com/anomalyco/opencode) | Anomaly | Open-source AI coding agent with extensible architecture |
| [Aider](https://github.com/paul-gauthier/aider) | Paul Gauthier | AI pair programming in your terminal with git integration |
| [cecli (aider-ce)](https://github.com/dwash96/cecli) | dwash96 | Aider fork with a different style of AI-assisted coding |
| [Mentat](https://github.com/AbanteAI/mentat) | Abante AI | AI coding assistant that understands your entire codebase |
| [GPT Engineer](https://github.com/gpt-engineer-org/gpt-engineer) | GPT Engineer | Generate entire codebases from a single prompt |
| [Sweep](https://github.com/sweepai/sweep) | Sweep AI | AI-powered junior developer that handles GitHub issues |
| [Mistral Vibe](https://github.com/mistralai/mistral-vibe) | Mistral AI | CLI coding assistant with interactive chat, code search, and shell integration |
| [Google Antigravity](https://antigravity.google) | Google | Agentic IDE with multi-agent deployment powered by Gemini 3 |
| [OpenAI Codex](https://openai.com/codex) | OpenAI | Cloud-based coding agent for autonomous development tasks |
| [GitHub Copilot CLI](https://github.blog/changelog/2026-01-14-github-copilot-cli-enhanced-agents-context-management-and-new-ways-to-install/) | GitHub | Terminal-based AI assistant with agent delegation and parallel execution |
| [GitHub Copilot Coding Agent](https://github.com/features/copilot/agents) | GitHub | Cloud-hosted autonomous agent that works on GitHub issues |
| [OpenPaw](https://github.com/daxaur/openpaw) | daxaur | Turns Claude Code into a personal assistant with 38 skills (Telegram, Discord, Obsidian, daily briefings) via `npx pawmode` |

---

## Coding Copilots

IDE-integrated assistants that augment your coding workflow.

| Name | Author | Description |
|------|--------|-------------|
| [Cursor](https://cursor.sh) | Cursor Inc | AI-first code editor built on VSCode with deep model integration |
| [Cline](https://github.com/cline/cline) | Cline | Autonomous coding agent that lives in your IDE |
| [Kilo Code](https://github.com/Kilo-Org/kilocode) | Kilo Org | VSCode extension for AI-assisted development with MCP support |
| [GitHub Copilot](https://github.com/features/copilot) | GitHub | AI pair programmer suite with Chat, CLI, coding agent, and code review agent |
| [Continue](https://github.com/continuedev/continue) | Continue | Open-source autopilot for software development |
| [Supermaven](https://supermaven.com) | Supermaven | Ultra-fast code completions with 1M token context |
| [Tabnine](https://www.tabnine.com) | Tabnine | AI code assistant trained on your codebase |
| [Windsurf](https://windsurf.com) | Codeium | AI-first IDE with Cascade agentic flow and multi-file editing |
| [Roo Code](https://github.com/RooCodeInc/Roo-Code) | Roo Code Inc | Open-source AI assistant with role-specific modes (Architect, Code, Debug, Test) |

---

## Multi-Agent Frameworks

Coordinate multiple AI agents for complex engineering tasks.

| Name | Author | Description |
|------|--------|-------------|
| [Gas Town](https://github.com/steveyegge/gastown) | Steve Yegge | Multi-agent coding framework with specialized agent roles |
| [Ralph](https://github.com/snarktank/ralph) | Snarktank | PRD-driven development with automated planning loops |
| [CrewAI](https://github.com/joaomdmoura/crewai) | Joao Moura | Framework for orchestrating role-playing autonomous agents |
| [AutoGen](https://github.com/microsoft/autogen) | Microsoft | Multi-agent conversation framework (⚠️ maintenance mode - see [Microsoft Agent Framework](#agent-sdks)) |
| [MetaGPT](https://github.com/geekan/MetaGPT) | MetaGPT | Multi-agent framework that turns requirements into PRDs and code |
| [ChatDev](https://github.com/OpenBMB/ChatDev) | OpenBMB | Collaborative AI agents simulating a software company |

---

## Agent SDKs

Build production AI agents programmatically with these SDKs.

| Name | Author | Languages | Description |
|------|--------|-----------|-------------|
| [Claude Agent SDK](https://platform.claude.com/docs/en/agent-sdk/overview) | Anthropic | Python, TypeScript | Build production agents using Claude Code as a library. Built-in tools, hooks, subagents, MCP support |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) | Microsoft | Python, .NET | Unified framework combining AutoGen and Semantic Kernel (GA Q1 2026) |
| [LangChain](https://github.com/langchain-ai/langchain) | LangChain | Python, JS | Popular framework for LLM-powered applications |
| [LlamaIndex](https://github.com/run-llama/llama_index) | LlamaIndex | Python | Data framework for LLM applications with RAG |

---

## LLM Observability & Gateways

Monitor, debug, and route LLM traffic in production.

| Name | Author | Type | Description |
|------|--------|------|-------------|
| [LiteLLM](https://github.com/BerriAI/litellm) | BerriAI | Gateway | Unified API proxy for 100+ LLM providers with load balancing, spend tracking, and caching |
| [Langfuse](https://github.com/langfuse/langfuse) | Langfuse | Observability | Open-source LLM engineering platform with tracing, prompt management, and evaluations |
| [Helicone](https://github.com/Helicone/helicone) | Helicone | Observability | LLM observability with request logging, cost tracking, and prompt analytics |
| [OpenLLMetry](https://github.com/traceloop/openllmetry) | Traceloop | Observability | OpenTelemetry-based tracing for LLMs, integrates with Datadog, Honeycomb, Grafana |
| [Logfire](https://github.com/pydantic/logfire) | Pydantic | Observability | Python-native observability with OpenTelemetry, excellent FastAPI/Pydantic integration |

---

## LLM Inference Engines

Self-host and run LLMs on your own infrastructure.

| Name | Author | Description |
|------|--------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | vLLM Project | High-throughput LLM serving with PagedAttention for efficient memory management |
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | GGML | C/C++ LLM inference with broad hardware support (CPU, GPU, Apple Silicon) |
| [SGLang](https://github.com/sgl-project/sglang) | SGLang Project | Fast serving framework with RadixAttention and structured generation support |

---

## Spec-Driven Development

Tools and methodologies for requirements-first AI development.

| Name | Author | Description |
|------|--------|-------------|
| [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD) | BMAD | Breakthrough Method for AI-Driven development with structured specs |
| [Shotgun](https://github.com/shotgun-sh/shotgun) | Shotgun | Spec-based code generation with planning phase |
| [Spec-Kit](https://github.com/github/spec-kit) | GitHub | Toolkit for managing specifications in AI workflows |
| [OpenSpec](https://github.com/Fission-AI/OpenSpec) | Fission AI | Open standard for AI-consumable specifications |
| [Get Shit Done](https://github.com/glittercowboy/get-shit-done) | Glitter Cowboy | Opinionated workflow for shipping with AI assistance |
| [SpecStory](https://github.com/specstoryai/specstory) | SpecStory | Turn user stories into detailed specifications |
| [nano-spec](https://github.com/tao-hpu/nano-spec) | tao-hpu | Lightweight task specification framework with 4-doc structure for AI development |

---

## Skills & Plugins

Extend your AI coding tools with custom capabilities.

| Name | Author | Description |
|------|--------|-------------|
| [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | ComposioHQ | Curated collection of Claude Code skills and extensions |
| [everything-claude-code](https://github.com/affaan-m/everything-claude-code) | Affaan M | Comprehensive guide and resources for Claude Code |
| [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | hesreallyhim | Collection of Claude Code tips, tricks, and skills |
| [awesome-claude-skills](https://github.com/VoltAgent/awesome-claude-skills) | VoltAgent | Skills library for extending Claude Code capabilities |
| [claudekit-skills](https://github.com/mrgoonie/claudekit-skills) | mrgoonie | Ready-to-use skills for Claude Code workflows |
| [MCP Servers](https://github.com/modelcontextprotocol/servers) | Anthropic | Official Model Context Protocol server implementations |

---

## Methodologies

Workflows and approaches for AI-assisted development.

### PRD Loops

The PRD (Product Requirements Document) loop is a cyclic workflow:

1. **Specify** - Write clear requirements in a PRD
2. **Plan** - Let AI break down the work into tasks
3. **Execute** - AI implements while you review
4. **Refine** - Update the PRD based on learnings
5. **Repeat** - Continue until complete

### Spec-First Development

Start every feature with a specification:
- Forces clarity of thought before coding
- Gives AI maximum context to work with
- Creates documentation as a byproduct
- Enables better code review

### Agent Swarms

Use multiple specialized agents for complex projects:
- **Architect Agent** - Designs system structure
- **Developer Agent** - Writes implementation code
- **Reviewer Agent** - Checks code quality
- **Tester Agent** - Creates and runs tests

See our [Spec-Driven Development Guide](guides/spec-driven-development.md) for details.

---

## Learning Resources

### In This Repository

| Guide | Description |
|-------|-------------|
| [Getting Started](guides/getting-started.md) | Your first steps with AI-powered development |
| [Spec-Driven Development](guides/spec-driven-development.md) | Deep dive into specification-first workflows |
| [Choosing Your Tools](guides/choosing-your-tools.md) | How to select the right AI coding tools |
| [Philosophy](concepts/philosophy.md) | Core principles and mindset |
| [Glossary](reference/glossary.md) | Key terms and definitions |

### Spec Templates

Ready-to-use templates for your projects:
- [PRD Template](patterns/spec-templates/PRD.md.template) - Product requirements document
- [AGENTS.md Template](patterns/spec-templates/AGENTS.md.template) - Multi-agent configuration
- [CONTEXT.md Template](patterns/spec-templates/CONTEXT.md.template) - Project state tracking

### External Resources

- [Anthropic Claude Documentation](https://docs.anthropic.com)
- [Claude Agent SDK Documentation](https://platform.claude.com/docs/en/agent-sdk/overview)
- [Model Context Protocol](https://modelcontextprotocol.io)
- [Prompt Engineering Guide](https://www.promptingguide.ai)

---

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### How to Add a Resource

1. Ensure the resource is actively maintained
2. Verify it adds unique value to the list
3. Submit a PR with the appropriate category
4. Include a clear, concise description

---

## License

[MIT](LICENSE) - Feel free to use this for your own awesome lists.

---

## Acknowledgments

This list is inspired by the amazing work of:
- The [awesome](https://github.com/sindresorhus/awesome) list community
- All the developers building AI coding tools
- Everyone sharing their workflows and learnings

---

*Built with AI assistance, curated by humans.*
