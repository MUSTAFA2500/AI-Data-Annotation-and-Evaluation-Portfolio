Project 03 — Multimodal Understanding
Teaching AI to Understand Audio & Video
Core idea

The world is not only text and images.

AI systems must also understand:

Sounds
Speech
Events
Actions
Temporal relationships
Main modalities

Audio + Video

Main tools
Label Studio
CVAT
Prodigy
Main format/concept
AudioSet ontology
1. Objective

Demonstrate the ability to transform raw audio and video into structured data representing events, objects, actions, and temporal information.

2. Role in the Overall Portfolio

This is the portfolio's multimodal perception layer.

It expands the portfolio from:

Seeing

and

Reading

to:

Hearing and understanding events over time.

3. Dataset

Document separately:

Audio
Dataset
Source
License
Audio format
Number of clips
Video
Dataset
Source
License
Video format
Number of clips

All publicly displayed materials should respect the original dataset licenses.

4. Annotation Ontology
Audio
Speech
Music
Human Sound
Animal Sound
Vehicle Sound
Environmental Sound
Mechanical Sound
Other
Video
PERSON
VEHICLE
OBJECT
ANIMAL

ACTIONS
├── Walking
├── Running
├── Picking Up
├── Opening
└── Entering

EVENTS
├── Person Enters
├── Object Interaction
└── Person Leaves

The audio categories can be mapped conceptually to relevant AudioSet ontology classes where appropriate.

5. Annotation Guidelines

Define:

Audio event boundaries
Overlapping sounds
Multiple simultaneous events
Video frame boundaries
Object tracking rules
Action definitions
Event start/end points
Occlusion
Ambiguous events
6. Annotation Workflow
Raw Audio / Video
        ↓
Data Inspection
        ↓
Ontology Definition
        ↓
Audio Annotation
        ↓
Video Annotation
        ↓
Temporal Annotation
        ↓
Tracking / Event Linking
        ↓
QA Review
        ↓
Structured Export
7. Quality Control

Check:

Incorrect audio labels
Incorrect temporal boundaries
Missing events
Incorrect object tracks
Broken tracks
Inconsistent action labels
Ambiguous cases
8. Results

Report:

Audio clips
Video clips
Audio events
Video objects
Actions
Temporal events
Tracking annotations
QA corrections
9. Examples

Show:

Audio waveform + labels
Video frame + annotations
Temporal event timeline
Object tracking example
Before/after QA correction
10. Exported Data

Show representative examples of:

Audio event labels
Temporal annotations
Video annotations
Tracking data
Structured JSON
11. Skills Demonstrated
Audio annotation
Video annotation
Temporal annotation
Event detection
Object tracking
Multimodal annotation
AudioSet ontology familiarity
Quality assurance
12. Tools
Label Studio
CVAT
Prodigy
--------------
# 03 — Multimodal Understanding

### *Teaching AI to Understand the World Through Audio & Video*

**Focus:** Audio and video annotation.

The goal is to transform information from sound and moving images into structured multimodal data.

## Audio

### Tasks

* [ ] Audio classification
* [ ] Sound event identification
* [ ] Temporal audio annotation
* [ ] Speech labeling
* [ ] Environmental sound labeling

### Reference

* `AudioSet` ontology

## Video

### Tasks

* [ ] Object annotation
* [ ] Object tracking
* [ ] Action annotation
* [ ] Event identification
* [ ] Temporal annotation

### Tools

* `Label Studio`
* `CVAT`
* `Prodigy`

### Workflow

```text
Raw Audio / Video
        │
        ▼
Identify Objects & Events
        │
        ▼
Add Temporal Annotations
        │
        ▼
Review Annotation Quality
        │
        ▼
Structured Multimodal Data
```

### Portfolio Evidence

* Audio annotation examples
* Video annotation examples
* Temporal annotation examples
* Object tracking examples
* AudioSet ontology mapping
* Label Studio screenshots
* CVAT screenshots
* Prodigy screenshots
* QA report
