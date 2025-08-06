
# GOODSPEED – Speculative Decoding for Efficient and Fair LLM Inference at the Edge

Deploying large language models (LLMs) in real-world applications demands both speed and accuracy—but current inference methods often fail to deliver on both fronts, especially in latency-sensitive and resource-constrained environments. **GOODSPEED** introduces a novel system for **speculative decoding** in distributed edge inference, aiming to **maximize inference efficiency and ensure fairness across clients**, all while retaining the high-quality outputs of large models.

## Goal

This project aims to build a scalable and adaptive framework for LLM inference that leverages speculative decoding to reduce latency and improve goodput—the rate of successfully accepted tokens per unit time—whilst fairly allocating resources across heterogeneous draft servers (clients). In addition to system-level improvements, we also explore **model-level tuning**, fine-tuning draft models to better align with the verification model, guided by insights from recent SD research and our own utility-based optimization objectives.

## Architecture

GOODSPEED builds on the core idea of **speculative decoding**: letting small, fast draft models generate candidate tokens, which are then verified by a larger, more accurate model. The framework supports **distributed deployment**, where each edge server hosts a lightweight draft model, and a central verification server performs batched validation using a high-capacity LLM.

This design helps eliminate common SD bottlenecks like uniform draft lengths and centralized delays, enabling:

- **Parallel speculative generation** across edge draft servers (clients)
- **Efficient batched verification** on the verification server  
- **Real-time feedback loops** to refine ongoing inferences  
- **Scalable system operation** under dynamic workloads  

## Fine-Tuning Draft Models

To further improve acceptance rates and speedup, we **fine-tune our draft models** based on techniques introduced in prior speculative decoding papers. Our tuning process is guided not only by token-level alignment but also by the **utility function** we optimize at the system level, helping each draft model better match the verification model’s behavior and contributing to overall goodput.

## Smarter Scheduling for Fair and Adaptive Inference

GOODSPEED introduces a **gradient-based scheduling algorithm** that adaptively decides how many tokens each draft server should generate in the next round. This decision is based on **real-time estimates** of token acceptance rates and goodput, ensuring fair and efficient use of the server’s verification capacity.

The algorithm solves a utility maximization problem under a hardware constraint, adjusting allocations over time as client performance and prompt difficulty vary. This not only improves goodput but also avoids starving any client, achieving **proportional fairness** in dynamic conditions.
