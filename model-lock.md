# **model-lock**

## Model lock (team record)

### The locked model

Model id: Qwen/Qwen2.5-1.5B-Instruct-AWQ

Quantisation: awq

Why this one: Passed the smoke test 10/10, with full distractor compliance and acceptable quality in the five-prompt spot check.

### The launch flags

The exact vLLM flags your team runs. Copy them from the SERVER_ARGS you launched with.

--model Qwen/Qwen2.5-1.5B-Instruct-AWQ --dtype half --max-model-len 4096 --gpu-memory-utilization 0.85 --port 8000 --quantization awq --enable-auto-tool-choice --tool-call-parser hermes

Tool-call parser: hermes

### The smoke score

Score (valid behaviours out of 10): 10

Distractor stayed call-free in the majority: yes

Passed the gate (>= 8/10 and distractor majority clean): yes

Measured against: AWQ (10/10)

### Quality spot check note

The quantised AWQ build held up across all five spot-check prompts. It produced relevant answers, followed the requested formats, and showed no obvious quality degradation in the tested prompts.
