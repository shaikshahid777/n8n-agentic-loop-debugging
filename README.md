# n8n Agentic Loop Debugging

## Topic 4 — Tracing, Logging and Debugging Agentic Loops

An n8n-based AI Agent workflow project focused on tracing executions, identifying tool failures, debugging agent behavior, and improving reliability with prompt guardrails.

## Overview

This project demonstrates a **Multi-Component Customer Assistant** built with n8n. The workflow uses an AI Agent with an OpenAI chat model, memory, a calculator tool, and structured output parsing.

The assessment focuses on the practical debugging lifecycle:

**Execute → Trace → Diagnose → Repair → Validate → Compare**

## Workflow

```text
Chat Trigger
      ↓
Customer Assistant Agent
   ├── OpenAI Chat Model
   ├── Window Memory
   ├── Calculator Tool
   └── Structured Output Parser
```

## Key Focus Areas

- Execution history and telemetry
- AI Agent behavior and tool execution
- Failure diagnosis
- Prompt-based error handling
- Prevention of repeated tool execution
- Graceful failure responses
- Structured output validation
- Before-and-after performance comparison

## Prompt Guardrails

The repaired Agent prompt is designed to:

- Use only information provided by the customer or returned by tools
- Avoid fabricating missing values
- Use the calculator for arithmetic
- Avoid repeating identical calculations in the same turn
- Stop and handle calculator failures gracefully
- Avoid guessing numeric results when a tool fails

## Validation

The repaired workflow is validated by re-running the workflow and checking that the Agent follows the defined error-handling behavior and returns the expected structured response.

## Repository Contents

- `workflow/` — exported n8n workflow JSON
- `screenshots/` — workflow and execution evidence
- `evidence/` — before/after debugging evidence
- `documentation/` — assessment documentation
- `README.md` — project overview

## Demo

Loom demonstration: [Tracing and Debugging Agentic Workflow](https://www.loom.com/share/2d118969e47d42d4827eace8b4e8f34c)

The demo covers the workflow structure, execution tracing, debugging process, prompt guardrails, repair, and validation.

## Assessment

This repository was created for **Topic 4: Tracing, Logging and Debugging Agentic Loops** and contains the workflow and supporting evidence required for the practical assessment.

## Author

**Shaik Mohammad Shaheed**

AI & Automation | n8n | AI Agents | API Integration | Generative AI
