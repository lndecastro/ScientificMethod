# Chapter 6 — Experimental Design and Evaluation in AI & Data Science

## Purpose

This chapter addresses **how scientific evidence is generated and validated** in Artificial Intelligence (AI) and Data Science (DS). Even well-formulated research questions and sound methodologies can fail if experiments are poorly designed or inadequately evaluated.

Students will learn how to design **robust experiments**, select appropriate datasets and baselines, define meaningful evaluation metrics, and apply statistical reasoning to interpret results. The chapter emphasizes experimental rigor as a cornerstone of scientific credibility in AI/DS research.

---

## Learning Objectives

After completing this chapter, you will be able to:

- Design controlled and reproducible AI/DS experiments.
- Select and justify appropriate datasets and baselines.
- Choose evaluation metrics aligned with research objectives.
- Apply sound data splitting and validation strategies.
- Conduct error analysis and robustness assessment.
- Interpret experimental results using statistical reasoning.
- Identify common experimental pitfalls in AI/DS research.

---

## 1. The Role of Experimental Design in Scientific Research

Experimental design determines **how evidence is generated**. In AI/DS, experiments serve as computational analogs to laboratory studies and must therefore:

- Control confounding variables
- Enable fair comparison between methods
- Support replicability
- Provide interpretable outcomes

Poor experimental design undermines the validity of conclusions, regardless of model performance.

---

## 2. Dataset Selection and Characterization

### 2.1 Dataset Relevance
Datasets should be selected based on:
- Alignment with the research question
- Representativeness of the target domain
- Availability of labels and metadata
- Ethical and legal constraints

Using inappropriate datasets can invalidate findings.

---

### 2.2 Dataset Characterization
Before experimentation, datasets must be analyzed for:
- Size and dimensionality
- Class imbalance
- Noise and missing data
- Temporal or spatial dependencies
- Potential sources of bias

Dataset characterization is part of experimental rigor, not a preliminary step to be skipped.

---

## 3. Data Splitting and Validation Strategies

### 3.1 Train / Validation / Test Splits
Standard practice involves separating data into:
- Training data for model fitting
- Validation data for model selection
- Test data for final evaluation

Test data must remain untouched until final evaluation to prevent information leakage.

---

### 3.2 Cross-Validation and Resampling
Cross-validation techniques improve reliability when data are limited, but require careful implementation to avoid leakage, especially with:
- Time-series data
- Grouped or hierarchical data

---

## 4. Baselines and Comparative Evaluation

Baselines provide context for interpreting results.

### 4.1 Characteristics of Good Baselines
Good baselines are:
- Representative of existing approaches
- Appropriately tuned
- Clearly documented
- Reproducible

Weak or inappropriate baselines exaggerate perceived contributions.

---

### 4.2 Ablation Studies
Ablation studies isolate the contribution of individual components by systematically removing or modifying them. They are particularly important for complex models.

---

## 5. Evaluation Metrics

### 5.1 Metric Selection
Metrics must align with:
- Task objectives
- Data characteristics
- Stakeholder priorities

Examples include:
- Accuracy, precision, recall, F1-score
- ROC-AUC and PR-AUC
- Mean absolute error and RMSE
- Fairness and robustness metrics

Metric choice influences conclusions and must be justified explicitly.

---

### 5.2 Metric Limitations
No single metric captures all aspects of performance. Multiple metrics are often necessary to provide a complete picture.

---

## 6. Statistical Reasoning and Uncertainty

### 6.1 Variability and Randomness
AI experiments are affected by randomness in:
- Initialization
- Data sampling
- Optimization processes

Single-run results are rarely sufficient.

---

### 6.2 Statistical Significance and Effect Size
Statistical analysis helps distinguish meaningful differences from noise. Reporting uncertainty, confidence intervals, or variability across runs improves interpretability.

---

## 7. Error Analysis and Failure Cases

Error analysis involves examining:
- Misclassified or poorly predicted cases
- Patterns of systematic failure
- Sensitivity to input variations

Understanding errors often provides deeper scientific insight than aggregate metrics.

---

## 8. Robustness and Generalization

Robustness evaluation assesses:
- Sensitivity to noise
- Performance under distribution shift
- Stability across datasets or domains

Generalization is a scientific claim and must be supported by evidence.

---

## 9. Common Experimental Pitfalls

Frequent issues include:
- Data leakage
- Improper reuse of test data
- Overfitting to benchmarks
- Insufficient repetitions
- Cherry-picked results
- Ignoring negative findings

Avoiding these pitfalls is essential for scientific integrity.

---

## Key Takeaways

- Experimental design is central to scientific validity in AI/DS.
- Dataset selection and characterization shape research outcomes.
- Proper baselines and metrics are essential for fair comparison.
- Statistical reasoning supports credible interpretation.
- Error analysis and robustness testing deepen scientific understanding.

---

## Reflection Questions

1. Why is experimental design as important as model choice in AI/DS research?
2. How can data leakage occur even with standard splitting practices?
3. What risks arise from relying on a single evaluation metric?
4. How does error analysis contribute to scientific insight?
5. What evidence is required to support claims of generalization?

---

## Exercises

### Exercise 1 — Dataset Audit
Select a dataset relevant to your research and:
- Describe its key characteristics
- Identify potential sources of bias or leakage
- Discuss suitability for your research question

---

### Exercise 2 — Experimental Plan
Design an experimental protocol for your research question, specifying:
- Dataset(s)
- Data splitting strategy
- Baselines
- Evaluation metrics
- Number of experimental runs

---

### Exercise 3 — Error and Robustness Analysis
Propose methods for:
- Conducting error analysis
- Testing robustness under at least one perturbation or distribution shift

---

## Further Reading (Recent Literature)

- Ji, Z., et al. (2023). Survey of hallucination in natural language generation. *ACM Computing Surveys, 55*(12), 1–38. https://doi.org/10.1145/3571730

- Raji, I. D., et al. (2023). Closing the AI accountability gap: Defining an end-to-end framework for internal algorithmic auditing. *Proceedings of the ACM Conference on Fairness, Accountability, and Transparency*, 33–44. https://doi.org/10.1145/3593013.3594013

- Bommasani, R., et al. (2023). On the opportunities and risks of foundation models. *Stanford Center for Research on Foundation Models*. https://doi.org/10.48550/arXiv.2108.07258

---

## What’s Next

In **Chapter 7**, we will focus on **reproducibility, tooling, and research pipelines**, examining how experiment tracking, version control, and documentation support trustworthy and reusable AI/DS research.
