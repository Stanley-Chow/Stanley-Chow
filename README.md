# Hi, I'm Stanley Chow 👋

**Applied Mathematics · Machine Learning · Recommendation Systems**

I am a Mathematics undergraduate at The University of Hong Kong, pursuing a
second major in Computer Science and a minor in Finance. I build recommendation
and retrieval systems, develop numerical methods for inverse problems, and
evaluate models through reproducible experiments. I am currently seeking
internships in **quantitative finance, recommendation systems, data science,
or machine learning engineering**.

## Current Focus

- Semantic IDs, residual quantization, Transformer sequence modeling, and constrained generative retrieval
- Multi-channel candidate retrieval, learning to rank, negative sampling, and temporal evaluation
- Reproducible ML experiments with ablations, baseline comparisons, and multiple pipeline seeds
- Numerical methods for inverse problems, reduced-order modeling, and regularization

## Featured Projects

### [Amazon Beauty: TIGER Generative Recommendation](https://github.com/Stanley-Chow/tiger-recommendation)

`Python` · `PyTorch` · `Transformers` · `Residual Quantization` · `MiniLM`

A TIGER-style generative recommender that predicts semantic product IDs from item histories, with controlled experiments on Amazon Beauty.

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

### Recovering a Hidden Heat Source

HKU Summer Research Fellowship · 2026

Heat spreads over time, blurring the shape of its source. My research asks how
we can work backwards from noisy temperature measurements to recover the
source's location and shape.

- Built numerical models of heat diffusion and compared full-sized solvers with reduced models using proper orthogonal decomposition (POD).
- Studied how training examples affect the shapes a compact model can recover, comparing reconstruction accuracy and computation time.
- Created a visual demonstration of three models recovering the same letter-shaped source from noisy measurements.

[Research overview & demo →](https://stanley-chow.github.io/research/parabolic-inverse-source/)

### Urban Rail Network Optimization

I studied how geometry, engineering constraints, and construction cost affect
the rail routes we can build. I combined analytical optimization with Particle
Swarm Optimization to search for feasible designs. This work was recognized in
the S.-T. Yau High School Science Award.

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

For internship opportunities or research collaborations, please get in touch.
