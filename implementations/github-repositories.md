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

### 4. WildBench Evaluation Harness
* **Repository:** [allenai/WildBench](https://github.com/allenai/WildBench)
* **What It Implements:** Benchmark suite and evaluation runners for testing models against in-the-wild user interactions collected from real-world usage[cite: 1].
* **Relevance:** Automates continuous capability testing and fine-grained pairwise scoring (WB-Reward, WB-Score) to detect alignment drift without risk of static benchmark contamination[cite: 1].

---

### 5. IFEval (Instruction-Following Evaluation Framework)
* **Repository:** [google-research/instruction_following_eval](https://github.com/google-research/google-research/tree/master/instruction_following_eval)
* **What It Implements:** Ground-truth verifiers for testing strict formatting and lexical constraint adherence[cite: 1].
* **Relevance:** Enables automated detection of syntactic drift, conversational bloat, and formatting failure modes caused by continuous safety and RLHF post-training[cite: 1].
