# PoseRadAI — Intelligent Patient Positioning Assistant for Radiography

> **Real-time AI feedback system that ensures correct patient positioning before the X-ray is taken**

[![Demo](https://img.shields.io/badge/▶%20Watch%20Demo-Google%20Drive-blue)](https://drive.google.com/file/d/1wM-sg9_asprKQrKb5Oos74z1a1EOTKvs/view)
[![CPU Only](https://img.shields.io/badge/Deployment-CPU%20Only-orange)]()
[![Real-time](https://img.shields.io/badge/Processing-Real--time-brightgreen)]()
[![Python](https://img.shields.io/badge/Python-3.8+-yellow)]()

---

## The Clinical Problem

A chest X-ray is only as good as the positioning of the patient when it is taken.

Poor patient positioning — even subtle tilts, shoulder asymmetry, or rotational errors — leads to:
- **Diagnostic inaccuracies**: Structures appear distorted, making findings unreliable
- **Repeated exposures**: Patients receive unnecessary radiation when images must be retaken
- **Missed pathology**: Positioning errors can mask or mimic real findings
- **Training gaps**: In Africa, radiography departments are understaffed and supervising juniors is difficult

In Nigerian hospitals, where one senior radiographer may oversee multiple junior staff simultaneously, there is no practical way to manually verify every patient's positioning before every exposure.

**PoseRadAI solves this by being the always-present, always-alert positioning supervisor.**

---

## What It Does

PoseRadAI uses a standard camera to watch the patient in real time and evaluates:

| Check | What It Detects |
|-------|----------------|
| **Shoulder Symmetry** | Detects if shoulders are uneven or rotated |
| **Spinal Alignment** | Checks midline alignment of the spine |
| **Tilt Detection** | Identifies lateral tilt of head or torso |
| **Obliquity** | Detects rotational positioning errors |
| **Cassette Alignment** | Verifies the X-ray plate is correctly positioned |
| **Light Field Check** | Confirms the X-ray beam is correctly collimated |

The system provides instant visual feedback — **green means ready, red means reposition** — before the exposure button is pressed.

---

## Why This Matters

This is not just a quality tool. It is a **training tool**.

In environments where:
- Radiography students are learning with limited supervision
- Patient throughput is high and supervision time is limited
- Equipment errors are common and quality assurance is manual

PoseRadAI enables **safe, feedback-driven training** — students learn correct positioning in real time without compromising patient care or diagnostic quality.

---

## Technical Approach

- **Pose Detection:** MediaPipe Pose — Google's real-time human pose estimation framework
- **Object Detection:** YOLOv8 — for cassette and equipment detection
- **Processing:** Real-time inference on CPU — no GPU required
- **Interface:** Live camera feed with overlay feedback
- **Deployment:** Runs on any standard Windows/Linux laptop

---

## Clinical Context

Built by a practicing radiographer who has personally experienced the consequences of poor positioning in a busy Nigerian hospital department — and designed the solution to work within those exact constraints.

---

## Demo

[▶ Watch PoseRadAI in action](https://drive.google.com/file/d/1wM-sg9_asprKQrKb5Oos74z1a1EOTKvs/view?usp=drive_link)

---

## Built By

**Ephraim Usani** — First-Class Radiographer & Clinical AI Engineer, Lagos, Nigeria

[LinkedIn](https://www.linkedin.com/in/ephraim-usani) | [GitHub](https://github.com/Ephraim-Usani)

> *"In many ways, this is my attempt to bring AI-guided imaging assistance into radiography — ensuring every patient gets a diagnostic-quality image, regardless of who positions them."*
