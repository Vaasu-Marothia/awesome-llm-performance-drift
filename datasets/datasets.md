# Benchmark Datasets for LLM Performance Drift & Evaluation

This document curates standard and dynamic benchmark datasets used to detect performance drift, catastrophic forgetting, reasoning degradation, and alignment shifts across Large Language Model updates.

---

### 1. LiveBench
* **Source:** [LiveBench Official Platform](https://livebench.ai/) | [arXiv:2406.19314](https://arxiv.org/abs/2406.19314)
* **Description:** A contamination-free, dynamically refreshed benchmark suite. Tasks are procedurally generated from recently published arXiv preprints, math competitions, news, and Kaggle datasets on a 6-month cycle with monthly delayed releases.
* **Primary Application:** Continuous longitudinal tracking of LLMs in Mathematics, Coding, Reasoning, Data Analysis, Language Comprehension, and Instruction Following using verifiable objective ground-truth scoring.
* **Access Link:** [https://github.com/livebench/livebench](https://github.com/livebench/livebench)

---

### 2. GSM-Symbolic & GSM-NoOp
* **Source:** [Apple ML Research](https://github.com/apple/ml-gsm-symbolic) | [arXiv:2410.05229](https://arxiv.org/abs/2410.05229)
* **Description:** A procedural dataset derived from Grade School Math (GSM8K) containing 100 symbolic templates with dynamically generated variants (names, values, clauses). It includes the **GSM-NoOp** split, which injects mathematically irrelevant distractor clauses to stress-test pattern-matching heuristics vs. true reasoning.
* **Primary Application:** Quantifying the fragility of mathematical reasoning, token sensitivity, and logic degradation across fine-tuning iterations.
* **Access Link:** [https://huggingface.co/datasets/apple/GSM-Symbolic](https://huggingface.co/datasets/apple/GSM-Symbolic)

---

### 3. MT-Bench (Multi-Turn Benchmark)
* **Source:** [LMSYS Org](https://github.com/lm-sys/FastChat) | [arXiv:2306.05685](https://arxiv.org/abs/2306.05685)
* **Description:** A curated set of 80 high-quality, multi-turn dialogue questions spanning 8 core domains: Writing, Roleplay, Extraction, Reasoning, Math, Coding, STEM, and Humanities.
* **Primary Application:** Automated LLM-as-a-Judge evaluation of multi-turn conversational coherence, conversational drift, and instruction adherence across successive API updates.
* **Access Link:** [https://huggingface.co/datasets/HuggingFaceH4/mt_bench_prompts](https://huggingface.co/datasets/HuggingFaceH4/mt_bench_prompts)

---

### 4. WildBench
* **Source:** [Allen Institute for AI (AI2)](https://github.com/allenai/WildBench) | [arXiv:2406.04770](https://arxiv.org/abs/2406.04770)
* **Description:** A collection of 1,024 challenging, uncurated real-world user interactions sourced directly from WildChat.
* **Primary Application:** Benchmarking models in realistic, "in-the-wild" prompt distributions to measure ecological validity and drift in practical user-facing tasks.
* **Access Link:** [https://huggingface.co/datasets/allenai/WildBench](https://huggingface.co/datasets/allenai/WildBench)

---

### 5. IFEval (Instruction-Following Evaluation)
* **Source:** [Google Research](https://github.com/google-research/google-research/tree/master/instruction_following_eval) | [arXiv:2311.07911](https://arxiv.org/abs/2311.07911)
* **Description:** A benchmark containing hundreds of prompt tasks with strictly verifiable lexical, formatting, and structural constraints (e.g., word count limits, specific JSON keys, capitalization constraints).
* **Primary Application:** Evaluating the loss of strict syntactic adherence and formatting drift caused by conversational fine-tuning updates.
* **Access Link:** [https://huggingface.co/datasets/wiseman/ifeval](https://huggingface.co/datasets/wiseman/ifeval)
