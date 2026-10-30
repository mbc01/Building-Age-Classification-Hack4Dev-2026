# Building Age Classification — Hack4Dev 2026
## Overview

The **Building Age Classification** project was developed as part of the Hack4Dev Data Science Hackathon at Mulungushi University, Zambia, in October 2026.

The primary purpose of this project was to develop a **machine-learning model that can classify buildings into different age categories using satellite-derived spectral and temporal features**. The goal was to investigate how machine learning can use Earth observation data to estimate building age and distinguish between buildings belonging to different age groups.

The project also explored how a model trained using data from one geographical region could be adapted to another region when only a limited number of labelled samples were available. This involved investigating geographic transfer from Madrid to Amsterdam and evaluating model performance under different few-shot learning scenarios.

## Project Objectives

- Develop a machine-learning model for classifying buildings into different age categories.
- Explore the use of satellite-derived spectral and temporal features for building-age classification.
- Establish and evaluate baseline machine-learning models.
- Investigate how additional features affect classification performance.
- Explore transferring a model between geographical regions.
- Evaluate performance when only a limited number of labelled samples are available.
- Compare experiments using appropriate evaluation metrics, including macro-averaged F1-score where applicable.
- Document the experiments, results, and limitations to support reproducibility.


## Research Objectives

- Establish a Random Forest baseline.
- Investigate additional spectral and temporal features.
- Compare feature groups under a consistent validation protocol.
- Evaluate source-only, target-only, prototype-based, and blended classifiers.
- Investigate performance under different labelled-sample budgets.
- Document experiments and validation methods.

## Study Context

The notebooks describe a transfer-learning setting involving Madrid and Amsterdam.

The experiments investigate target-region sample budgets of 5, 25, 50, 100, and 200 labelled pixels per class. These details should be checked against the official challenge materials.

## Repository Contents

- `1-Introduction (1).ipynb` — introduction.
- `2-Reading_Data (1).ipynb` — data reading and inspection.
- `3-Preprocessing (1).ipynb` — preprocessing.
- `4-Modelling (2).ipynb` — modelling and evaluation.
- `docs/experiment-log.csv` — experiment configurations and reported results.
- `requirements.txt` — Python dependencies.
- Experiment CSV files — saved experiment results and summaries.

## Experiments

Six experiment groups are documented:

1. FE-01 feature comparison.
2. Feature-group ablation.
3. Few-shot leaf-size and blend-weight exploration.
4. Few-shot transfer experiment A.
5. Few-shot transfer experiment B.
6. Few-shot transfer experiment C.

Recorded scores are local validation results, not official leaderboard scores. The original result files must be checked before the metrics are considered independently verified.

## Data Availability and Usage

The project references datasets associated with the Hack4Dev building-age classification challenge. At the time of this documentation, the datasets' redistribution permissions have not been verified.

The original challenge datasets and generated data files are therefore excluded from this repository pending confirmation of the applicable rules. Users should obtain the data through an authorized source and comply with the competition's data-use requirements.

## Environment Setup

Install the listed dependencies in an appropriate Python environment:

```bash
python -m pip install -r requirements.txt
```
