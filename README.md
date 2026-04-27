# learn-ai
Learning AI from scratch

# AI/ML/DL Learning Journey

A structured study plan covering mathematics, classical ML, deep learning, and modern AI engineering. This repo tracks my progress, notes, and projects across each phase.

## Timeline

~10–12 months at 15–20 hrs/week, then continuous.

## Structure

- `phase-XX-topic/` — notes, code, and exercises for each phase
- `papers/` — paper reading notes
- `projects/` — end-to-end builds

---

## Phase 1 — Mathematics & Tensor Fluency

**Topics**

- Linear Algebra: vectors, matrices, rank, eigendecomposition, SVD, matrix calculus
- Calculus: partial derivatives, gradients, Jacobians, chain rule
- Probability & Statistics: distributions, Bayes' theorem, MLE, MAP, sampling
- Optimization: gradient descent, SGD, Adam, AdamW, learning rate schedules
- Information Theory: entropy, cross-entropy, KL divergence
- NumPy / PyTorch tensors: broadcasting, indexing, vectorization

**Resources**

- 3Blue1Brown — Essence of Linear Algebra
- 3Blue1Brown — Essence of Calculus
- *Mathematics for Machine Learning* — Deisenroth, Faisal, Ong (free PDF)
- Gilbert Strang — MIT 18.06 Linear Algebra
- Joe Blitzstein — Harvard Stat 110
- Sebastian Ruder — "An overview of gradient descent optimization algorithms"
- NumPy 100 exercises — github.com/rougier/numpy-100

---

## Phase 2 — Classical Machine Learning

**Topics**

- Linear & logistic regression
- Decision trees, random forests
- Gradient boosting: XGBoost, LightGBM, CatBoost
- SVMs, kernel methods
- K-Means, DBSCAN, hierarchical clustering
- PCA, t-SNE, UMAP
- Bias–variance tradeoff
- Cross-validation, regularization (L1/L2)
- Feature engineering, missing data, class imbalance, leakage
- Evaluation: precision/recall, ROC-AUC, calibration

**Resources**

- Andrew Ng — Machine Learning Specialization (Coursera)
- *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* — Aurélien Géron
- *An Introduction to Statistical Learning* — James, Witten, Hastie, Tibshirani (free PDF)
- Kaggle — Playground competitions

---

## Phase 3 — Deep Learning Core

**Topics**

- MLPs, universal approximation
- Activations: ReLU, GELU, SiLU, softmax
- Backpropagation (derivation + from-scratch implementation)
- Loss functions
- Optimizers: AdamW, schedulers (cosine, warmup)
- Regularization: dropout, weight decay, augmentation, early stopping
- Normalization: BatchNorm, LayerNorm, RMSNorm
- Initialization: Xavier, Kaiming
- CNNs: convolutions, pooling, ResNet
- RNNs, LSTMs, GRUs

**Resources**

- Andrej Karpathy — Neural Networks: Zero to Hero (YouTube)
- *Dive into Deep Learning* — d2l.ai (free)
- fast.ai — Practical Deep Learning for Coders
- *Deep Learning* — Goodfellow, Bengio, Courville (reference)

**Projects**

- MLP from scratch in NumPy on MNIST
- CNN on CIFAR-10 in PyTorch
- ResNet-18 reproduction

---

## Phase 4 — Transformers & LLMs

**Topics**

- Self-attention, multi-head attention
- Positional encodings: sinusoidal, RoPE, ALiBi
- Encoder, decoder, encoder-decoder architectures
- BERT, GPT, T5
- Tokenization: BPE, SentencePiece, tiktoken
- Pretraining objectives, scaling laws
- Instruction tuning / SFT
- RLHF, DPO, GRPO
- LoRA, QLoRA, adapters
- Quantization: int8, int4, GPTQ, AWQ
- Mixture of Experts
- KV cache, FlashAttention, speculative decoding
- Long-context techniques

**Resources**

- *Attention Is All You Need* — Vaswani et al. (2017)
- The Illustrated Transformer — Jay Alammar
- The Annotated Transformer — Harvard NLP
- Andrej Karpathy — Let's build GPT + nanoGPT
- Stanford CS336 — Language Modeling from Scratch
- *Build a Large Language Model (From Scratch)* — Sebastian Raschka
- Lilian Weng — lilianweng.github.io

**Projects**

- BPE tokenizer from scratch
- nanoGPT reproduction & extension
- Character-level GPT trained on custom corpus

---

## Phase 5 — Generative & Multimodal

**Topics**

- VAEs
- GANs
- Diffusion: DDPM, score-based, classifier-free guidance, latent diffusion
- Flow matching / rectified flow
- CLIP & contrastive learning
- Vision-Language Models: LLaVA, Qwen-VL
- Whisper / audio models
- Video generation

**Resources**

- Lilian Weng — diffusion explainers
- *The Annotated Diffusion Model* — Hugging Face
- Hugging Face Diffusion Models course

---

## Phase 6 — Applied AI Engineering

**Topics**

- RAG: chunking, embeddings, hybrid retrieval, rerankers, evals
- Vector DBs: pgvector, Qdrant, Weaviate, LanceDB
- Agents: ReAct, function calling, tool use, planning, memory
- Fine-tuning: LoRA, QLoRA, synthetic data
- Inference engines: vLLM, SGLang, TensorRT-LLM
- Evaluation: lm-eval-harness, ragas, custom evals
- Observability: Langfuse, Helicone
- MLOps: Docker, model versioning, CI for prompts

**Resources**

- Hugging Face NLP, Audio, Diffusion courses
- DeepLearning.ai short courses
- *AI Engineering* — Chip Huyen
- Eugene Yan — eugeneyan.com
- Hamel Husain — hamel.dev

**Projects**

- RAG over a personal document collection with evals
- Fine-tuned 7B model with LoRA on a domain task
- Coding agent with tool use
- Production LLM feature in a real app

---

## Phase 7 — Specialized Depth (pick one)

- **NLP** — Stanford CS224N
- **Computer Vision** — Stanford CS231N
- **Reinforcement Learning** — Sutton & Barto + David Silver UCL lectures + OpenAI Spinning Up
- **Graph Neural Networks** — Stanford CS224W
- **Mechanistic Interpretability** — Neel Nanda's tutorials, Anthropic circuits

---

## Phase 8 — Distributed Training & Systems

**Topics**

- Data parallelism, FSDP
- Tensor, pipeline, sequence parallelism
- DeepSpeed, Megatron-LM
- Mixed precision training
- Gradient checkpointing
- Memory optimization

---

## Paper Reading List

1. Attention Is All You Need — Vaswani et al. (2017)
2. BERT — Devlin et al. (2018)
3. GPT-2 — Radford et al. (2019)
4. GPT-3 — Brown et al. (2020)
5. Chinchilla — Hoffmann et al. (2022)
6. InstructGPT — Ouyang et al. (2022)
7. LoRA — Hu et al. (2021)
8. LLaMA / LLaMA-2 / LLaMA-3
9. DPO — Rafailov et al. (2023)
10. Mixtral
11. DeepSeek-V3 / DeepSeek-R1
12. Mamba — Gu, Dao
13. DDPM — Ho et al. (2020)
14. Stable Diffusion / Latent Diffusion — Rombach et al. (2022)
15. CLIP — Radford et al. (2021)

---

## Frontier Topics (track, don't try to master)

- Reasoning models & test-time compute
- Agentic AI & long-horizon tool use
- Long-context architectures
- MoE at scale
- State space models (Mamba)
- World models & video generation
- On-device inference & small capable models
- Synthetic data & self-improvement
- Mechanistic interpretability

---

## Staying Current

**Newsletters**

- Import AI — Jack Clark
- The Batch — Andrew Ng
- AlphaSignal
- Interconnects — Nathan Lambert
- Ahead of AI — Sebastian Raschka

**Sources**

- arxiv-sanity (cs.LG, cs.CL, cs.CV)
- Hugging Face papers
- Papers with Code
- GitHub trending

**Conferences**

- NeurIPS, ICML, ICLR
- ACL, EMNLP
- CVPR, ICCV
- COLM

---

## Progress Log

| Phase | Started | Completed | Notes |
|-------|---------|-----------|-------|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |
| 5 | | | |
| 6 | | | |
| 7 | | | |
| 8 | | | |
