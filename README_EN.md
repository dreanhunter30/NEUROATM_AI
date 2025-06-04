
# NeuroATM — Lightweight Adaptive Intelligence Core

**NeuroATM (Neuro-Adaptive Token Memory)** is a minimal, interpretable, self-adaptive behavioral core for intelligent agents. It supports real-time memory-based learning without retraining or neural networks.

> The agent doesn't train weights. It learns from experience.  
> Logic becomes adaptive, explainable, and transferable.

---

## 🚀 Features

- 📦 Micro-core in ~150 lines of pure Python
- 🧠 Three memory types: short-term, long-term, success-pattern
- 🔁 Adaptation via **success/failure feedback** — no gradient or model training
- 🤖 Universal interface: `observe() → evaluate_result() → get_behavior_vector()`
- 🌐 Works with any input: tokens, sensors, LLM outputs, actions
- 🔄 Pattern sharing: agents can import/export behavior vectors
- 🧩 Easily pluggable into drones, games, edge-AI, autonomous agents

---

## 🔧 Quick Example

```python
agent = NeuroATM()
agent.observe(['wall', 'left', 'hit'])
agent.evaluate_result(False)
agent.observe(['wall', 'right', 'passed'])
agent.evaluate_result(True)
print(agent.get_behavior_vector())
# ['wall', 'right', 'passed']
```

---

## 📂 Structure

- `neuroatm.py` — core module
- `demo/` — usage examples
- `docs/` — architecture and design principles
- `LICENSE` — choose MIT or Apache 2.0

---

## 📄 License

All files in this repository — including source code, data, documentation, and associated materials —  
are licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0),  
unless stated otherwise.

This includes all past and future additions to this repository.
This repository and all its contents are further subject to a moral restriction clause:

> No part of this work may be used for military, weapons-related, or surveillance applications.


---

## ✉️ Author

Developed by **Bato Naidanov**  
📧 **bnaydanov@gmail.com**
