# LLM Inference Engine Benchmark

A comparison of vLLM, LMDeploy, and SGLang for batch inference on an NVIDIA H100. The published study uses Llama 3.1 8B Instruct with a shared set of ShareGPT prompts.

[Read the benchmark on AIMultiple](https://aimultiple.com/inference-engines).

The evaluation compares generated tokens per second under the configurations documented in the article. It also describes the dependency, kernel, and memory-setting work required to run each engine.

The local research includes separate benchmark runners for the three engines. Retained development scripts contain configuration differences from the final published setup. The article is the reference for the settings and results summarized here.

This comparison covers an offline batch workload on one hardware and model configuration. It does not establish the same ranking for interactive serving, other model sizes, or different accelerators. The published methodology explains the workload, repeated runs, and deployment conditions needed to interpret its throughput measurements.

The benchmark implementation was developed for AIMultiple and belongs to AIMultiple. This repository is a documentation summary. Source code and benchmark datasets are not distributed here.
