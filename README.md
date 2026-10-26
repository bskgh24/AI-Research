
# AI Research | Safety, Evaluation & Governance

## Overview
An independent research project investigating the reliability of AI-generated answers, evidence grounding, unsupported claims, and responsible AI evaluation.

## Research Question
Can a structured evaluation framework identify unsupported claims and evidence-grounding failures in language-model outputs?

## Objectives
- Develop a reproducible evaluation dataset.
- Compare AI-generated answers against supplied evidence.
- Assess factual support and appropriate uncertainty.
- Examine the limitations of automated evaluation.
- Document findings transparently.

## Technology Stack
- Python
- Pandas
- Google Colab
- GitHub

## Current Progress
- Created an initial synthetic evaluation dataset.
- Implemented and verified a simple rule-based baseline.
- Preparing the AI-model evaluation experiment.

## Research Integrity
The current examples are synthetic. No real language-model evaluation results have been established yet. Future findings will include methodology, limitations, and reproducibility details.

## Planned Deliverables
- Research notebook
- Evaluation dataset
- Python evaluation code
- Experimental results
- Research report

## Research Status
Early-stage pilot — work in progress.
## Initial Qwen Model Evaluation

### Experiment Overview

An exploratory AI safety evaluation was conducted using Qwen2.5-1.5B-Instruct, loaded locally in Google Colab using Hugging Face Transformers.

The experiment tested three synthetic evidence-based question-answering examples. The objective was to examine whether the model:
- Answered questions consistently with supplied evidence.
- Acknowledged when information was missing.
- Avoided unsupported claims.
- Produced direct and useful answers.

### Artifacts

- `AI_Safety_Evidence_Traceability_Pilot.ipynb` — experiment notebook.
- `ai_safety_pilot_examples.csv` — synthetic test dataset.
- `qwen_ai_safety_pilot_results.csv` — model responses and latency measurements.
- `qwen_ai_safety_manual_assessment.csv` — preliminary manual assessment.

### Preliminary Observations

The initial run produced responses for all three examples. Preliminary manual review found responses consistent with the supplied evidence, while one response was less direct than the reference answer.

These observations are exploratory and have not been independently validated.

### Limitations

- Only three synthetic examples were evaluated.
- The test cases are not representative of real-world AI use.
- Manual labels are preliminary and may be subject to researcher judgement.
- Response latency was measured in a CPU-based Colab session and is environment-dependent.
- No conclusions about general model safety, hallucination rates, or real-world reliability can be drawn from this pilot.

### Next Research Steps

1. Expand the dataset with systematically designed supported-answer, missing-evidence, and misleading-premise cases.
2. Define an explicit scoring rubric before evaluation.
3. Assess inter-rater agreement where feasible.
4. Compare model performance across a larger test set and document limitations.
5. Preserve code, data, model identification, and results for reproducibility.
