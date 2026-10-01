---
name: framework-architecture-advisor
description: "Compares and recommends agent frameworks (LangGraph, CrewAI, AutoGen, Agno) based on architectural requirements."
---

# Framework Architecture Advisor

## Overview
The `framework-architecture-advisor` skill evaluates project requirements and maps technical constraints to optimal multi-agent frameworks, preventing architectural mismatches.

## Evaluation Criteria
| Requirement | Recommended Framework | Key Justification |
|---|---|---|
| Deterministic graph execution & checkpointing | **LangGraph** | Cycle support, human-in-the-loop state interrupts, durable state. |
| Role-based task delegation & rapid prototyping | **CrewAI** | Declarative agent roles, sequential/hierarchical task processes. |
| Conversational multi-agent consensus & debate | **AutoGen** | Group chat dynamics, code execution sandbox, custom agents. |
| High-performance async agents with multimodal DBs | **Agno** | Vector database integrations, lightweight memory management. |

## Guidance Pipeline
1. Ingest user requirements (state complexity, team coordination needs, deployment targets).
2. Rank frameworks based on feature-fit matrices and operational trade-offs.
3. Provide concrete migration pathways and trade-off summaries.
