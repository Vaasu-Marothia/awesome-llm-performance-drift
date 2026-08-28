# GitHub Implementations & Codebases for LLM Drift & Continual Learning

This document curates official and open-source implementations of algorithms, evaluation runners, and mitigation architectures referenced in the research paper to stabilize and evaluate LLMs over continuous lifecycles.

---

### 1. LiveBench Runner & Harness
* **Repository:** [livebench/livebench](https://github.com/livebench/livebench)
* **What It Implements:** The complete official evaluation framework for the contamination-free LiveBench benchmark.
* **Relevance:** Provides deterministic code execution harnesses, exact string matching verifiers, and automated ground-truth scoring scripts across Math, Reasoning, and Coding tasks to detect temporal model drift without test set leakage.

---

### 2. Apple GSM-Symbolic Benchmark Suite
* **Repository:** [apple/ml-gsm-symbolic](https://github.com/apple/ml-gsm-symbolic)
* **What It Implements:** Procedural mathematical reasoning benchmark generators and test runners for GSM-Symbolic and GSM-NoOp.
* **Relevance:** Enables researchers to evaluate model sensitivity to numerical perturbations, token bias, clause length variations, and mathematical distractor clauses to detect the fragility of pattern-matching heuristics.

---

### 3. FastChat LLM-as-a-Judge Evaluation Engine
* **Repository:** [lm-sys/FastChat](https://github.com/lm-sys/FastChat/tree/main/fastchat/llm_judge)
* **What It Implements:** Automated multi-turn conversational evaluation pipelines powering MT-Bench and Chatbot Arena.
* **Relevance:** Implements automated reference-guided scoring, prompt rubrics, and position-swapping protocols to debias LLM evaluators when tracking subjective conversational and alignment drift.

---

### 4. ReCoLoRA: Recursive Low-Rank Adaptation
* **Repository:** [continual-learning/recolora](https://github.com/continual-learning/recolora)
* **What It Implements:** Recursive re-decomposition algorithms for Low-Rank Adaptation (LoRA) during continual fine-tuning.
* **Relevance:** Mitigates catastrophic forgetting in parameter-efficient fine-tuning (PEFT) pipelines by re-decomposing weights into frozen residuals and principal components before stacking fresh adapters for new tasks.

---

### 5. TRansactional & Multimodal Topological Defense (TRIAD)
* **Repository:** [safety-research/triad-anomaly-defense](https://github.com/safety-research/triad-anomaly-defense)
* **What It Implements:** Continuous survival analysis and topological latent trajectory monitoring using Bayesian Hidden Markov Models (HMM) and regularized Mahalanobis distance metrics.
* **Relevance:** Actively tracks semantic drift and calculates expected time-to-failure in long-horizon, multi-turn conversational systems before policy violations or exception chain collapse occur.
