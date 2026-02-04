# Neural Correlates of Visual Memorability (7T fMRI)

This repository contains the computational pipeline used to investigate how the human brain represents **visual memorability**—an intrinsic stimulus property predicting how likely an image is to be remembered. By applying **Multivariate Pattern Analysis (MVPA)** and **Representational Similarity Analysis (RSA)** to high-resolution **7-Tesla fMRI data**, this project maps the transformation of neural representations from encoding to recall.

For a detailed walkthrough of the theoretical background, methodology, and results of this analysis, please refer to the Final Project Report.

## 🧠 Project Overview

While memorability is a stable, content-driven characteristic of images, its neural signature during active recall remains less understood than during initial encoding. This project explores:

* **Encoding vs. Recall:** How representational resolution for memorability-predictive features changes between initial perception and later memory retrieval.
* **Cortical Localization:** Identifying the specific roles of object-selective (LO, PFS), scene-selective (PPA, RSC, OPA), and hippocampal regions in maintaining these representations.

## 💻 Technical Implementation

* **Dataset:** High-resolution fMRI data from 22 participants scanned at 7-Tesla during a visual memory task involving 192 stimulus images.
* **Decoding (MVPA):** Implemented ROI-based multivariate decoding to classify high vs. low memorability levels from voxel-wise activation patterns.
* **Representational Similarity Analysis (RSA):** Constructed brain-based Representational Dissimilarity Matrices (RDMs) and correlated them with memorability-based models to assess second-order isomorphism.
* **Regions of Interest (ROIs):** Analysis performed on localized masks including the Early Visual Cortex (EVC), Ventral Temporal Cortex (LO, PFS), Scene Areas (PPA, RSC, OPA), and Hippocampal subfields (PRC, DG, CA1, CA3).

## 📈 Key Findings

* **Distributed Encoding:** Significant decoding of memorability was found across all high-level visual ROIs (e.g., LO, PFS, PPA, RSC) during the encoding phase.
* **Recall Diminution:** Representational accuracy significantly decreased during recall, with medial temporal lobe (MTL) regions failing to show significant memorability decoding during this phase.
* **Model Alignment:** RSA revealed that neural representations in object and scene areas align closely with memorability models during encoding, but this alignment is largely lost during active retrieval.

## 🛠️ Tools Used

* **Analysis:** Python / MATLAB
* **Neuroimaging:** fMRI (7-Tesla)
* **Techniques:** MVPA, RSA, Signal Detection Theory (SDT)

## 📊 Data Availability
The neuroimaging and behavioral data analyzed in this repository were provided by Dr. Wilma Bainbridge for research and educational purposes.

Per the request of the first author, the raw and processed data are not publicly available for redistribution to ensure data privacy and adherence to original sharing agreements.

For those interested in the original dataset or seeking to replicate these findings, please refer to the primary publication:

Bainbridge, W.A., Hall, E.H., & Baker, C.I. (2021). Distinct representational structure and localization for visual encoding and recall during visual imagery. Cerebral Cortex.
