# Project 02 — Structured Human Knowledge

## Teaching AI to Understand Text, Claims & Evidence

### Core Idea

AI needs structured language data to understand not only words, but also entities, claims, evidence, and question-answer relationships.

This project demonstrates how raw text can be transformed into structured knowledge data that supports annotation, evaluation, and reasoning.

> **Raw Text → Structured Language Annotations → Quality-Controlled Knowledge Data**

### Main Modality

**Text**

### Main Tasks

* Named Entity Recognition (NER)
* BIO tagging
* Text classification
* Claim identification
* Evidence identification
* Question answering
* Annotation quality control

### Main Tools

* Doccano
* Prodigy

### Main Formats / Concepts

* CoNLL
* SQuAD-style question answering

---

## 1. Objective

The objective of this project is to transform raw text into structured information that can support AI training and evaluation.

The project focuses on identifying entities, classifying text, connecting claims to evidence, and creating question-answer data in a consistent and high-quality format.

---

## 2. Role in the Overall Portfolio

This project represents the portfolio's knowledge-understanding layer.

It demonstrates the ability to help AI systems answer:

> **What does this text mean?**

It also supports the broader portfolio goal of organizing human knowledge into structured, verifiable forms that can be used for reliable AI systems.

---

## 3. Dataset

> **Dataset details will be finalized after selecting the exact public dataset or dataset subset for this project.**

This section should document:

* Dataset name
* Original source
* Dataset URL
* Number of documents or text samples selected
* Selection criteria
* License
* Permitted usage
* What I personally annotated
* What I modified
* What I publish publicly

### Planned dataset requirements

The dataset should be:

* publicly available
* legally usable for portfolio work
* small enough to annotate carefully
* suitable for text annotation tasks
* appropriate for public GitHub publication, at least in sample form

### Dataset notes

* I will only use data that can be used responsibly under the dataset’s license.
* I will document the source and licensing terms clearly.
* I will publish only selected samples and demonstrations if the full dataset should not be redistributed.

---

## 4. Annotation Ontology

The annotation ontology defines what can be annotated and how the categories are organized.

### Example ontology

```text
ENTITY
├── PERSON
├── ORGANIZATION
├── LOCATION
├── EVENT
├── DATE
├── CONCEPT
└── WORK

CLAIM
├── FACTUAL
├── OPINION
├── INTERPRETATION
├── PREDICTION
└── UNCERTAIN

EVIDENCE
├── SUPPORTS
├── CONTRADICTS
└── INSUFFICIENT
```

### Class documentation

Each class should include:

* Definition
* Inclusion criteria
* Exclusion criteria
* Examples
* Ambiguous cases

### Notes

The ontology should stay small, clear, and consistent.

The goal is to create a practical annotation system that can be applied reliably, not an overly complex label set.

---

## 5. Annotation Guidelines

The annotation guidelines explain exactly how annotations should be created.

### The guidelines should cover:

* How to identify entity boundaries
* How to assign entity types
* How to apply BIO tags consistently
* How to recognize factual claims
* How to distinguish claims from opinions and interpretations
* How to identify supporting or contradicting evidence
* How to create question-answer pairs
* How to handle ambiguous cases

### Example rules

* Label only entities that are clearly and directly supported by the text.
* Keep entity boundaries as precise as possible.
* Use BIO tags consistently across the dataset.
* Mark a sentence as a factual claim only when it states something that can be checked.
* Do not label unsupported assumptions as evidence.
* When an answer depends on a specific span of text, mark that span clearly.
* If a case is too ambiguous, follow the project’s resolution rule instead of guessing.

The guidelines are designed to promote consistency, accuracy, and reproducibility throughout the annotation process.

---

## 6. Annotation Workflow

```text
Dataset Selection
        ↓
Data Inspection
        ↓
Ontology Definition
        ↓
Annotation Guidelines
        ↓
Initial Annotation
        ↓
Second-Pass Review
        ↓
Error Correction
        ↓
Quality Control
        ↓
Export
        ↓
Format Validation
```

### Workflow explanation

1. Select a small public text dataset.
2. Inspect the text samples and decide what should be annotated.
3. Define the annotation ontology.
4. Write clear annotation guidelines.
5. Perform the initial annotations in the selected tool.
6. Review the annotations a second time.
7. Correct inconsistencies and errors.
8. Run quality control checks.
9. Export the final structured data.
10. Validate the exported format.

---

## 7. Quality Control

The quality-control process focuses on identifying and correcting annotation issues before the data is considered complete.

### Quality-control checks

* Incorrect entity boundaries
* Wrong entity labels
* BIO tagging inconsistencies
* Missing entities
* Incorrect claim labels
* Unsupported evidence links
* Question-answer mismatches
* Duplicate annotations
* Ambiguous cases
* Other text annotation errors

### QA methods

* QA checklist
* Error taxonomy
* Sample annotation errors
* Before/after corrections
* Final quality summary

### Example error types

```text
Wrong entity type
Missing entity
Boundary too wide
Boundary too narrow
BIO tag inconsistency
Incorrect claim category
Evidence not supported by text
Question-answer mismatch
```

---

## 8. Results

> **Results will be added after annotation and QA are completed.**

This section should report:

* Number of documents
* Number of sentences
* Number of entities
* Number of entity categories
* Number of claims
* Number of evidence links
* Number of questions and answers
* Number of QA corrections
* Common error types
* Final quality observations

### Placeholder result format

```text
Documents annotated: [to be added]
Sentences annotated: [to be added]
Entities labeled: [to be added]
Claims labeled: [to be added]
Questions created: [to be added]
QA corrections: [to be added]
Most common issue: [to be added]
Final observation: [to be added]
```

---

## 9. Examples

This section will include representative examples showing the full annotation process.

### Planned examples

* Raw text
* Entity annotation
* BIO tagging example
* Claim classification example
* Evidence annotation example
* Question-answer example
* Before/after QA example

### Example file locations

```text
screenshots/
├── raw-text-example.png
├── doccano-annotation.png
├── prodigy-annotation.png
├── qa-review.png
└── before-after-correction.png
```

The goal is to show not only the final output, but also the annotation and review process itself.

---

## 10. Exported Data

Representative samples of the exported data will be provided here.

### Expected export contents

* CoNLL-style BIO sample
* JSON representation
* SQuAD-style sample
* Claim/evidence sample
* Entity mapping

### Example export files

```text
sample-output/
├── sample-conll.txt
├── sample-squad.json
└── sample-claims.json
```

If the full dataset should not be published publicly, only selected samples and demonstrations will be shared.

This allows others to evaluate the work while keeping control over the complete project assets.

---

## 11. Skills Demonstrated

* Text annotation
* Named Entity Recognition (NER)
* BIO tagging
* CoNLL-style data
* Text classification
* Claim annotation
* Evidence identification
* Question answering
* SQuAD-style data
* Annotation ontology design
* Annotation guideline development
* Structured knowledge preparation
* Quality assurance
* Error analysis
* Critical reasoning
* Text data workflows

---

## 12. Tools

* Doccano
* Prodigy

---

## Project Status

**In progress**

This project will be completed step by step, starting with dataset selection, ontology design, annotation guidelines, and a small carefully reviewed sample of text annotations.
