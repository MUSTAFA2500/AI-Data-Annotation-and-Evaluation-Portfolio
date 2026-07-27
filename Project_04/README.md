# Project 04 — Reliable AI Evaluation

## Teaching AI to Give More Reliable Answers

### Core Idea

AI can produce fluent answers that still contain factual errors, unsupported claims, hidden uncertainty, or biased reasoning.

This project demonstrates how AI responses can be evaluated by humans using clear criteria so that better, safer, and more reliable systems can be built.

> **User Question → AI Responses → Human Evaluation → Preference / Factuality / QA**

### Main Modality

**Text / LLM Responses**

### Main Tasks

* Response quality evaluation
* Human preference ranking
* Pairwise response comparison
* Factuality checking
* Hallucination detection
* Evidence evaluation
* Relevance assessment
* Reasoning evaluation
* Uncertainty assessment
* Annotation quality control

### Main Tools

* Labelbox
* Label Studio

### Main Formats / Concepts

* General RLHF
* Structured evaluation data
* Factuality and evidence-based review
* QA review workflows

---

## 1. Objective

The objective of this project is to evaluate AI-generated responses using structured human judgment.

The project focuses on determining whether an answer is relevant, accurate, useful, supported by evidence, and appropriately uncertain.

It also demonstrates how human reviewers can compare multiple responses, identify hallucinations or unsupported claims, and apply quality control to evaluation data.

---

## 2. Role in the Overall Portfolio

This project represents the portfolio's reliability and evaluation layer.

It demonstrates the ability to help AI systems answer:

> **Is this answer reliable?**

Unlike the first three projects, which focus on transforming raw data into structured annotations, this project focuses on evaluating the quality of AI outputs themselves.

It connects the annotation skills developed across the portfolio with RLHF-style evaluation, factuality verification, and quality assurance.

---

## 3. Dataset

> **Dataset details will be finalized after selecting the exact prompt set, AI responses, and reference sources for this project.**

This section should document:

* Prompt source
* Response source
* Reference or evidence source
* Number of prompts selected
* Number of AI responses evaluated
* Selection criteria
* License or usage notes for any source material
* What I personally annotated
* What I modified
* What I publish publicly

### Planned dataset requirements

The dataset should be:

* publicly usable or safely created from public prompts
* small enough to evaluate carefully
* suitable for response comparison and factuality review
* appropriate for public GitHub publication in sample form
* aligned with the project’s goal of evaluating reliability

### Dataset notes

* I will clearly document the origin of prompts, responses, and references.
* I will use only materials that can be shared responsibly.
* I will publish selected samples and demonstrations if the full evaluation set should not be redistributed.

---

## 4. Annotation Ontology

The annotation ontology defines what can be evaluated and how the categories are organized.

### Example ontology

```text id="n2y9hb"
RELEVANCE
├── Low
├── Medium
└── High

FACTUALITY
├── Incorrect
├── Partially Correct
└── Correct

EVIDENCE
├── Unsupported
├── Partially Supported
└── Well Supported

HALLUCINATION
├── Present
└── Not Present

UNCERTAINTY
├── Missing
├── Appropriate
└── Excessive

OVERALL PREFERENCE
├── Response A
├── Response B
└── Tie
```

### Class documentation

Each label should include:

* Definition
* Inclusion criteria
* Exclusion criteria
* Examples
* Ambiguous cases

### Notes

The ontology should stay clear and practical.

The goal is not to create an overly complicated score sheet, but a reliable and interpretable evaluation system.

---

## 5. Annotation Guidelines

The annotation guidelines explain exactly how AI responses should be evaluated.

### The guidelines should cover:

* How to judge relevance
* How to judge factual correctness
* How to detect hallucinations
* How to evaluate supporting evidence
* How to compare two responses
* How to judge uncertainty
* How to handle partial correctness
* How to resolve ambiguous cases

### Example rules

* Judge a response based on whether it actually answers the question.
* Mark a claim as incorrect if it conflicts with reliable reference information.
* Mark a response as unsupported if it makes a claim without evidence.
* Do not penalize appropriate uncertainty.
* Prefer the response that is more accurate, clearer, and better supported.
* If both responses are weak, use the tie option when appropriate.
* If a case is ambiguous, follow the project’s decision rule instead of guessing.

The guidelines are designed to promote consistency, accuracy, and reproducibility throughout the evaluation process.

---

## 6. Annotation Workflow

```text id="g1kqcp"
Question Selection
        ↓
AI Response Generation
        ↓
Reference / Evidence Collection
        ↓
Evaluation Ontology Definition
        ↓
Annotation Guidelines
        ↓
Initial Evaluation
        ↓
Pairwise Comparison
        ↓
Factuality Review
        ↓
Quality Control
        ↓
Export
        ↓
Format Validation
```

### Workflow explanation

1. Select a set of prompts or questions.
2. Generate or collect AI responses.
3. Gather reference information or evidence sources.
4. Define the evaluation ontology.
5. Write clear evaluation guidelines.
6. Perform the first round of human evaluation.
7. Compare responses pairwise when needed.
8. Review factuality, evidence, and uncertainty.
9. Run quality control checks.
10. Export the final evaluation data.
11. Validate the export format.

---

## 7. Quality Control

The quality-control process focuses on identifying and correcting problems in the human evaluation data.

### Quality-control checks

* Inconsistent preference labels
* Incorrect factuality labels
* Unsupported evaluation judgments
* Missing evidence checks
* Hallucination misclassification
* Relevance errors
* Weak or unclear reasoning
* Ambiguous cases
* Duplicate evaluations
* Other evaluation errors

### QA methods

* QA checklist
* Error taxonomy
* Sample evaluation errors
* Before/after corrections
* Final quality summary

### Example error types

```text id="jv5m4f"
Wrong preference label
Incorrect factuality judgment
Evidence not checked
Hallucination missed
Uncertainty misread
Relevance underestimated
Tie used incorrectly
Reasoning explanation incomplete
```

---

## 8. Results

> **Results will be added after the evaluation dataset and QA are completed.**

This section should report:

* Number of prompts
* Number of AI responses
* Number of pairwise comparisons
* Number of factuality evaluations
* Number of hallucination cases
* Number of QA corrections
* Common error types
* Final quality observations

### Placeholder result format

```text id="u9n3qr"
Prompts evaluated: [to be added]
AI responses reviewed: [to be added]
Pairwise comparisons: [to be added]
Factuality judgments: [to be added]
Hallucination cases found: [to be added]
QA corrections: [to be added]
Most common issue: [to be added]
Final observation: [to be added]
```

---

## 9. Examples

This section will include representative examples showing the full evaluation process.

### Planned examples

* User question
* Response A
* Response B
* Human preference decision
* Factuality check
* Hallucination example
* Correct uncertainty example
* Before/after QA example

### Example file locations

```text id="c6r8dv"
screenshots/
├── prompt-example.png
├── response-a.png
├── response-b.png
├── labelbox-evaluation.png
├── label-studio-evaluation.png
├── factuality-review.png
└── before-after-correction.png
```

The goal is to show not only the final decision, but also the evaluation and review process itself.

---

## 10. Exported Data

Representative samples of the exported data will be provided here.

### Expected export contents

* Preference labels
* Pairwise ranking data
* Factuality labels
* Hallucination labels
* Evidence links
* QA results
* Evaluation schema

### Example export files

```text id="h4x6wy"
sample-output/
└── sample-evaluation.json
```

If the full dataset should not be published publicly, only selected samples and demonstrations will be shared.

This allows others to evaluate the work while keeping control over the complete project assets.

---

## 11. Skills Demonstrated

* General RLHF concepts
* Human preference evaluation
* Pairwise ranking
* AI response evaluation
* Factuality verification
* Hallucination detection
* Evidence evaluation
* Relevance assessment
* Uncertainty assessment
* Annotation ontology design
* Annotation guideline development
* Structured evaluation data preparation
* Quality assurance
* Error analysis
* Critical reasoning
* AI reliability workflows

---

## 12. Tools

* Labelbox
* Label Studio

---

## Project Status

**In progress**

This project will be completed step by step, starting with prompt selection, response collection, evaluation ontology design, evaluation guidelines, and a small carefully reviewed sample of AI response annotations.
