# Data Science Interview Prep

Interview preparation is a second learning loop: solve, explain, receive feedback, and revisit weak areas. Start with one timed session per week before you feel ready.

## Role families

| Role family | Typical emphasis | Portfolio signal |
|---|---|---|
| Product / Decision Science | SQL, metrics, experimentation, communication, causal reasoning | A clear decision memo and experiment analysis |
| Data Analyst | SQL, dashboards, data quality, business analysis | Reproducible SQL case study with stakeholder recommendations |
| Generalist Data Scientist | Statistics, ML, product sense, coding, communication | End-to-end model with error analysis and business framing |
| Applied Scientist / ML Scientist | Modeling depth, experiments, papers, coding, domain reasoning | Rigorous technical report and strong baselines |
| ML Engineer / Applied ML | Software engineering, systems, deployment, model lifecycle | Tested, containerized service with monitoring design |

Read the job description as a specification. Build a matrix of required skills, evidence you have, and the gap to close.

## SQL practice map

Practice in this order:

1. Filtering, CASE expressions, NULL semantics, and aggregations.
2. Joins and duplicate control; always state the expected row grain.
3. CTEs and readable decomposition.
4. Date arithmetic, cohorts, retention, and rolling windows.
5. Window functions: ranking, lag/lead, cumulative values, and sessionization.
6. Data quality checks and query performance intuition.

For every solution, explain: **What is one row? Which rows can multiply? What happens to NULLs? Why is this metric defined this way?**

## Statistics and experimentation

Be ready to explain the intuition, assumptions, and practical interpretation of:

- sampling bias, confounding, selection effects, and survivorship bias;
- mean, median, variance, quantiles, covariance, and correlation;
- confidence intervals versus prediction intervals;
- hypothesis tests, p-values, statistical power, effect size, and practical significance;
- A/B tests, randomization, guardrail metrics, multiple testing, and peeking;
- regression assumptions, residuals, regularization, and omitted-variable concerns;
- causal versus descriptive claims.

A high-quality answer begins by clarifying the population, treatment, outcome, time horizon, and decision. It does not begin with a formula.

## Machine learning questions

Use this response structure: **problem framing → baseline → data split → features → metric → model → diagnostics → decision**.

Common prompts include:

| Prompt | What a strong answer should cover |
|---|---|
| How would you predict churn? | Outcome window, intervention, leakage, class imbalance, threshold cost, retention action |
| How do you handle missing values? | Why missingness occurs, train-only fitting, indicators, domain rules, sensitivity checks |
| How do you choose a metric? | Business costs, prevalence, calibration, ranking versus classification, operating point |
| Your model is overfitting. What next? | Confirm split and leakage, simplify, regularize, add data, tune with validation, inspect slices |
| How do you explain a model? | Audience, global versus local explanation, correlated features, limitations, counterfactual caution |
| Offline metrics improved but business impact fell. Why? | Distribution shift, proxy metric, feedback loop, implementation error, selection bias, experiment design |

## Case study framework

When given an ambiguous business problem, ask clarifying questions before proposing a model.

1. **Objective:** What decision changes if we succeed?
2. **User and constraint:** Who acts on the result? What are latency, cost, privacy, and fairness constraints?
3. **Outcome:** What is the target, observation window, and label delay?
4. **Baseline:** What happens today, and what simple rule should we beat?
5. **Evaluation:** Which offline and online metrics matter? What are guardrails?
6. **Risks:** Where could the model fail or create harm?
7. **Launch plan:** How would you test, monitor, roll back, and learn?

## Coding and Python

Prioritize arrays, strings, hash maps, sorting, two pointers, stacks/queues, binary search, trees, graphs, recursion, and complexity. For data roles, also practice writing a clean transformation with pandas or SQL while explaining memory and correctness trade-offs.

During a coding answer, state assumptions, use a small example, write the simplest correct version, test edge cases, then discuss complexity and improvements.

## Behavioral preparation

Prepare six stories using **Situation → Task → Action → Result → Reflection**:

- a project that changed after feedback;
- a disagreement with a stakeholder;
- a failed analysis or model and what you learned;
- a time you improved data quality or reproducibility;
- a decision made under uncertainty;
- a project where you communicated technical work clearly.

Never memorize a fictional success story. Quantify impact only when the measurement is defensible, and explain how it was measured.

## Four-week practice cycle

| Week | Focus | Deliverable |
|---|---|---|
| 1 | SQL and Python fundamentals | 15 timed questions plus an error log |
| 2 | Statistics and experimentation | Two experiment designs explained aloud |
| 3 | ML and case studies | Three model-design prompts with trade-offs |
| 4 | Full loop | One mock interview, project walkthrough, and revised stories |

## Final checklist

Before an interview, you should be able to explain one project in 90 seconds, five minutes, and 20 minutes. You should know the grain and limitations of every dataset you used, the baseline and metric for every model, the biggest failure case, and the next experiment you would run.
