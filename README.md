# Workflow Execution Timer – Autonomous SRE Agent

An n8n-based workflow monitoring system that measures workflow execution time, detects slow executions, analyzes performance issues, and generates alerts automatically.

## Project Overview

The Workflow Execution Timer – Autonomous SRE Agent is developed using n8n for workflow automation.

The project monitors the execution time of a workflow and compares it with a predefined threshold. If the execution takes longer than the allowed time, the workflow identifies it as a slow execution and triggers an Autonomous SRE Agent for further analysis.

The system also creates performance and alert logs for future analysis.

## Objectives


- Measure workflow execution time.
- Record workflow start and end timestamps.
- Calculate total execution duration.
- Detect slow workflow executions.
- Analyze performance issues using an AI agent.
- Generate performance and alert logs automatically.

## Technologies Used

- n8n
- JavaScript
- AI Agent
- Google Gemini / Ollama
- IF Node
- Code Node
- Write File Node
- JSON

## Workflow

The workflow follows these main steps:


Manual Trigger
      ↓
Configuration
      ↓
Start Timer & Initialize Checkpoints
      ↓
Processing Steps
      ↓
Checkpoint
      ↓
Calculate Total Duration
      ↓
Write Performance Log
      ↓
Is Execution Slow?
      ↓
   ┌──┴──┐
   ↓     ↓
Normal  Slow
         ↓
Autonomous SRE Agent
         ↓
Prepare Alert File
         ↓
Write Alert Log
