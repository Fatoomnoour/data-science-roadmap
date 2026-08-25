# Project Ladder

A portfolio is strongest when each project demonstrates a different professional capability. For every project, publish a short README, a reproducible environment, a data dictionary, tests where applicable, and a section called **What I would do next**.

## Project 1 — Public Data Story

**Question:** What changed, where, and why might it matter?

Use a public dataset such as bike sharing, city services, public health, or climate data. Define the unit of observation, clean obvious quality issues, create a small set of purposeful charts, and write a one-page memo for a fictional decision-maker.

**Skills:** Python, pandas, visualization, descriptive statistics, communication.

**Acceptance criteria:** The analysis can be reproduced from a clean environment; every chart has a takeaway; limitations and missingness are explicit; conclusions do not exceed the evidence.

## Project 2 — SQL Analytics Case Study

**Question:** Which customers, products, or operational segments need attention?

Create a relational schema from a public dataset or synthetic transactional data. Answer ten business questions using joins, CTEs, conditional aggregation, date logic, and window functions. Include the expected grain and a validation query for every major result.

**Skills:** SQL, data modeling, metrics, query reasoning.

**Acceptance criteria:** Queries are readable and documented; duplicate multiplication is checked; NULL behavior is intentional; the final report distinguishes descriptive facts from recommendations.

## Project 3 — Leakage-Safe Churn or Risk Model

**Question:** Which entities are likely to experience an outcome within a defined future window?

Build a baseline and two candidate models. Split data according to the time or prediction setting, put preprocessing inside a pipeline, choose metrics based on the decision cost, calibrate or tune the threshold, and analyze performance by meaningful slices.

**Skills:** scikit-learn, feature engineering, evaluation, error analysis, explainability.

**Acceptance criteria:** No future information enters features; the baseline is competitive enough to discuss; the README includes a model card; metrics include uncertainty or repeated validation; failure cases are illustrated.

## Project 4 — Experiment or Quasi-Experiment

**Question:** Did a product, campaign, policy, or process change cause a measurable effect?

Design an A/B test or analyze a naturally occurring intervention. State the estimand, population, treatment, primary metric, guardrails, power assumptions, and decision rule. If randomization is unavailable, describe the identification assumptions and conduct sensitivity checks.

**Skills:** statistics, experimentation, causal reasoning, communication.

**Acceptance criteria:** The analysis distinguishes statistical significance from practical importance; multiple testing and stopping behavior are addressed; alternative explanations are discussed; the conclusion is appropriately cautious.

## Project 5 — End-to-End Model Service

**Question:** How would a useful prediction become a reliable product capability?

Train a model, serialize it safely, expose a versioned API or batch job, validate inputs, add tests and logging, containerize the service, and document monitoring signals such as data drift, latency, missingness, and outcome quality.

**Skills:** Python packaging, FastAPI or equivalent, Docker, testing, CI, MLOps thinking.

**Acceptance criteria:** One command starts the service; a sample request works; invalid inputs return useful errors; tests cover core transformations; the deployment and rollback plan are written down.

## Project 6 — Advanced Specialization Capstone

Choose one: forecasting, causal inference, NLP/RAG evaluation, recommender systems, computer vision, or analytics engineering.

**Acceptance criteria:** The capstone includes a literature or baseline review, a clear evaluation protocol, ablations or meaningful alternatives, an error taxonomy, responsible-use considerations, and a technical report that another practitioner can critique.

## Project README template

```markdown
# Project title

## Decision / user problem
What decision will this work support? Who is the user?

## Data and data-generating process
What does one row represent? What is missing, biased, delayed, or unreliable?

## Approach
What baseline, alternatives, and assumptions were considered?

## Evaluation
Which metric matches the decision? How was leakage prevented?

## Results
Show the smallest set of charts/tables that support the conclusion.

## Limitations and responsible use
Where can this fail? Who could be harmed? What should not be inferred?

## Reproduce
```bash
# setup and run commands
```

## Next steps
What would you test or improve with more time, data, or access?
```

## Project scoring rubric

| Dimension | 0 | 1 | 2 |
|---|---|---|---|
| Problem framing | No decision | Vague question | Specific decision, user, and success metric |
| Data quality | Unexamined | Basic cleaning | Grain, missingness, bias, and validation documented |
| Method | Arbitrary | One method | Baseline, alternatives, and justified choice |
| Evaluation | One score | Reasonable split | Leakage-safe design, uncertainty, slices, and error analysis |
| Communication | Notebook only | Basic README | Decision memo, visuals, limitations, and reproducibility |
| Engineering | Does not run | Runs locally | Clean setup, tests, versioning, and operational plan |

Aim for **10/12 or higher** before listing a project as a flagship portfolio piece.
