# NAAMII Research Assistant Assignment I – Medical Image Analysis

## Overview

This repository contains the full solution to the NAAMII Research Assistant Assignment I for the Medical Image Analysis track. It includes:

- Bone segmentation from CT scans
- Contour expansion in physical space (mm)
- Randomized mask generation
- Tibial landmark detection

All solutions were implemented using classical image processing (no deep learning).


---

## Tasks Summary

### Task 1.1 – Bone Segmentation
- CT preprocessed with Otsu thresholding, morphological ops
- Tibia and femur extracted using region filtering
- Output: 'original_mask.nii.gz'

### Task 1.2 – Contour Expansion
- Expanded 2mm and 4mm using voxel spacing
- Outputs: 'expanded_2mm.nii.gz', 'expanded_4mm.nii.gz'

### Task 1.3 – Randomized Contour Generation
- Shell between original and 2mm used to generate randomized contours
- Constraint: Within 2mm shell, no shrinkage
- Outputs: 'randomized_1.nii.gz', `randomized_2.nii.gz'

### Task 1.4 – Tibia Landmark Detection
- Medial and lateral lowest tibial points extracted from all 5 masks
- Output: 'tibia_landmarks.txt'


## How to Run

Install dependencies:


pip install -r requirements.txt 
then open the notebook naamii-assignment-i.ipynb

Outputs
All .nii.gz masks and landmark text file are saved in the outputs/ directory.

## Use of AI Tools

ChatGPT was used to assist in structuring the code into modular components and improving documentation clarity. All logic and implementation were developed and validated manually.



