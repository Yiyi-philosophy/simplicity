---
title: 'QuadraLib: A Performant Quadratic Neural Network Library For Architecture Optimization And Design Exploration'
image: 'Summarize.assets/image (6).png'
---

<!--more-->


## Abstract

- DNNs' success depends on many supporting libraries.

- QDNNs ($(WX)^2+b$) show better **non-linearity** and **learning capability**

- In this paper, author proposed a new QDNN neuron architecture design, and further developed QuadraLib. 

- **good accuracy** and computation consumption

## 1 Introduction

- the benefits of QDNNs stem from the unique characteristics of the second-order polynomial form: 

  - (1) **stronger non-linearity**, hence improved capability for feature extraction

  - (2) **higher model efficiency** as QDNN can approximate polynomial decision boundaries using smaller network depth/width

- Contribution

  - four types of QDNN

  - new quadratic neuron architecture

  - QuadraLib

  - experiment

## 2 DRAWBACKS OF THE EXISTING QDNN NEURON ARCHITECTURE DESIGN

- P1 Approximation Capability Issue:

- P2 Computation Complexity Issue:

- P3 Converge Performance Issue:

  - second-order term in QDNNs will introduce critical gradient vanishing issue

- P4 Implementation Feasibility Issue:

  - need to rewrite the entire convolution operation to add extra multiplication between W and the second X.

- P5 Structure Design Issue:

- P6 Memory Usage Issue:

## 3 QDNN NEURON ARCHITECTURE OPTIMIZATION

  - 3.1 New Neuron Architecture Design

    <img src="../images/Summarize.assets/image (5).png" alt="image (5)" width="50%" />

    - introduce extra trainable parameters on the second-order term

    - other term to prevent the gradient vanishing

    - Hardmard product

    - easily assembled

  - 3.2 Theoretical Performance Analysis

    - Extra Weights and Linear Term for Approximation Capa-
  bility (P1) Improvement:

    - Hadamard Product for Computation Complexity (P2) Optimization:

    - Linear Term for Converge Performance ( P3 ) Enhancement

    - First-order Neuron Combination for Implementation Feasibility ( P4 ) Improvement

## 4 QUADRALIB FOR QDNN DESIGN EXPLORATION

  <img src="../images/Summarize.assets/image (6).png" alt="image (6)" width="100%" />

- In **Model** Level, QuadraLib defines a set of encapsulated layer modules

  - auto-builder for converting first-order model to a corresponding QDNN version

- In **Training**/Inference Level, QuadraLib leverages a memory profiler to monitor the memory cost of the generated QDNN model 

- In **Application** Level, QuadraLib also provides model analysis tools such as activation and weight/gradient distribution **visualization**.

- 4.3 QuadraLib Training Optimization

  - Hybrid Back-propagation for Memory Efficiency

  <img src="../images/Summarize.assets/image (7).png" alt="image (7)" width="50%" />
  
  - Quadratic Optimizer Implementation
      
## 6 CONCLUSION AND DISCUSSION

- QDNNs show a significant potential on learning tasks which highly depends on **extracted objects,** such as object detection, segmentation, and position recognition.

- the recognition process will more focus on the important objects while ignoring the unimportant background
