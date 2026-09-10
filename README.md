# Mobile Game Experimentation

## Overview

This project analyses a real-world style A/B test using the **Cookie Cats** mobile game dataset.

The experiment tests whether moving a progression gate from **level 30 to level 40** affects player behaviour (will players stay more engaged and be more likely to return to the game).

What we can measure is behaviour after installation, mainly:
- whether they return after 1 day
- whether they return after 7 days
- how many game rounds they play
So the experiment is really about retention and engagement, not acquisition.

The goal is not simply to determine whether one variant performs better. The project is designed to evaluate the experiment as a Product Data Scientist would in practice, including experiment validity, statistical significance, effect size, statistical power, commercial significance and rollout decisions.

## Business Question

Should the game move its progression gate from level 30 to level 40?

The analysis will consider whether the treatment:

- improves player retention
- changes player engagement
- produces a statistically reliable treatment effect
- produces an effect large enough to matter from a product perspective
- creates any unintended negative effects

The final objective is to make a recommendation to:

**Launch, iterate, run a further experiment, or stop the treatment.**

## Dataset

The dataset contains approximately 90,000 players randomly assigned to one of two experiment groups:

- `gate_30` — existing experience / control
- `gate_40` — new experience / treatment

Available variables include:

- `userid` — unique player identifier
- `version` — assigned experiment group
- `sum_gamerounds` — number of game rounds played
- `retention_1` — whether the player returned after one day
- `retention_7` — whether the player returned after seven days

## Experimentation Topics

This project will cover:

- Experimental design
- Hypothesis formulation
- Primary and guardrail metric selection
- Randomisation and experiment health checks
- Sample Ratio Mismatch
- Treatment effect estimation
- Confidence intervals
- Statistical hypothesis testing
- Absolute and relative uplift
- Effect size
- Statistical power
- Minimum Detectable Effect (MDE)
- Sample-size estimation
- Type I and Type II errors
- Multiple testing
- Heterogeneous treatment effects
- Incrementality
- Practical / product significance
- Experiment decision-making

## Project Structure

```text
mobile-game-experimentation/
│
├── data/
│
├── notebooks/
│   └── 01_experiment_audit.ipynb
│
├── src/
│
├── outputs/
│
├── README.md
├── requirements.txt
└── .gitignore