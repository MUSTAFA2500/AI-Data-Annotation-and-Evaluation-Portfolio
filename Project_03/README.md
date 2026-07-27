# Project 03 — Multimodal Understanding

## Teaching AI to Understand Audio & Video

### Core Idea

AI needs structured multimodal data to understand events, actions, sounds, and changes over time.

This project demonstrates how raw audio and video can be transformed into structured annotations and then into quality-controlled training data.

> **Raw Audio & Video → Structured Multimodal Annotations → Quality-Controlled Training Data**

### Main Modalities

**Audio + Video**

### Main Tasks

* Audio classification
* Sound event identification
* Temporal audio annotation
* Speech labeling
* Environmental sound labeling
* Object annotation
* Object tracking
* Action annotation
* Event identification
* Temporal annotation

### Main Tools

* Label Studio
* CVAT
* Prodigy

### Main Formats / Concepts

* AudioSet ontology
* Video annotation and tracking workflows

---

## 1. Objective

The objective of this project is to transform raw audio and video into structured, high-quality annotations that can support AI training and evaluation.

The project focuses on identifying sounds, events, objects, actions, and temporal relationships in multimodal data using clear annotation rules and quality control.

---

## 2. Role in the Overall Portfolio

This project represents the portfolio's multimodal perception layer.

It demonstrates the ability to help AI systems answer:

> **What is happening in the world, and how can it be represented across sound and video?**

It expands the portfolio beyond text and images by showing practical skills in audio annotation, video annotation, temporal labeling, and multimodal data preparation.

---

## 3. Dataset

> **Dataset details will be finalized after selecting the exact public audio and video dataset or dataset subset for this project.**

This section should document:

* Dataset name
* Original source
* Dataset URL
* Number of audio clips selected
* Number of video clips selected
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
* suitable for audio and video annotation tasks
* appropriate for public GitHub publication, at least in sample form

### Dataset notes

* I will only use data that can be used responsibly under the dataset’s license.
* I will document the source and licensing terms clearly.
* I will publish only selected samples and demonstrations if the full dataset should not be redistributed.

---

## 4. Annotation Ontology

The annotation ontology defines what can be annotated and how the categories are organized.

### Example audio ontology

```text
Speech
Music
Human Sound
Animal Sound
Vehicle Sound
Environmental Sound
Mechanical Sound
Other
```

### Example video ontology

```text
Person
Vehicle
Object
Animal

Actions
├── Walking
├── Running
├── Picking Up
├── Opening
└── Entering

Events
├── Person Enters
├── Object Interaction
└── Person Leaves
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

* How to identify audio event boundaries
* How to handle overlapping sounds
* How to label speech and non-speech audio
* How to define temporal segments
* How to identify objects in video frames
* How to track objects across frames
* How to annotate actions and events
* How to handle occlusion
* How to handle ambiguous audio or video cases

### Example rules

* Label only audio events that are clearly audible.
* Mark the start and end of each sound event as precisely as possible.
* If multiple sounds overlap, label each clearly identifiable sound.
* Label only video objects that are clearly visible enough to identify.
* Track objects consistently across frames when the same object remains visible.
* If an event is too unclear to identify, do not guess.
* If a case is ambiguous, follow the project’s resolution rule instead of inventing a label.

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

1. Select a small public audio and video dataset.
2. Inspect the samples and decide what should be annotated.
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

* Incorrect audio labels
* Incorrect temporal boundaries
* Missing sound events
* Overlapping sounds not labeled correctly
* Incorrect object labels
* Broken object tracks
* Inconsistent action labels
* Missing video events
* Ambiguous cases
* Other multimodal annotation errors

### QA methods

* QA checklist
* Error taxonomy
* Sample annotation errors
* Before/after corrections
* Final quality summary

### Example error types

```text
Wrong sound label
Missing sound event
Boundary too wide
Boundary too narrow
Incorrect object label
Broken track
Incorrect action label
Event start/end mismatch
```

---

## 8. Results

> **Results will be added after annotation and QA are completed.**

This section should report:

* Number of audio clips
* Number of video clips
* Number of audio events
* Number of video objects
* Number of actions
* Number of temporal annotations
* Number of object tracks
* Number of QA corrections
* Common error types
* Final quality observations

### Placeholder result format

```text
Audio clips annotated: [to be added]
Video clips annotated: [to be added]
Audio events labeled: [to be added]
Video objects labeled: [to be added]
Actions labeled: [to be added]
Tracks created: [to be added]
QA corrections: [to be added]
Most common issue: [to be added]
Final observation: [to be added]
```

---

## 9. Examples

This section will include representative examples showing the full annotation process.

### Planned examples

* Raw audio clip with labels
* Raw video frame with annotations
* Temporal audio event example
* Object tracking example
* Action annotation example
* Before/after QA example

### Example file locations

```text
screenshots/
├── raw-audio-example.png
├── audio-annotation.png
├── raw-video-frame.png
├── cvat-video-annotation.png
├── label-studio-audio.png
├── tracking-example.png
└── before-after-correction.png
```

The goal is to show not only the final output, but also the annotation and review process itself.

---

## 10. Exported Data

Representative samples of the exported data will be provided here.

### Expected export contents

* Audio event labels
* Temporal annotations
* Video annotations
* Object tracking data
* Structured JSON samples

### Example export files

```text
sample-output/
└── sample-annotations.json
```

If the full dataset should not be published publicly, only selected samples and demonstrations will be shared.

This allows others to evaluate the work while keeping control over the complete project assets.

---

## 11. Skills Demonstrated

* Audio annotation
* Video annotation
* Temporal annotation
* Sound event identification
* Object tracking
* Action annotation
* Multimodal annotation
* Structured data preparation
* Annotation ontology design
* Annotation guideline development
* Quality assurance
* Error analysis
* Multimodal data workflows
* Audio and video label consistency
* Event and boundary reasoning

---

## 12. Tools

* Label Studio
* CVAT
* Prodigy

---

## Project Status

**In progress**

This project will be completed step by step, starting with dataset selection, ontology design, annotation guidelines, and a small carefully reviewed sample of audio and video annotations.
