# Roadmap: Zero to Advanced Data Science

This roadmap is a sequence of **capability gates**, not a race through content. At every stage, write, practice, build, explain, and review.

## Level 0 — Foundations

**Outcome:** You can write readable Python, use Git confidently, inspect data, and reason about basic functions, vectors, and uncertainty.

| Track | Learn | Proof of skill |
|---|---|---|
| Python | variables, control flow, functions, modules, exceptions, iterators, OOP basics, typing, testing | 20 short exercises plus a small package with tests |
| Developer workflow | shell, virtual environments, Git branches, commits, README writing | Reproduce your project from a clean clone |
| Math | algebra, functions, logarithms, vectors, matrices, derivatives intuition | Explain a linear model and gradient descent visually |
| Data structures | lists, dictionaries, sets, tuples, complexity intuition | Solve basic array/string/hash-map problems |

**Gate:** Given a small CSV, you can load it, validate assumptions, write reusable functions, create a plot, and explain every transformation.

## Level 1 — Analyst Core

**Outcome:** You can turn messy tables into a reliable analysis and communicate the result to a non-technical stakeholder.

| Track | Learn | Proof of skill |
|---|---|---|
| SQL | SELECT, joins, aggregations, CTEs, window functions, dates, NULLs, query plans | Solve 30 problems and explain row grain for every query |
| Python data stack | NumPy, pandas, data types, missingness, reshaping, grouping, pipelines | Build a clean analysis notebook and a script version |
| Visualization | distributions, uncertainty, comparison, trends, annotation, accessibility | Produce five decision-oriented charts, not five decorative charts |
| Statistics | sampling, distributions, confidence intervals, hypothesis tests, effect size, correlation | Write a one-page statistical interpretation with limitations |
| Communication | problem framing, metric definitions, executive summary, reproducibility | Present a three-minute recommendation supported by evidence |

**Gate:** Complete an end-to-end EDA: define the question, document the data, clean it, analyze it, visualize it, quantify uncertainty where relevant, and end with a recommendation plus caveats.

## Level 2 — Machine Learning Practitioner

**Outcome:** You can build a baseline, prevent leakage, compare models fairly, and diagnose errors.

| Track | Learn | Proof of skill |
|---|---|---|
| Supervised ML | linear/logistic regression, trees, random forests, gradient boosting, regularization | Compare a simple baseline with at least two justified alternatives |
| Unsupervised ML | clustering, PCA, anomaly detection, dimensionality reduction | Explain when an unsupervised result is useful and when it is only exploratory |
| Evaluation | train/validation/test, cross-validation, calibration, thresholding, ROC/PR, regression metrics | Select metrics based on business costs, not habit |
| Feature work | encoding, imputation, scaling, feature selection, pipelines | Use a leakage-safe preprocessing pipeline |
| Explainability | coefficients, permutation importance, partial dependence, slices, error analysis | Document which cases the model fails on and why |

**Gate:** Ship a repository where a reviewer can run one command, reproduce the evaluation, inspect the data contract, and understand why the final model was selected.

## Level 3 — Production and Impact

**Outcome:** You can connect a model or analysis to a usable system and measure whether it helps.

| Track | Learn | Proof of skill |
|---|---|---|
| Software quality | packaging, logging, configuration, unit/integration tests, CI | Tests run automatically on every pull request |
| Serving | REST APIs, batch inference, Docker, versioning, schema validation | A documented endpoint or batch job works from a clean environment |
| Experimentation | randomization, power, guardrails, CUPED intuition, sequential pitfalls | Design an experiment with primary metric and stopping rule |
| Data systems | warehouse concepts, partitions, incremental jobs, orchestration, data quality | A small pipeline has retries, validation, and failure documentation |
| Monitoring | drift, data quality, latency, model performance, alerting | Define what you would monitor before deployment |

**Gate:** Explain the full lifecycle from raw data to decision, including cost, latency, privacy, monitoring, rollback, and ownership.

## Level 4 — Advanced / Specialist

Choose one primary specialization and one supporting area. Depth is more valuable than collecting frameworks.

| Specialization | Core topics | Portfolio direction |
|---|---|---|
| Causal inference | DAGs, confounding, treatment effects, quasi-experiments | Estimate the impact of a product or policy change |
| Time series | baselines, temporal validation, seasonality, forecasting intervals | Forecast demand with a realistic backtest |
| NLP / LLM systems | representations, retrieval, evaluation, hallucination, safety | Build an evaluated retrieval or classification system |
| Deep learning | optimization, regularization, embeddings, transfer learning | Compare a simple baseline with a neural approach |
| Recommenders | candidate generation, ranking, offline/online metrics | Design an offline evaluation and cold-start strategy |
| Analytics engineering | dimensional modeling, dbt-style transformations, semantic layers | Build a tested analytical data model |

**Gate:** Produce a technical report that states the problem, assumptions, methods, ablations or alternatives, evaluation design, limitations, responsible-use risks, and operational plan.

## Diagnostic checklist

Mark each statement **green**, **yellow**, or **red**. Start at the lowest level containing a red statement.

| Statement | Green means… |
|---|---|
| I can explain a project to a non-technical person. | I can state the decision, metric, evidence, and limitation in under two minutes. |
| I can write SQL with joins and windows. | I can reason about grain, duplicates, NULLs, and edge cases. |
| I can validate a model. | I can identify leakage, choose a metric, use a baseline, and analyze errors. |
| I can ship reproducible work. | Another person can clone, install, run, test, and inspect the result. |
| I can discuss impact. | I can connect model quality to cost, risk, user experience, or revenue without overclaiming. |

## Recommended order of projects

1. Descriptive analysis with a stakeholder memo.
2. SQL analytics case study with window functions.
3. Leakage-safe tabular classification or regression.
4. Experiment or quasi-experiment analysis.
5. Deployed model or data product with monitoring plan.
6. Specialist capstone with a technical report.

## Anti-patterns to avoid

Do not optimize a leaderboard score before defining the decision. Do not publish notebooks with hidden state, unexplained cleaning, or no baseline. Do not use a complex model to compensate for a weak problem definition. Do not claim causality from correlation. Do not hide negative results; failure analysis is part of the portfolio.
