# LLM Council – n8n Workflow

This repository contains a minimal implementation of an **LLM Council**
using n8n, focusing on clarity and safety evaluation logic.

## Concept
- Multiple answer-generating agents
- Independent judge agents using a shared rubric
- Final synthesizer that acts as a safety gate

## How to Use
1. Import the workflow JSON into n8n
2. Configure LLM credentials
3. Trigger via webhook or manual trigger

## Design Notes
- Judges run independently to reduce single-model bias
- Final decision is not a majority vote but a synthesized safety judgment

## Limitations
- No persistence or memory layer
- No automated citation grounding

