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
# AI/ML/DL Learning Journey

A structured study plan covering mathematics, classical ML, deep learning, transformers/LLMs, and applied AI engineering. This repo tracks my progress, notes, and projects across each phase.

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
- *Mathematics for Machine Learning* — Deisenroth, Faisal, Ong (free at mml-book.github.io)
- Gilbert Strang — MIT 18.06 Linear Algebra
- Joe Blitzstein — Harvard Stat 110 (YouTube + free textbook)
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

- Andrew Ng — Machine Learning Specialization (Coursera, new version)
- *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* — Aurélien Géron (3rd ed., 2022)
- *An Introduction to Statistical Learning* — James, Witten, Hastie, Tibshirani (free PDF; ISLP for Python edition)
- Kaggle — Playground competitions

**Projects**

- End-to-end Kaggle competition

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

- **Andrej Karpathy — Neural Networks: Zero to Hero** (YouTube, karpathy.ai/zero-to-hero.html) — start here
- *Dive into Deep Learning* — d2l.ai (free, has PyTorch/JAX versions)
- fast.ai — Practical Deep Learning for Coders
- *Deep Learning* — Goodfellow, Bengio, Courville (2016, dated but still useful as a math reference)

**Projects**

- micrograd from scratch (Karpathy series)
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
- **Andrej Karpathy — "Let's build GPT from scratch"** + **karpathy/nanochat** (the successor to nanoGPT — full pipeline: tokenizer, pretraining, SFT, RL/GRPO, inference, web UI in ~8,000 lines)
- **Stanford CS336 — Language Modeling from Scratch** — Hashimoto, Liang (Spring 2025/2026 lectures on YouTube)
- *Build a Large Language Model (From Scratch)* — Sebastian Raschka (Manning, 2024) + github.com/rasbt/LLMs-from-scratch
- *Build a Reasoning Model (From Scratch)* — Sebastian Raschka (Manning) — for reasoning models, RL fine-tuning, inference-time techniques
- *Hands-On Large Language Models* — Jay Alammar & Maarten Grootendorst (O'Reilly, 2024)
- Lilian Weng — lilianweng.github.io

**Projects**

- BPE tokenizer from scratch
- nanochat reproduction & extension (full pipeline)
- Train a small GPT on a custom corpus

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
- Hugging Face Diffusion Models course (free)
- Hugging Face Audio course (free)

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

- *AI Engineering* — Chip Huyen (O'Reilly, 2025)
- *Designing Machine Learning Systems* — Chip Huyen
- Hugging Face NLP course
- Hugging Face Agents course (hf.co/learn/agents-course)
- DeepLearning.ai short courses (50+ available, many on agents/RAG)
- Hugging Face TRL — github.com/huggingface/trl — standard library for SFT/DPO/GRPO/PPO
- Eugene Yan — eugeneyan.com
- Hamel Husain — hamel.dev (especially his work on evals)

**Projects**

- RAG over a personal document collection with evals
- Fine-tuned 7B model with LoRA on a domain task
- Coding agent with tool use
- Production LLM feature in a real app

---

## Phase 7 — Specialized Depth (pick one)

- **NLP** — Stanford CS224N (Manning)
- **Computer Vision** — Stanford CS231N
- **Reinforcement Learning** — Sutton & Barto (2nd ed., 2018) + David Silver UCL lectures + OpenAI Spinning Up (spinningup.openai.com)
- **Graph Neural Networks** — Stanford CS224W
- **Mechanistic Interpretability & Alignment** — **ARENA curriculum** (arena.education, free, v6.0+ as of late 2025) — covers transformers, mech interp, RL, evals, alignment science. Also Neel Nanda's tutorials and Anthropic's transformer circuits work.

---

## Phase 8 — Distributed Training & Systems

**Topics**

- Data parallelism, FSDP
- Tensor, pipeline, sequence parallelism
- DeepSpeed, Megatron-LM
- Mixed precision training
- Gradient checkpointing
- Memory optimization

**Resources**

- Hugging Face's distributed training docs
- DeepSpeed and Megatron-LM tutorials
- *Hands-On Large Language Models* (covers some of this)

---

## Paper Reading List

**Foundational transformers & LLMs**

1. Attention Is All You Need — Vaswani et al. (2017)
2. BERT — Devlin et al. (2018)
3. GPT-2 — Radford et al. (2019)
4. GPT-3 — Brown et al. (2020)
5. Chinchilla scaling laws — Hoffmann et al. (2022)
6. InstructGPT / RLHF — Ouyang et al. (2022)
7. LoRA — Hu et al. (2021)
8. LLaMA / LLaMA-2 / LLaMA-3
9. DPO — Rafailov et al. (2023)
10. Mixtral / MoE
11. DeepSeek-V3 / DeepSeek-R1 (reasoning models)

**Generative & multimodal**

12. DDPM — Ho et al. (2020)
13. Latent Diffusion / Stable Diffusion — Rombach et al. (2022)
14. CLIP — Radford et al. (2021)

**Architecture alternatives**

15. Mamba / State Space Models — Gu, Dao
16. FlashAttention — Dao et al.

---

## Frontier Topics to Track

These move weekly. Track, don't try to master.

- Reasoning models & test-time compute (o-series, R-series, extended thinking)
- Agentic AI & long-horizon tool use
- Long-context architectures (1M+ tokens)
- MoE at scale
- State space models (Mamba)
- World models & video generation
- On-device inference & small capable models (1–8B)
- Synthetic data & self-improvement loops
- Mechanistic interpretability (sparse autoencoders, circuits)

---

## Karpathy Repos Worth Knowing

- **nanochat** — github.com/karpathy/nanochat — full ChatGPT-clone training pipeline for ~$100. The capstone reference repo.
- **nn-zero-to-hero** — github.com/karpathy/nn-zero-to-hero — notebooks for the YouTube series
- **llm.c** — github.com/karpathy/llm.c — LLM training in raw C/CUDA, useful for understanding the low level
- **autoresearch** — github.com/karpathy/autoresearch — agent-based autonomous LLM research (March 2026)
- **micrograd** — github.com/karpathy/micrograd — tiny autograd engine (built in the YouTube series)
- **LLM101n** (upcoming) — Karpathy's full LLM course at Eureka Labs, his AI-native education company. Track for release.

---

## Newsletters

- **Import AI** — Jack Clark (weekly, broad coverage)
- **The Batch** — Andrew Ng / DeepLearning.ai
- **Interconnects** — Nathan Lambert (best on post-training and RLHF)
- **Ahead of AI** — Sebastian Raschka (technical paper breakdowns)
- **AlphaSignal** — daily, fast but high-noise

---

## Sources to Track

- **arxiv-sanity** (cs.LG, cs.CL, cs.CV)
- **Hugging Face papers** — huggingface.co/papers (trending)
- **Papers with Code**
- **GitHub trending** (machine-learning, llm topics)

---

## Conferences

- **NeurIPS, ICML, ICLR** — general ML
- **ACL, EMNLP** — NLP
- **CVPR, ICCV** — vision
- **COLM** — language models specifically (newer, very relevant)

---

## Twitter/X Accounts to Follow

- Andrej Karpathy
- Yann LeCun
- Sebastian Raschka
- Lilian Weng
- Jim Fan
- Nathan Lambert
- Jason Wei
- Authors of papers you respect

---

## Libraries & Tools to Get Hands-On With

- **PyTorch** — primary deep learning framework
- **Hugging Face Transformers, Datasets, Tokenizers** — the standard stack
- **Hugging Face TRL** — SFT, DPO, GRPO, PPO
- **Hugging Face Accelerate** / **DeepSpeed** — distributed training
- **vLLM, SGLang** — production inference
- **LangGraph** (or plain Python) — agent orchestration
- **Weights & Biases** or **MLflow** — experiment tracking
- **PEFT** — parameter-efficient fine-tuning (LoRA, QLoRA)

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

## Paper Log

| Paper | Date Read | Notes |
|-------|-----------|-------|
| | | |

## Project Log

| Project | Started | Completed | Phase | Repo |
|---------|---------|-----------|-------|------|
| | | | | |
