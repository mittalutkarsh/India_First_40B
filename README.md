# 40B — Research Proposal

A plan to train a 40-billion-parameter language model, from scratch, that matches Gemma 4 on general tasks, is fluent across the top-ten Indian languages, and reasons from an Indian perspective. Published as a small static website.

**Author:** Utkarsh Mittal

---

## What this is

The proposal treats data provenance, the tokenizer, and the model's "Indian perspective" as one problem. Native Indic text is scarce — the largest cleaned corpus tops out near ~280B tokens against a 1.32T Indic budget — so most of the corpus is repeated native text plus a bounded amount of manufactured text. The novel part is a from-scratch experiment that measures whether the origin of the training data (native vs. translated) changes the geometry of the model's perspective direction, and whether that direction survives alignment.

It covers the full pipeline: data strategy, cleaning, the tokenizer and fertility targets, the analytical framework (F1–F7), and post-training.

## Pages

| File | Section |
|---|---|
| `index.html` | Overview, visuals, and links to every section |
| `problem.html` | Problem & Approach — the constraint and the research reversal |
| `data.html` | Data Strategy — budget, provenance tiers, repetition rule, curriculum |
| `cleaning.html` | Data Cleaning — the nine objective-mapped stages |
| `tokenizer.html` | Tokenizer & Fertility — the minimax objective, per-language and per-domain targets, vocabulary, metrics |
| `research.html` | Research Core — the contrastive perspective corpus and F1–F7 |
| `training.html` | Post-training — native-first fine-tuning and alignment |




