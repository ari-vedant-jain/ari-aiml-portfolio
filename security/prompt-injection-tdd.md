# Test-Driven Development (TDD) for Prompt-Injection Testing

## Overview

Prompt-injection is one of the most common and dangerous classes of LLM vulnerabilities. Instead of treating it as an ad-hoc problem, I advocate for **test-driven development (TDD)** applied to prompt and policy design.

Based on my article:  
**“Test-Driven Development for Prompt Injection Testing: Fail Fast, Learn, Iterate”**.

---

## Core Idea

Apply TDD principles to AI security:

1. Define **threat models and attack prompts** up front.  
2. Encode them as **tests** that your system must resist.  
3. Run these tests iteratively as you refine:
   - Prompts  
   - Guardrails  
   - Policies  
   - Model configurations  

If tests fail, you **fix the vulnerability** and rerun.

---

## Components

- **Attack Libraries**
  - Collections of known and hypothesized injection patterns.
- **Automated Test Harness**
  - Executes prompts against your system (LLM + orchestration + guardrails).
- **Evaluation**
  - Classifies outcomes as pass/fail based on safety and policy criteria.
- **Reporting**
  - Summaries of vulnerabilities, regressions, and resilience trends.

---

## Benefits

- Moves AI security from **reactive** to **proactive and iterative**.  
- Gives teams a shared language around “what we defend against”.  
- Integrates AI security with normal CI/CD and testing practices.

---

## Related Articles

- [Test-Driven Development for Prompt Injection Testing](https://medium.com/@ari_in_media_res/test-driven-development-for-prompt-injection-testing-fail-fast-learn-iterate-55e0c85cadc3)  
- [Taming the Trojan: A Guide to Combating Prompt Injection](https://medium.com/@ari_in_media_res/taming-the-trojan-a-guide-to-combating-prompt-injection-17d2ae06fc99)  
- [Simple Techniques for Common LLM Vulnerabilities Remediation](https://medium.com/@ari_in_media_res/simple-techniques-for-common-llm-vulnerabilities-remediation-6663df64d09c)
