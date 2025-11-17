# Graph Neural Network Fraud Detection with Amazon SageMaker

## Overview

This project applies **Graph Neural Networks (GNNs)** to detect fraudulent financial transactions using **Amazon SageMaker**.

Based on the AWS blog:  
**“Detect financial transaction fraud using a Graph Neural Network with Amazon SageMaker”**.

---

## Problem

Traditional fraud detection models often rely on:

- Tabular features only  
- Per-transaction evaluation  
- Limited modeling of relationships between entities

Fraud is inherently **graph-structured**, involving relationships between accounts, devices, merchants, IP addresses, and more.

---

## Approach

The solution:

1. **Builds a transaction graph** where:
   - Nodes represent entities (accounts, cards, devices, etc.)  
   - Edges represent interactions or transactions  

2. **Trains a GNN model** (e.g., GraphSAGE, GAT) to learn node or edge embeddings that capture relational patterns.

3. **Classifies transactions or entities** as fraudulent vs legitimate using downstream classifiers.

4. Uses **Amazon SageMaker** to:
   - Prepare and process graph data  
   - Train the GNN at scale  
   - Deploy the model as an endpoint  

---

## Techniques & Stack

- **Graph ML:** GNNs (GraphSAGE, GAT, or similar)  
- **ML Frameworks:** DGL or PyTorch Geometric (depending on implementation)  
- **Platform:** Amazon SageMaker for:
  - Training  
  - Hyperparameter tuning  
  - Model hosting  

---

## Outcomes

- Improved ability to capture complex fraud patterns that tabular methods can miss.  
- A scalable pipeline for training and deploying GNN models on AWS.

---

## My Role

- Co-authored the blog and solution patterns.  
- Contributed to architecture, data pipelines, and explanation of the fraud detection workflow.

---

## Related Reading

- “Detect financial transaction fraud using a Graph Neural Network with Amazon SageMaker”
