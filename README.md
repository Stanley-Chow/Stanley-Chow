# Hi, I'm Stanley Chow 👋

**Recommendation & Search Algorithms · Machine Learning · Applied Mathematics**

I am a Mathematics undergraduate at The University of Hong Kong, pursuing a
second major in Computer Science and a minor in Finance. I build generative and
two-stage recommenders, C++ retrieval systems, and numerical methods for inverse
problems. My interests span recommendation, search, ranking, and advertising
algorithms, backed by reproducible experiments in Python and PyTorch.

## Current Focus

- Semantic IDs, residual quantization, Transformer sequence modeling, and constrained generative retrieval
- Multi-channel candidate retrieval, learning to rank, negative sampling, and temporal evaluation
- Reproducible ML experiments with ablations, baseline comparisons, and multiple pipeline seeds
- Numerical methods for inverse problems, reduced-order modeling, and regularization

## Featured Projects

### [TIGER-Style Generative Recommendation](https://github.com/Stanley-Chow/tiger-recommendation)

`Python` · `PyTorch` · `Transformers` · `Residual Quantization` · `MiniLM`

A generative recommender that predicts semantic product IDs from item histories, with controlled experiments on Amazon Beauty.

- Built a residual-quantization tokenizer over frozen metadata embeddings, an encoder–decoder Transformer, and trie-constrained beam search over valid catalog codes.
- Evaluated three seeds under global time cutoffs on a **50,000-user** Amazon Reviews 2023 cohort: **6.853% mean Recall@100**, versus **7.993% for SASRec**, on **2,252 eligible warm test users**. Reported ranking and new-item limitations alongside the results.
- Exported a portable CPU inference bundle with CLI/HTTP interfaces, five retrieval/fusion strategies, and full-history seen-item exclusion; audited checkpoint hashes, temporal contexts, and saved rankings.

[Repository →](https://github.com/Stanley-Chow/tiger-recommendation) · [Latest results →](https://github.com/Stanley-Chow/tiger-recommendation/blob/main/docs/m5_results.md)

### [H&M Two-Stage Personalized Recommendation System](https://github.com/Stanley-Chow/hm-2stage-recommender)

`Python` · `PyTorch` · `LightGBM` · `DuckDB`

An offline retrieval-and-ranking system built on 31.8 million H&M transaction events.

- Combined nine heuristic, collaborative, learned, text, and image retrieval channels in a quota-aware K=500 candidate interface.
- Trained a LambdaRank model on 100,000 customer-week queries under four rolling temporal cutoffs; an untouched future week reached MAP@12 of **0.03448**, a **3.94%** relative gap from development.
- Ran bounded-memory inference for **1,371,980 customers** across 138 shards and submitted final predictions scoring **0.03117 public / 0.03116 private MAP@12** on Kaggle.

[Repository →](https://github.com/Stanley-Chow/hm-2stage-recommender)

### [DocuQuest Agent](https://github.com/Stanley-Chow/docuquest-agent)

`C++17` · `Information Retrieval` · `CMake` · `LLM APIs`

A retrieval-augmented document question-answering system with a deterministic C++ search layer.

- Implemented tokenization, a custom ownership-aware binary-search-tree multimap, and an inverted index.
- Applied AND constraints within expanded term groups and unions across groups before grounded synthesis.
- Injected the model client so retrieval tests remain deterministic and credential-free; live generation reads credentials only from environment variables.

[Repository →](https://github.com/Stanley-Chow/docuquest-agent)

### [Behavioral Personality Analytics](https://github.com/Stanley-Chow/behavioral-personality-analytics)

`Python` · `scikit-learn` · `pandas` · `Matplotlib`

A study of personality, stage-fright, and behavioral-outcome prediction on generated data, with separate model-selection and holdout partitions.

- Kept preprocessing and model selection inside development pipelines before one-time evaluation on an untouched 20% holdout.
- Evaluated **381** model-and-feature-subset configurations with a predeclared parsimony rule.
- Selected a three-feature Gradient Boosting model with **0.9651 holdout ROC-AUC**, retaining a compact behavioral feature set.

[Repository →](https://github.com/Stanley-Chow/behavioral-personality-analytics)

### [Flight Price Prediction & Pricing Dynamics](https://github.com/Stanley-Chow/flight-price-prediction-and-pricing-analysis)

`Python` · `XGBoost` · `scikit-learn` · `pandas`

A collaborative regression study comparing tree ensembles, regularized models, and principal-component regression on airfare data.

- The final XGBoost model reached **RMSE ₹2,319.47** and **R² 0.9896** on a 60,031-row held-out same-period test set.
- Examined model-estimated booking-time effects with partial dependence while keeping predictive associations distinct from causal claims.
- My recorded contributions cover code for Experiments 1 and 2 and the interpretation and discussion for Experiment 2.

[Repository →](https://github.com/Stanley-Chow/flight-price-prediction-and-pricing-analysis)

## Research

### Covariance-Designed POD for Parabolic Inverse Source Problems

As an HKU Summer Research Fellow, I study reduced-order reconstruction of
source geometry from noisy final-time diffusion observations.

- Implemented 100 × 100 finite-difference simulations, Tikhonov regularization, and Monte Carlo noise and sensor experiments.
- Constructed covariance-designed Proper Orthogonal Decomposition bases and reduced reconstruction to a 20–40 dimensional solution space.
- Audited five numerical experiments against theoretical claims while preparing a manuscript-style research write-up.

[Research overview & demo →](https://stanley-chow.github.io/research/parabolic-inverse-source/)

I have also modeled urban rail route design under geometric and construction
constraints, combining analytical linear-programming cases with Particle Swarm
Optimization for multi-intersection layouts. This work was recognized in the
S.-T. Yau High School Science Award.

## Technical Toolkit

**Languages**

Python · C++ · SQL · MATLAB

**Machine Learning & Data**

PyTorch · LightGBM · XGBoost · scikit-learn · pandas · NumPy · SciPy · DuckDB

**Recommendation & Search**

Generative Retrieval · Semantic IDs · Residual Quantization · SASRec · Candidate Retrieval · Collaborative Filtering · Two-Tower Models · LightGCN · LambdaRank · Negative Sampling · Temporal Validation · MAP/NDCG/Recall

**Engineering & Research**

Git · CMake · pytest · Jupyter · LaTeX · Numerical Optimization · Experiment Design

## Selected Highlights

- HKU Summer Research Fellow in numerical inverse problems and reduced-order modeling
- GPA **3.98/4.30**; Dean's List, HKU Undergraduate Entrance Scholarship, and Lee Shau Kee Scholarship
- Mathematics coursework in probability, stochastic processes, optimization, numerical analysis, and scientific computing

## Contact

- Email: [pingsenchow@outlook.com](mailto:pingsenchow@outlook.com)
- GitHub: [github.com/Stanley-Chow](https://github.com/Stanley-Chow)
- Portfolio: [stanley-chow.github.io](https://stanley-chow.github.io/)

I am open to internship and research opportunities in recommendation, search,
ranking, advertising algorithms, machine learning engineering, and applied data
science.
