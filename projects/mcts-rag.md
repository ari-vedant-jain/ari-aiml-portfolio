# Improving RAG Answer Quality with Monte Carlo Tree Search (MCTS)

## Overview

This project investigates using **Monte Carlo Tree Search (MCTS)** to improve answer quality in RAG pipelines by exploring and ranking multiple candidate responses instead of relying on a single forward pass.

Based on my article  
**“Improving Text Quality with Monte Carlo Tree Search (MCTS) in Retrieval Augmented Generation”**.

---

## Problem

Standard RAG implementations typically:

- Generate a single answer given a prompt and context.  
- Do not explicitly explore alternative reasoning paths or candidates.  
- Lack a principled mechanism for **searching** the space of possible responses.

The goal was to introduce a **search-based optimization layer** over the LLM outputs.

---

## Approach

MCTS is used as a controller over the LLM:

1. **Node Representation**  
   - Nodes represent partial or complete candidate responses, or different reasoning paths.

2. **Expansion**  
   - From a given state, the LLM is prompted to extend or propose a variant of the answer.

3. **Simulation**  
   - A simulation step evaluates a completed answer using heuristics such as:
     - Alignment with retrieved context  
     - Semantic similarity to relevant documents  
     - Specific task-oriented quality metrics

4. **Backpropagation**  
   - Quality scores are propagated back up the tree to guide exploration.

The result is a set of candidate answers with associated scores, from which the best (or a small set) is selected.

---

## Techniques & Stack

- **Search algorithm:** Monte Carlo Tree Search  
- **LLM:** any model capable of generating candidate continuations  
- **RAG:** retrieval as a fixed context provider to ground generation  
- **Evaluation heuristics:** semantic similarity, task-specific scoring, or learned reward models  

Typical implementation would use:

- Python  
- An LLM API or local LLM  
- Vector store for retrieval  
- Custom MCTS loop implementation  

---

## Outcomes

- More robust and diverse candidate answers for complex queries.  
- A structured way to trade off **exploration** (trying new candidates) vs **exploitation** (focusing on promising answers).  
- A foundation for integrating **learned reward models** and **reinforcement-style optimization** into RAG.

---

## My Role

- Proposed applying MCTS to RAG answer generation and selection.  
- Designed the conceptual architecture and evaluation framework.  
- Authored the technical article and example patterns.

---

## Related Reading

- [Improving Text Quality with MCTS in RAG](https://medium.com/@ari_in_media_res/improving-text-quality-with-monte-carlo-tree-search-mcts-in-retrieval-augmented-generation-59e9c14cda4a)
