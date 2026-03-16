# AUPAD
Hybrid Knowledge Distillation for Zero-Shot Anomaly Detection
# Introduction
This is the official data link of AUPAD
# datasets

Industrial Visual Anomaly Detection Datasets:

MVTec AD https://drive.google.com/file/d/12IukAqxOj497J4F0Mel-FvaONM030qwP/view?usp=drive_link

VisA https://drive.google.com/file/d/1U0MZVro5yGgaHNQ8kWb3U1a0Qlz4HiHI/view?usp=drive_link

MPDD https://drive.google.com/file/d/1cLkZs8pN8onQzfyNskeU_836JLjrtJz1/view?usp=drive_link

BTAD https://drive.google.com/file/d/19Kd8jJLxZExwiTc9__6_r_jPqkmTXt4h/view?usp=drive_link

KSDD https://drive.google.com/file/d/13UidsM1taqEAVV_JJTBiCV1D3KUBpmpj/view?usp=drive_link

DTD-Synthetic https://drive.google.com/file/d/1em51XXz5_aBNRJlJxxv3-Ed1dO9H3QgS/view?usp=drive_link

Medical Visual Anomaly Detection Datasets:

HeadCT https://drive.google.com/file/d/1ore0yCV31oLwwC--YUuTQfij-f2V32O2/view?usp=drive_link

BrainMRI https://drive.google.com/file/d/1JLYyzcPG3ULY2J_aw1SY9esNujYm9GKd/view?usp=drive_link

Br35H https://drive.google.com/file/d/1qaZ6VJDRk3Ix3oVp3NpFyTsqXLJ_JjQy/view?usp=drive_link

ISIC https://drive.google.com/file/d/1atZwmnFsz7mCsHWBZ8pkL_-Eul9bKFEx/view?usp=drive_link

ColonDB https://drive.google.com/file/d/1tjZ0o5dgzka3wf_p4ErSRJ9fcC-RJK8R/view?usp=drive_link

ClinicDB https://drive.google.com/file/d/1ciqZwMs1smSGDlwQ6tsr6YzylrqQBn9n/view?usp=drive_link

TN3K https://drive.google.com/file/d/1LuKEMhrUGwFBlGCaej46WoooH89V3O8_/view?usp=drive_link

## AUPAD: Adaptive Unified Prompt Anomaly Detection

Zero-shot anomaly detection (ZSAD) aims to detect anomalies in unseen datasets without any training samples from the target domain. This problem is particularly important in real-world scenarios where collecting labeled anomaly data is difficult due to privacy, cost, or accessibility constraints. However, ZSAD is highly challenging because models must generalize across diverse domains with significant variations in object appearance, abnormal regions, and background patterns.

This repository provides the official implementation of **AUPAD (Adaptive Unified Prompt Anomaly Detection)**, a **one-for-all zero-shot anomaly detection framework** built upon pretrained vision–language models such as CLIP.

### Key Idea

While large vision–language models demonstrate strong zero-shot recognition ability, their anomaly detection performance is often limited because they focus on object semantics rather than normality or abnormality cues. AUPAD addresses this limitation through **instance-adaptive prompt learning**, enabling the model to better capture anomaly semantics.

### Main Features

- **Instance-adaptive prompt generation**  
  Generates adaptive prompts by combining shared semantic vectors with instance-specific tokens to model both normal and abnormal states.


- **Dynamic Region Attention Module (DRAM)**  
  Reduces global attention bias and enhances local semantic consistency without modifying the pretrained encoder.

- **Glocal abnormality learning**  
  Introduces a glocal abnormality loss that jointly captures global and local anomaly characteristics.

### Performance

AUPAD has been extensively evaluated on **17 industrial and medical anomaly detection datasets**, demonstrating strong performance in both **anomaly detection** and **anomaly segmentation** across highly diverse semantic categories.

### Highlights

- One-for-all **zero-shot anomaly detection framework**
- Built on **pretrained vision–language models (CLIP)**
- Strong **cross-domain generalization**
- Effective for **both industrial and medical anomaly detection**
