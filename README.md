# palm-sEMG-doorknob-filtered

Palm sEMG-based user authentication during doorknob rotation using a convolutional neural network
Yeonjung Shin1, Junghun Kim2,*, Sang-Il Choi2,*
1Department of Computer Software, Daegu Catholic University, Gyeongsangbuk-do, 38430, Republic of Korea
2School of Computer Software, Daegu Catholic University, Gyeongsangbuk-do, 38430, Republic of Korea
*fainal2@cu.ac.kr; sangilchoi@cu.ac.kr
<img width="468" height="187" alt="image" src="https://github.com/user-attachments/assets/4f25d8ff-0328-4464-81bb-1b7da3bb5907" />


This repository releases palm surface EMG (sEMG) recordings collected during doorknob-rotation actions.  
Data are minimally preprocessed to support reproducible research.

The data used in this study were collected after obtaining approval from the Institutional Review Board (IRB) of Kyungpook National University Hospital, in accordance with ethical guidelines (IRB number: KNUH 2025). 

## License
Data © 2025 Yeonjung Shin — released under **CC BY 4.0**. See `LICENSE` for the full text.


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
