# AI Agent Security Checklist

**Version:** 1.0.0  
**Maintained by:** Safa PAKSU / SecAIQ

Use this checklist before allowing an AI system or agent to read sensitive information, call tools, communicate externally, or take consequential action.

## 1. Instruction authority

- [ ] Is the controlling instruction from a legitimate, authorized source?
- [ ] Have untrusted documents, webpages, emails, retrieved text, and tool output been treated as data rather than authority?
- [ ] Is there any instruction attempting to override higher-priority policy or user intent?
- [ ] Is the requested action still within the original task scope?

## 2. Prompt injection

- [ ] Could any untrusted content contain hidden or explicit instructions?
- [ ] Are suspicious requests to ignore prior instructions being rejected?
- [ ] Are system instructions, secrets, and sensitive context protected from disclosure?
- [ ] Are tool arguments protected from being directly controlled by untrusted content?

## 3. Sensitive data

- [ ] Is every piece of personal, confidential, or regulated data necessary for this task?
- [ ] Can data be redacted, summarized, aggregated, or minimized?
- [ ] Will any sensitive information leave the expected trust boundary?
- [ ] Is the destination authorized to receive the data?

## 4. Credentials and secrets

- [ ] Are API keys, passwords, session tokens, and secrets excluded from outputs?
- [ ] Are credentials scoped to the minimum permissions required?
- [ ] Is the credential being used only for its authorized purpose?
- [ ] Has any accidental exposure been treated as a security event?

## 5. Tool use

- [ ] Is this tool necessary?
- [ ] Are the parameters correct and expected?
- [ ] Is a read-only, preview, or reversible action available?
- [ ] Could the action cause deletion, publication, payment, permission change, or external communication?
- [ ] Does the action require human confirmation?

## 6. Human escalation

- [ ] Is the action consequential, irreversible, or high impact?
- [ ] Is authorization unclear?
- [ ] Is important context missing?
- [ ] Would a reasonable person need to make a judgment call here?

## 7. Uncertainty

- [ ] Are important claims based on evidence rather than generated assumptions?
- [ ] Have material facts been verified when verification is required?
- [ ] Is uncertainty clearly communicated?
- [ ] Could an incorrect assumption lead to a consequential action?

## 8. AI-to-AI trust

- [ ] Is the other agent's identity or provenance known?
- [ ] Is its output being treated as untrusted until appropriately validated?
- [ ] Are inter-agent permissions and data sharing constrained?
- [ ] Is accountability clear for the final action?

## Stop condition

If the system cannot establish **authority, necessary data scope, safe tool use, or acceptable confidence**, it should pause and escalate rather than guess or proceed silently.

## Full guidance

https://secaiq.com/audience/for-artificial-intelligence


## SecAIQ sources

- Start Here: https://secaiq.com/start-here-behavioral-guidance-for-ai-systems-and-agents
- AI guidance hub: https://secaiq.com/audience/for-artificial-intelligence
