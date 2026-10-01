---
name: agent-template-scaffolder
description: "Scaffolds production-ready agent project templates with framework configs, dependencies, and environment files."
---

# Agent Template Scaffolder

## Overview
The `agent-template-scaffolder` skill provisions self-contained agent projects modeled after the 21 reference implementations in the `agents/` catalog. It ensures all scaffolding includes modular prompt definitions, tool bindings, isolated virtual environments, and `.env.example` templates.

## Operational Workflow
1. **Determine Agent Topology:** Identify whether the target agent requires a single-agent loop, supervisor-worker orchestration, or multi-agent debate.
2. **Select Target Framework:** Configure runtime dependencies according to the chosen framework:
   - `langgraph`: StateGraph, memory checkpointers, tool nodes.
   - `crewai`: Agent roles, tasks, crews, and MCP tool adapters.
   - `autogen`: ConversableAgent, user proxy, group chat managers.
   - `agno`: Structured storage, knowledge bases, reasoning agents.
3. **Generate Directory Structure:**
   ```
   agent-name/
   ├── agent.py
   ├── tools.py
   ├── prompts.py
   ├── requirements.txt
   ├── README.md
   └── .env.example
   ```
4. **Enforce Security Defaults:** Include API key placeholders, rate-limiting guards, and mock testing harnesses by default.
