---
name: multi-agent-orchestrator
description: "Configures multi-agent debate, collaboration, and supervisor-worker patterns for complex workflows."
---

# Multi-Agent Orchestrator

## Overview
The `multi-agent-orchestrator` skill designs communication protocols, consensus voting schemes, and turn-taking strategies across multi-agent collectives.

## Supported Coordination Topologies
1. **Hierarchical Supervisor:** A central supervisor evaluates task states, delegates sub-goals to specialist agents, and synthesizes final outputs.
2. **Peer-to-Peer Debate:** Opposing agents critique intermediate reasoning steps to reduce hallucination and improve factual accuracy.
3. **Sequential Pipeline:** Discrete agents pass typed payloads through sequential refinement stages with strict validation checks.

## Protocol Standards
- Use typed JSON schemas for inter-agent communication messages.
- Impose maximum round limits (e.g., max 6 debate turns) to prevent conversational deadlock.
- Include automated consensus thresholds before terminating execution.
