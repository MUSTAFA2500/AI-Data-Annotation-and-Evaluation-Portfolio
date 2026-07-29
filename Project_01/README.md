# Project 01 — Visual Knowledge

## Teaching AI to See the World

### Core Idea

AI needs structured visual data to learn about the physical world.

This project demonstrates how raw images can be transformed into structured visual annotations and then into quality-controlled training data.

> **Raw Images → Structured Visual Annotations → Quality-Controlled Training Data**

### Main Modality

**Image**

### Main Tasks

* Object detection
* Bounding boxes
* Polygon annotation
* Semantic segmentation
* Instance segmentation
* Image classification

### Main Tools

* Labelbox
* CVAT

### Main Formats / Concepts

* COCO
* ImageNet concepts

---

## 1. Objective

The objective of this project is to transform raw visual data into structured, high-quality annotations that can support computer vision model training and evaluation.

The project focuses on accurately identifying and labeling objects and regions within real-world images using clear annotation rules and quality control.

---

## 2. Role in the Overall Portfolio

This project represents the visual perception layer of the portfolio.

It demonstrates the ability to help AI systems answer:

> **What is present in the visual world?**

It provides the foundation for working with image data and demonstrates practical skills in computer vision annotation, structured data preparation, and quality control.

---

## 3. Dataset

> **Dataset details will be finalized after selecting the exact public dataset or dataset subset for this project.**

This section should document:

* Dataset name
* Original source
* Dataset URL
* Number of images selected
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
* suitable for image annotation tasks
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

Person
├── adult
├── Teenager
└── child

Vehicle
├── Car
├── Bus
├── Bike
└── Motorcycle

Animal
├── Cat
└── Dog

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

* When an object should be labeled
* How bounding boxes should be drawn
* How to handle partially visible objects
* How to handle overlapping objects
* How to handle occlusion
* How to handle truncated objects
* When to use polygons
* When to use segmentation
* How to handle ambiguous cases

### Example rules

* Label only objects that are clearly visible.
* Draw bounding boxes tightly around the visible part of the object.
* If an object is partially occluded, label the visible portion only.
* If an object is too unclear to identify, do not label it.
* Use polygons only when the object shape requires more precision than a bounding box.

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

1. Select a small public dataset.
2. Inspect the images and decide which objects should be annotated.
3. Define the annotation ontology.
4. Write clear annotation guidelines.
5. Perform the initial annotations.
6. Review the annotations a second time.
7. Correct errors and inconsistencies.
8. Run quality control checks.
9. Export the final structured data.
10. Validate the exported format.

---

## 7. Quality Control

The quality-control process focuses on identifying and correcting annotation issues before the data is considered complete.

### Quality-control checks

* Annotation inconsistencies
* Missing annotations
* Incorrect labels
* Poorly placed bounding boxes
* Incorrect segmentation
* Duplicate annotations
* Ambiguous cases
* Other annotation errors

### QA methods

* QA checklist
* Error taxonomy
* Sample annotation errors
* Before/after corrections
* Final quality summary

### Example error types

```text
Wrong class label
Missing object
Bounding box too loose
Bounding box too tight
Duplicate annotation
Unclear ambiguous case
Incorrect segmentation boundary
```

---

## 8. Results

> **Results will be added after annotation and QA are completed.**

This section should report:

* Number of images
* Number of annotations
* Number of classes
* Types of annotations
* Number of QA corrections
* Common error types
* Final quality observations

### Placeholder result format

```text
Images annotated: [to be added]
Total annotations: [to be added]
Classes used: [to be added]
QA corrections: [to be added]
Most common issue: [to be added]
Final observation: [to be added]
```

---

## 9. Examples

This section will include representative examples showing the full annotation process.

### Planned examples

* Raw image
* Annotated image
* Incorrect annotation
* Corrected annotation
* Complex or ambiguous example
* Before/after QA example

### Example file locations

```text
screenshots/
├── raw-image.png
├── labelbox-annotation.png
├── cvat-annotation.png
├── qa-review.png
└── before-after-correction.png
```

The goal is to show not only the final output, but also the annotation and review process itself.

---

## 10. Exported Data

Representative samples of the exported data will be provided here.

### Expected export contents

* COCO JSON
* Annotation schema
* Class mapping
* Sample structured annotations

### Example export files

```text
sample-output/
└── sample-coco.json
```

If the full dataset should not be published publicly, only selected samples and demonstrations will be shared.

This allows others to evaluate the work while keeping control over the complete project assets.

---

## 11. Skills Demonstrated

* Image annotation
* Object detection
* Bounding boxes
* Polygon annotation
* Semantic segmentation
* Instance segmentation
* Image classification
* Annotation ontology design
* Annotation guideline development
* Structured data preparation
* Quality assurance
* Error analysis
* COCO format
* Computer vision data workflows

---

## 12. Tools

* Labelbox
* CVAT

---

## Project Status

**In progress**

This project will be completed step by step, starting with dataset selection, ontology design, annotation guidelines, and a small carefully reviewed sample of image annotations.
