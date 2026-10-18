# llm-serving-portfolio

Notes and write-ups on fine-tuning, quantizing and serving open-weight LLMs on my own hardware.

Mihail Stoyanov, RnDaiTa Ltd, Sofia, Bulgaria.

## Focus

- **LLM fine-tuning:** LoRA fine-tuning of open-weight models.
- **Quantization:** low-bit (4-bit) builds of open models, checked against the full-precision model on standard benchmarks.
- **Serving:** vLLM and llama.cpp, measured for throughput under concurrent load.
- **Agent and multi-agent pipelines:** coding agents and multi-perspective setups running on locally served models.
- **Evaluation:** benchmark harnesses that report limits, confidence intervals and negative results.

## Hardware

Two NVIDIA DGX Spark (GB10) machines, run as a private lab.

## Planned write-ups

These are **planned**. None of them is published in this repository yet, and this README makes no result claims beyond what is committed here.

- [ ] Quantizing a mixture-of-experts model to 4-bit and checking accuracy against BF16 on several benchmarks
- [ ] Serving throughput on a DGX Spark at different concurrency levels
- [ ] A LoRA fine-tuning walkthrough, with a baseline comparison
- [ ] Notes on evaluation pitfalls (truncated answers, shared seeds, leaked answers) and how to catch them
- [ ] A coding agent running on a locally served model

## Status

Work in progress. Write-ups will be added here as they are cleaned up.