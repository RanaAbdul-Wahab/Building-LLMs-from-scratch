# Building-LLMs-from-scratch

A complete implementation of Large Language Model (LLM) fundamentals from scratch using Python. This repository is a hands-on journey through the core building blocks of modern language models, starting from tokenization and embeddings all the way to constructing a GPT-style architecture and text generation pipeline.

## Project Overview

This project is divided into three phases, each focusing on a critical component of LLM development.

The goal is to understand how modern language models work under the hood by implementing every major component from scratch instead of relying on high-level deep learning libraries or pre-built transformer architectures.

---

# Phase 1: Data Preprocessing Pipeline

This phase focuses on transforming raw text into numerical representations that can be processed by neural networks.

### Implemented Components

#### 1. LLM Tokenizer
- Built a custom tokenizer from scratch
- Converts raw text into tokens
- Handles vocabulary creation and token mapping

#### 2. GPT Tokenizer
- Implemented a GPT-style tokenization pipeline
- Demonstrated how modern LLMs tokenize text efficiently

#### 3. Byte Pair Encoding (BPE)
- Implemented the Byte Pair Encoding algorithm from scratch
- Learned subword vocabulary generation
- Reduced vocabulary size while preserving language structure

#### 4. Token Embeddings
- Created trainable token embeddings
- Converted token IDs into dense vector representations
- Prepared inputs for transformer-based architectures

#### 5. Positional Embeddings
- Implemented positional encoding mechanisms
- Preserved word order information within sequences
- Combined positional and token embeddings for transformer input

---

# Phase 2: Attention Mechanisms

This phase focuses on the core innovation behind Transformer architectures: the Attention Mechanism.

### Implemented Components

#### 1. Self-Attention Mechanism
- Built self-attention from scratch
- Computed Query, Key, and Value matrices
- Generated contextual token representations

#### 2. Causal Attention Mechanism
- Implemented masked attention
- Prevented tokens from accessing future information
- Enabled autoregressive text generation

#### 3. Multi-Head Attention
- Implemented multiple attention heads
- Learned different contextual relationships simultaneously
- Combined outputs into a unified representation

### Key Concepts Covered

- Query-Key-Value computation
- Attention score calculation
- Scaled dot-product attention
- Attention masking
- Multi-head parallel processing
- Context vector generation

---

# Phase 3: Building an LLM Architecture

This phase combines all previous components into a complete GPT-style language model.

### Implemented Components

#### 1. Layer Normalization
- Implemented normalization layers from scratch
- Stabilized training dynamics
- Improved gradient flow

#### 2. GELU Activation Function
- Implemented Gaussian Error Linear Unit (GELU)
- Used as the primary activation function
- Replicated transformer architecture behavior

#### 3. Complete Transformer Block
- Integrated:
  - Multi-head attention
  - Feed-forward network
  - Residual connections
  - Layer normalization

#### 4. Full LLM Architecture
- Constructed an end-to-end GPT-style architecture
- Connected embeddings, attention blocks, and output layers
- Implemented forward propagation logic

#### 5. Loss Function
- Implemented language modeling loss computation
- Used cross-entropy loss for next-token prediction

#### 6. Temperature Scaling
- Experimented with different temperature values
- Controlled output randomness during generation
- Studied the impact on generated text quality

#### 7. Top-K Sampling
- Implemented Top-K token selection
- Reduced low-probability token noise
- Improved generation coherence

#### 8. Text Generation Pipeline
- Generated text autoregressively
- Combined temperature scaling and Top-K sampling
- Demonstrated inference workflow

#### 9. Model Checkpointing
- Saved trained model weights
- Loaded model checkpoints
- Enabled model reuse without retraining

---

# Technologies Used

- Python
- NumPy
- PyTorch

---

# Learning Outcomes

By completing this project, the following concepts were implemented and understood from first principles:

- Tokenization
- Byte Pair Encoding (BPE)
- Embeddings
- Positional Encoding
- Self-Attention
- Causal Attention
- Multi-Head Attention
- Transformer Blocks
- Layer Normalization
- GELU Activation
- Language Modeling Loss
- Temperature Scaling
- Top-K Sampling
- GPT-Style Architecture
- Model Saving and Loading

---

# Repository Structure

```text
Building-LLMs-From-Scratch/
│
├── Phase-1-Data-Preprocessing/
│   ├── LLM Tokenizer
│   ├── GPT Tokenizer
│   ├── Byte Pair Encoding
│   ├── Token Embeddings
│   └── Positional Embeddings
│
├── Phase-2-Attention-Mechanisms/
│   ├── Self Attention
│   ├── Causal Attention
│   └── Multi-Head Attention
│
├── Phase-3-LLM-Architecture/
│   ├── Layer Normalization
│   ├── GELU Activation
│   ├── Transformer Block
│   ├── Full LLM Architecture
│   ├── Loss Function
│   ├── Temperature Scaling
│   ├── Top-K Sampling
│   └── Model Saving & Loading
│
└── README.md
```

---

# Key Objective

The primary objective of this repository is not merely to use Large Language Models but to understand and implement every fundamental building block behind modern GPT-style architectures from scratch.

This project serves as a practical deep dive into how state-of-the-art language models work internally, bridging the gap between theoretical concepts and real-world implementation.  
