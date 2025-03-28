# 🐉 Project Loong

Project Loong is a collaborative effort to explore whether reasoning-capable models can bootstrap themselves from small, high-quality **seed datasets** by generating synthetic data — and verifying LLM agent responses.

This repository contains:

- ✅ **Seed Datasets** — Real, human-vetted data from computable domains like math, physics, finance, etc.
- 📘 **Cookbooks** — Modular scripts for synthetic data generation, verification, and RL training loops.

---

## 🔍 What’s in this Repo?

### `/data/`
A collection of **seed datasets**, structured for generation and verification.

Each datapoint includes:
- `question`
- `final_answer`
- `rationale` (typically code)
- `metadata` (license, source, domain)
- `misc` (difficulty, tags, anything else)

Domains include:
- Mathematical Programming
- Graph Theory
- Computational Biology
…and more.

Each dataset is designed to allow automatic evaluation via **verifiers**, usually by executing the rationale code and comparing the output to the known answer.

Want to contribute your own? See the [CONTRIBUTING.md](.data/CONTRIBUTING.md) for seed datasets.

---

### `/cookbooks/`
Reusable scripts and notebooks for:
- Few-shot prompting from seed data
- Generating synthetic questions, rationales, and answers
- Running verifiers over generations
- Exporting datasets for supervised fine-tuning or RL

These pipelines allow you to condition generations on real data, verify outputs, and build consistent synthetic traces.

---

## 🧬 Contribute

We're looking for:
- Seed datasets in verifiable domains
- New verifiers
- Cookbook improvements
- Experimental environments for RL

Get started: [CONTRIBUTING.md](./CONTRIBUTING.md)

---

## 📜 License

- Code: [LICENSE](./LICENSE)
- Data: Per-dataset license in `metadata.json`

---

## 👥 Maintainers

Project Loong is led by the [CAMEL](https://www.camel-ai.org/) team, with contributors from across the open-source AI research community.

🐲 Join Us
