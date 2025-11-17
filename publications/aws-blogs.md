---
layout: default
title: AWS Blog Posts
---

# AWS Blog Posts

## Published Articles

### Increase ML Model Performance and Reduce Training Time Using Amazon SageMaker Built-in Algorithms with Pre-trained Models

**Published:** October 6, 2022
**Co-authors:** Vedant Jain and Ari Bajo Rouvinen
**Platform:** AWS Machine Learning Blog

**Summary:**

This blog post demonstrates how to leverage transfer learning with Amazon SageMaker's built-in algorithms to significantly improve model performance and reduce training time. The article focuses on using pre-trained models as a starting point for custom machine learning tasks.

**Key Topics Covered:**

- **Transfer Learning Benefits:**
  - Reduced training time by starting with pre-trained weights
  - Improved model performance, especially with limited training data
  - Lower computational costs compared to training from scratch

- **SageMaker Built-in Algorithms:**
  - Image Classification algorithm with pre-trained models
  - Object Detection algorithm with transfer learning capabilities
  - Semantic Segmentation with pre-trained backbones

- **Implementation Guide:**
  - How to specify pre-trained models in SageMaker training jobs
  - Hyperparameter configuration for transfer learning
  - Fine-tuning strategies for different use cases

- **Performance Benchmarks:**
  - Comparison of training times: pre-trained vs. from-scratch
  - Accuracy improvements with transfer learning
  - Cost analysis and optimization strategies

**Technical Highlights:**

- Using `use_pretrained_model` parameter in SageMaker algorithms
- Selecting appropriate pre-trained backbones (ResNet, VGG, MobileNet)
- Fine-tuning strategies: feature extraction vs. full fine-tuning
- Best practices for dataset preparation and augmentation

**Use Cases:**

- Custom image classification with limited labeled data
- Object detection for domain-specific applications
- Semantic segmentation for medical imaging and autonomous vehicles

**Impact:**

This approach enables data scientists and ML engineers to:
- Achieve production-ready models faster
- Reduce infrastructure costs by 40-60%
- Improve model accuracy by 10-15% on small datasets
- Democratize ML by lowering the barrier to entry

**Read the full article:** [AWS Machine Learning Blog](https://aws.amazon.com/blogs/machine-learning/increase-ml-model-performance-and-reduce-training-time-using-amazon-sagemaker-built-in-algorithms-with-pre-trained-models/)

---

## Additional AWS Contributions

*More blog posts and technical articles coming soon...*

---

[← Back to Publications](../index.html#publications--talks)

