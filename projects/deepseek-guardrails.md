# Building Guardrails for DeepSeek-R1 on Amazon Bedrock

## Overview

This project focuses on designing and implementing **LLM guardrails** for **DeepSeek-R1** hosted on **Amazon Bedrock**, using Protect AI capabilities to harden model behavior in production scenarios.

It is based on the work described in:  
**“Building Robust LLM Guardrails for DeepSeek-R1 in Amazon Bedrock”** (Protect AI).

---

## Problem

Enterprises adopting DeepSeek-R1 on Bedrock need to:

- Control unsafe, non-compliant, or high-risk outputs.  
- Reduce exposure to **prompt-injection**, **jailbreak attempts**, and **sensitive data leakage**.  
- Embed security and governance into their model deployment patterns.

---

## Approach & Architecture

The solution integrates:

1. **Amazon Bedrock with DeepSeek-R1**  
   - Provides managed model hosting and scaling.

2. **Protect AI Guardrails / Recon**  
   - Used to design and test adversarial prompts.  
   - Runs automated red-teaming workflows against Bedrock endpoints.

3. **Guardrail Policy Layer**  
   - A layer of routing and validation that:
     - Filters or modifies high-risk prompts.  
     - Checks responses for policy violations.  
     - Applies safe defaults or fallback behaviors.

4. **Monitoring & Feedback Loop**  
   - Logs prompts, responses, and guardrail decisions.  
   - Feeds back into test suites and continuous hardening activities.

---

## Techniques

- Prompt-injection detection patterns  
- Output classification and filtering  
- Policy-driven response rewriting or blocking  
- Automated red-teaming using generated adversarial prompts  
- Integration with Bedrock APIs and security best practices  

---

## Outcomes

- A repeatable approach to deploying DeepSeek-R1 in **highly regulated or risk-sensitive** environments.  
- Stronger protection against common LLM failure modes.  
- A living test suite and feedback loop for continuous improvement.

---

## My Role

- Co-designed the architecture integrating Bedrock, DeepSeek-R1, and Protect AI.  
- Contributed to threat modeling and guardrail strategy.  
- Authored or co-authored the associated technical write-up and demo content.

---

## Related Links

- YouTube:  
  - https://www.youtube.com/watch?v=fqFyJoPrLcU  
  - https://www.youtube.com/watch?v=6AZB2V13SJ4  

- AWS APN Blog:  
  - https://aws.amazon.com/blogs/apn/protect-deepseek-model-deployments-with-protect-ai-and-amazon-bedrock/
