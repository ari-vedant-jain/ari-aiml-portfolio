# Simple Techniques for Common LLM Vulnerabilities Remediation

## Overview

LLM deployments are exposed to various vulnerabilities including:

- Prompt-injection  
- Jailbreak attempts  
- Data exfiltration  
- Toxic or policy-violating content  

This page summarizes practical remediation techniques from my article:  
**“Simple Techniques for Common LLM Vulnerabilities Remediation”**.

---

## Example Remediation Patterns

- **Input Validation & Normalization**
  - Sanitize and normalize user inputs before passing to the LLM.
- **Prompt Hardening**
  - Explicitly instruct the model to ignore user attempts to override system instructions.
- **Output Filtering**
  - Post-process outputs via classifiers, regexes, or policy models.
- **Structured Responses**
  - Constrain outputs to JSON, enums, or templates to reduce uncontrolled free-text.
- **Least-Privilege Tool Use**
  - Limit which tools or APIs an agent can invoke based on trust and risk levels.

---

## Role in My Work

These techniques appear across:

- Guardrail design for Bedrock and DeepSeek-R1.  
- Red-teaming remediation cycles for Mosaic AI endpoints.  
- Multi-agent RAG systems with security-aware orchestrators.

Combined with TDD-style prompt-injection testing, they form a **practical defense-in-depth** approach for LLM systems.
