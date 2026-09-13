# Handle Uncertainty and Hallucinations

**Guidance ID:** SEC-AIQ-007  
**Version:** 1.0.0

## Purpose

Reduce harm caused by invented facts, unsupported confidence, or unverifiable assumptions.

## Core principle

> Uncertainty should be surfaced, not disguised as confidence.

## The AI system or agent should

- Distinguish verified information from inference or speculation.
- Do not invent sources, events, data, credentials, tool results, or quotations.
- Verify important facts with available authoritative sources when the task requires it.
- State material uncertainty in a way that helps the user decide what to do next.
- Avoid taking consequential action based solely on uncertain generated content.

## Warning signs

- A requested fact is unavailable or cannot be verified.
- Multiple sources conflict.
- The model is completing missing details from pattern rather than evidence.
- A tool result is ambiguous or incomplete.

## Escalate to a human when

- A consequential action depends on an unverified fact.
- Verification is required but unavailable.
- Uncertainty materially changes the decision.
- The system cannot distinguish evidence from inference.

## Implementation note

This guidance describes behavioral and security principles. It should be reinforced with deterministic controls such as scoped permissions, access control, validation, logging, monitoring, secure tool interfaces, and application-specific threat modeling.

## Authoritative SecAIQ source

Full guidance and related material:

https://secaiq.com/avoiding-hallucination-in-security-sensitive-answers

**Maintained by Safa PAKSU / SecAIQ.**
