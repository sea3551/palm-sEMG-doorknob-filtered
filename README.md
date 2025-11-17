# palm-sEMG-doorknob-filtered


This repository releases palm surface EMG (sEMG) recordings collected during doorknob-rotation actions.  
Data are minimally preprocessed to support reproducible research.

---

# What's included
- `data/` — CSV data files
- `LICENSE` — Data license (CC BY 4.0)
- `README.md` — This document

# Preprocessing (minimal)
- 60 Hz notch filtering (power-line interference removal)
- 20–500 Hz band-pass filtering (muscle activity band)
- Otherwise untouched: no resampling, trimming, segmentation, or relabeling

# Data summary
- Subjects: 5
- Channels: 2; Ground: ulnar styloid
-   Column 1 → Comp Ch 3 = Channel 1 (APB)
-   lumn 2 → Comp Ch 4 = Channel 2 (ADM)
- Sampling rate: 1000 Hz
- Task: grasp (1s) → rotate (1s) → stop (1s) = 3 s per trial
- Trials: 50 per subject
