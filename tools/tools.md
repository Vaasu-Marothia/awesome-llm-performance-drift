# Tools and Evaluation Frameworks for LLM Drift & Alignment

This document details key open-source software libraries, CI/CD evaluation harnesses, and diagnostic suites used to measure model degradation, catastrophic forgetting, and output stability.

---

### 1. FastChat (LLM-as-a-Judge Pipeline)
* **Purpose:** Provides the core evaluation infrastructure for pairwise LLM judging and MT-Bench scoring. Implements position-swapping, rubric generation, and multi-turn automated grading to detect subtle behavioral regressions in conversational models.
* **Key Capabilities:**
  * Automated execution of multi-turn benchmarks.
  * Mitigation of judge biases (position, verbosity, self-enhancement).
* **Official Link:** [https://github.com/lm-sys/FastChat](https://github.com/lm-sys/FastChat)

---

### 2. LM-Evaluation-Harness
* **Purpose:** The industry standard framework developed by EleutherAI for zero-shot and few-shot evaluation of language models across hundreds of standard tasks.
* **Key Capabilities:**
  * Reproducible evaluation of open-weight models (Hugging Face, vLLM).
  * Detection of performance regressions across checkpoints during continual fine-tuning.
* **Official Link:** [https://github.com/EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness)

---

### 3. DeepEval
* **Purpose:** An open-source, production-ready unit testing and continuous integration (CI/CD) framework for LLM applications.
* **Key Capabilities:**
  * Tracks hallucination rates, answer relevancy, and G-Eval custom metrics on every PR or API version change.
  * Integrates regression alerts to prevent deploying drifted prompts or updated base models.
* **Official Link:** [https://github.com/confident-ai/deepeval](https://github.com/confident-ai/deepeval)

---

### 4. Inspect Evals
* **Purpose:** A standardized evaluation framework developed by the UK AI Safety Institute (UK AISI) for assessing LLM capabilities and safety risks.
* **Key Capabilities:**
  * Native execution engines for dynamic benchmarks including LiveBench and SWE-bench.
  * Granular logging and diagnostic toolchains for analyzing edge-case logic failures and exception chain collapse.
* **Official Link:** [https://github.com/UKGovernmentBEIS/inspect_evals](https://github.com/UKGovernmentBEIS/inspect_evals)

---

### 5. Ragas (Retrieval Augmented Generation Assessment)
* **Purpose:** A framework specifically designed to evaluate and monitor performance drift in RAG pipelines and multi-hop knowledge retrieval systems.
* **Key Capabilities:**
  * Computes faithfulness, context recall, and semantic similarity over time.
  * Isolates whether regressions stem from LLM output drift or underlying vector embedding changes.
* **Official Link:** [https://github.com/explodinggradients/ragas](https://github.com/explodinggradients/ragas)
