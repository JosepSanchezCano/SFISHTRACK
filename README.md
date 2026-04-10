# FISHTRACK
A high-quality underwater video dataset for fish segmentation and multi-object tracking, featuring pixel-level annotations, temporally consistent identities, and structured metadata from diverse marine environments in the Balearic Sea. Designed for benchmarking and developing underwater computer vision methods. 

# FISHTRACK Dataset

## Overview

FISHTRACK is a curated underwater video dataset designed for **fish segmentation and multi-object tracking** in natural marine environments. It provides pixel-level instance segmentation masks and temporally consistent identities for each fish, supporting research in computer vision, marine ecology, environmental monitoring, and autonomous underwater systems. fileciteturn0file0

The dataset was collected in the **Balearic Sea (Mediterranean region, Spain)** between 2021 and 2025 and captures a wide range of real-world underwater conditions, including variations in lighting, turbidity, depth, background complexity, and species diversity.

---

## Dataset Characteristics

The dataset is designed as a research-grade benchmark resource with the following characteristics:

* Pixel-level instance segmentation for all visible fish
* Temporally consistent object identities across frames
* Multi-object tracking support
* High-resolution underwater imagery
* Structured and standardized metadata
* COCO-compliant annotation format
* Designed for reproducible benchmarking and method evaluation

---

## Directory Structure

```
dataset/
├── videos/
│   ├── video_001.mp4
│   ├── video_002.mp4
│   └── ...
├── frames/
│   ├── video_001/
│   │   ├── frame_000001.jpg
│   │   ├── frame_000002.jpg
│   │   └── ...
│   └── ...
├── annotations/
│   ├── video_001.json
│   ├── video_002.json
│   └── ...
├── metadata/
│   ├── video_001.json
│   ├── video_002.json
│   └── ...
└── README.md
```

---

## Annotations

Annotations follow the **COCO JSON standard** and include:

* Instance segmentation masks (polygon format)
* Bounding boxes
* Object identifiers for tracking
* Frame indices
* Image references
* Class labels (currently a single class: `fish`)

Each video sequence is associated with a dedicated annotation file and a corresponding metadata file.

---

## Metadata

Each recording includes structured metadata such as:

* Recording date and local time
* Recording depth
* Camera model
* Approximate geographic location
* Environmental and deployment context

Metadata are provided in structured JSON format to support interoperability and reproducibility.

---

## Intended Use

The dataset is suitable for research and development in the following areas:

* Fish detection, segmentation, and tracking
* Multi-object tracking (MOT)
* Underwater computer vision
* Marine biodiversity monitoring
* Autonomous underwater robotics
* Model robustness and domain adaptation

---

## Annotation Pipeline

Annotations were produced using a semi-automatic pipeline integrating:

* The Segment Anything Model (SAM2) for instance segmentation
* Cutie for temporal mask propagation
* Manual expert validation and correction
* Multi-stage quality control and cross-review procedures

An open-source, browser-based annotation platform is provided to ensure reproducibility and facilitate future dataset extension.

The Dataset can be downloaded at: BLANK (removed link due to fixing some issues with the download link)


