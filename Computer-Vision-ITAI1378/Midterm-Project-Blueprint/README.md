# Midterm Project – Blueprint

## Overview

This project proposal was developed as the Midterm assignment for **ITAI 1378 – Computer Vision and AI**. The objective was to design a complete blueprint for a computer vision application, including the problem definition, technical approach, dataset plan, evaluation metrics, milestones, and project risks before beginning implementation.

The proposed project, **Meal Ingredient Detection: What's on My Plate?**, focuses on detecting common food ingredients from meal images using object detection.

---

## Project Goal

The goal of this project is to automatically identify common meal ingredients from a photograph. Detecting ingredients can serve as the foundation for applications such as recipe recommendations, meal organization, and nutrition tools by reducing the manual effort required to identify ingredients in food images.

---

## Proposed Solution

The proposed application follows a simple computer vision pipeline:

```text
Meal Image
      ↓
YOLO11 Object Detection
      ↓
Ingredient Detection
      ↓
Annotated Image + Ingredient List + Confidence Scores
```

The system receives a meal image as input and returns an annotated image highlighting the detected ingredients together with their confidence scores.

---

## Technical Approach

- **Computer Vision Technique:** Object Detection
- **Model:** YOLO11
- **Framework:** Ultralytics + PyTorch
- **Development Environment:** Google Colab

YOLO11 was selected for its speed, accuracy, and ability to detect multiple ingredients within a single meal image.

---

## Data Plan

The project proposed using publicly available ingredient detection datasets from **Roboflow Universe** or **Kaggle**. Images would be resized, normalized, and annotated using the YOLO11 bounding-box format before being divided into training, validation, and testing sets.

---

## Success Metrics

The proposed evaluation metrics were:

- **Primary Metric:** mAP50 ≥ 0.70
- **Secondary Metric:** Inference time under 1 second per image

These metrics were selected to balance detection accuracy with real-time performance.

---

## Milestone Plan

The project roadmap consisted of five development phases:

1. Blueprint
2. First Working Demo
3. Make It Yours
4. Improve & Measure
5. Package & Present

Each phase was designed to gradually evolve the project from planning to a complete working computer vision application.

---

## Risks and Resources

The proposal identified two primary risks:

- A suitable ingredient detection dataset may not be available.
- The model may not achieve the expected performance.

The proposed mitigation strategies included selecting an alternative public dataset or reducing the number of ingredient classes to simplify training. The project planned to use **Google Colab** as the development environment with no expected computing cost.

---

## Project Repository

The complete project repository, including the Blueprint documentation and implementation, is available at:

**https://github.com/alissacanesim/meal-ingredient-detection**

---

## Files

- `Midterm_Alissa_Canesim_Bento_ITAI1378.pdf` – Midterm project proposal slides.
