---
layout: page
permalink: /annotations/
title: Annotations
description:
nav: true
nav_order: 3
---

The annotations include 85,803 manually annotated audio events covering common English filler-word and non-filler-word events. We also provide automatically-generated speech transcripts from a speech-to-text system, which do not contain the manually annotated events.

### Full label vocabulary
Each of the 85,803 manually annotated events is labeled as one of 5 filler classes or 8 non-filler classes (label: number of events).

Fillers
- Uh: 17,907
- Um: 17,078
- You know: 668
- Other: 315
- Like: 157

Non-fillers
- Words: 12,709
- Repetitions: 9,024
- Breath: 8,288
- Laughter: 6,623
- Music : 5,060
- Agree (agreement sounds, e.g., “mm-hmm”, “ah-ha”): 3,755
- Noise : 2,735
- Overlap (overlapping speakers): 1,484

Total: 85,803 

### Consolidated label vocabulary
76,689 of the audio events are also labeled with a smaller, consolidated vocabulary with 6 classes. The consolidated vocabulary was obtained by removing classes with less than 5,000 annotations (like, you know, other, agreement sounds, overlapping speakers, noise), and grouping “repetitions” and “words” into “words”.

- Words: 21,733
- Uh: 17,907
- Um: 17,078
- Breath: 8,288
- Laughter: 6,623
- Music : 5,060

Total: 76,689

The consolidated vocabulary was used to train [FillerNet](https://arxiv.org/abs/2203.15135). For a detailed description of how the dataset was created, please see our paper.


## Data Split for Machine Learning:
To facilitate  machine learning experiments, the audio data in this dataset (full-length recordings and preprocessed 1-sec clips) are pre-arranged into “train”, “validation”, and “test” folders. This split ensures that episodes from the same podcast show are always in the same subset (train, validation, or test), to prevent speaker leakage. We also ensured that each subset in this split remains gender balanced, same as the complete dataset.

We strongly recommend using this split in your experiments. It will ensure your results are not inflated due to overfitting, and that they are comparable to the results published in the [FillerNet paper](https://arxiv.org/abs/2203.15135)
