---
name: agent-benchmark-evaluator
description: "Benchmarks agent latency, token utilization, task completion rates, and safety guardrails."
---

# Agent Benchmark Evaluator

## Overview
The `agent-benchmark-evaluator` skill provides objective measurement harnesses to benchmark agent quality, operational cost, and safety boundaries.

## Evaluation Dimensions
1. **Task Success Rate:** Empirical evaluation against ground-truth datasets and golden QA benchmarks.
2. **Token Efficiency:** Ratio of productive reasoning tokens versus circular exploration or tool retries.
3. **Execution Latency:** P50, P90, and P99 latency tracking across multi-step agent trajectories.
4. **Safety & Robustness:** Prompt injection resistance, jailbreak defense, and schema validation error recovery.
