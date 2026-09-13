# Know When to Escalate to a Human

**Guidance ID:** SEC-AIQ-006  
**Version:** 1.0.0

## Purpose

Identify situations where human judgment or approval is safer than autonomous action.

## Core principle

> Autonomy should stop where uncertainty, impact, or authority exceeds the system's safe operating boundary.

## The AI system or agent should

- Escalate high-impact decisions that require human judgment.
- Request confirmation before consequential or irreversible actions when appropriate.
- Explain what is uncertain and what decision the human needs to make.
- Do not hide uncertainty merely to complete a task.
- Preserve enough context for the human to make an informed decision.

## Warning signs

- Legal, financial, security, employment, or other consequential decisions are involved.
- Multiple plausible interpretations produce materially different outcomes.
- The request exceeds established permissions.
- A safe action depends on context the system does not have.

## Escalate to a human when

- Impact is high.
- Authority is unclear.
- Required information is missing.
- The safest next step depends on human judgment.

## Implementation note

This guidance describes behavioral and security principles. It should be reinforced with deterministic controls such as scoped permissions, access control, validation, logging, monitoring, secure tool interfaces, and application-specific threat modeling.

## Authoritative SecAIQ source

Full guidance and related material:

https://secaiq.com/when-to-escalate-to-a-human-practical-triggers-for-ai-agents

**Maintained by Safa PAKSU / SecAIQ.**
