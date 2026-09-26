# Knee Osteoarthritis Detection and Severity Classification — YOLOv4-tiny

This repository contains the trained model weights, Darknet configuration files, and dataset split lists used in the study:

**"Automatic Knee Osteoarthritis Detection and Severity Classification from Radiographs Using YOLOv4-tiny"**
(Manuscript ID: JDH-703, Journal of Digital Health)

## Contents

- `custom-yolov4-tiny-detector_best.weights` — trained model weights (best validation-mAP checkpoint)
- `*.cfg` — Darknet network configuration file
- `*.data` — Darknet data configuration file
- `obj.names` — class label names (Normal, Doubtful, Mild, Moderate, Severe)
- Split list files — image filenames used in the training, validation, and test partitions

## Dataset

The source dataset is publicly available on Mendeley Data:
Gornale, S. & Patravali, P. (2020). *Digital Knee X-ray Images*, V1.
DOI: [10.17632/t9ndx37v5h.1](https://doi.org/10.17632/t9ndx37v5h.1)
License: CC BY 4.0

## Method summary

The 1,633 deduplicated source radiographs were partitioned 70/20/10 by class into training, validation, and test subsets **before** augmentation (split-then-augment protocol), to prevent data leakage between partitions. Only the training subset was subsequently augmented. Full methodology is described in the manuscript, Section 3.

## Citation

If you use these files, please cite the associated manuscript (citation details to be added upon publication).

## License

These files are provided for research reproducibility purposes, consistent with the CC BY 4.0 license of the source dataset.
