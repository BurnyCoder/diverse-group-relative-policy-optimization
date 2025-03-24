# Diverse Group Relative Policy Optimization (DGRPO)

Language models trained with reinforcement learning often converge to common solution patterns, limiting their creative problem-solving capabilities. This paper introduces Diverse Group Relative Policy Optimization (DGRPO), an extension of Group Relative Policy Optimization (GRPO) that specifically addresses this limitation. While GRPO normalizes rewards within groups of responses to promote accuracy, DGRPO incorporates solution diversity into the advantage calculation through two novel approaches: (1) upweighting less likely but correct tokens to incentivize rare solutions, and (2) quantifying solution uniqueness using cosine similarity of neural embeddings. By introducing a configurable diversity weight parameter, DGRPO allows practitioners to balance accuracy with exploration of diverse solution strategies. My approach encourages language models to discover multiple valid approaches to problems, a critical capability for applications in scientific discovery, mathematical problem-solving, creative coding, and art. DGRPO demonstrates how reinforcement learning can be adapted to reward not just correctness but also the novelty and diversity of solutions in generative AI systems.

Read `Diverse_Group_Relative_Policy_Optimization_(DGRPO).pdf` paper for more details.

## Usage

Run `Diverse_Group_Relative_Policy_Optimization_(DGRPO).ipynb` locally or in Google Colab.

## Summary

The project includes:

- Implements GRPO and DGRPO training algorithms with reward function implementations
- Training examples on math reasoning tasks (GSM8K)
- Comparative model evaluation tools

## To do

- Double check code for errors
- Fix broken plotting
- Fix broken testing
- Benchmark and compare original model, model trained using GRPO, and model trained using DGRPO
- Implement cosine similarity method in code and benchmark it