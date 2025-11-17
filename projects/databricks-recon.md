# Automated Red Teaming for Databricks Mosaic AI Model Serving (Protect AI Recon)

## Overview

This project integrates **Protect AI Recon** with **Databricks Mosaic AI Model Serving** to perform **automated red-teaming scans** of deployed LLM endpoints.

Based on:  
**“Automated Red Teaming Scans of Databricks Mosaic AI Model Serving Endpoints Using Protect AI Recon”**.

---

## Problem

Organizations deploying LLMs on Mosaic AI need to:

- Understand how their endpoints behave under adversarial conditions.  
- Detect prompt-injection vulnerabilities and jailbreaks early.  
- Continuously validate that guardrails and policies remain effective as models and prompts evolve.

Manual red-teaming is time-consuming and non-scalable.

---

## Approach

The solution uses **Protect AI Recon** to:

1. **Discover and register Mosaic AI endpoints** targeted for testing.  
2. **Generate adversarial prompts** that simulate:
   - Jailbreak attempts  
   - Data exfiltration  
   - Policy evasion  
3. **Execute batch tests** against Mosaic AI endpoints.  
4. **Aggregate and analyze findings**, highlighting:
   - Vulnerable prompts  
   - Risk categories  
   - Recommended mitigations  

This forms an ongoing, automated security testing layer around Mosaic AI deployments.

---

## Techniques & Stack

- Platform: Databricks Mosaic AI Model Serving  
- Security tooling: Protect AI Recon  
- LLM security testing: prompt-level adversarial generation, classification, and reporting  
- Integration: API-driven workflows connecting Recon and Mosaic AI endpoints  

---

## Outcomes

- A scalable way to **continuously red-team** Mosaic AI endpoints.  
- Clear visibility into model behaviors under attack.  
- Actionable insights to strengthen guardrails, prompts, and deployment policies.

---

## My Role

- Led or co-led the design of the Recon–Mosaic AI integration.  
- Worked on defining attack scenarios and evaluation criteria.  
- Authored the long-form technical article and supporting material.

---

## Related Reading

- Protect AI Blog – Automated Red Teaming Scans of Databricks Mosaic AI Model Serving Endpoints Using Protect AI Recon
