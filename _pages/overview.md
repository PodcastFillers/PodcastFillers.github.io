---
layout: about
title: Home
permalink: /
subtitle:

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

## Overview

The PodcastFillers dataset consists of 199 full-length podcast episodes in English with manually annotated filler words and automatically generated transcripts. The podcast audio recordings, sourced from [SoundCloud](www.soundcloud.com), are CC-licensed, gender-balanced, and total 145 hours of audio from over 350 speakers. The annotations are provided under a [non-commercial license](/license) and consist of 85,803 manually annotated audio events including approximately 35,000 filler words (“uh” and “um”) and 50,000 non-filler events such as breaths, music, laughter, repeated words, and noise. The annotated events are also provided as pre-processed 1-second audio clips. The dataset also includes automatically generated speech transcripts from a speech-to-text system. A detailed description is provided in [Dataset](/dataset).

**The PodcastFillers dataset is available at**: [zenodo](https://zenodo.org/record/6609215#.Ys3IwZPMK3I)\
**The preprocessing utility functions and code repository for reproducing our experimental results**: [PodcastFillersUtils](https://github.com/gzhu06/PodcastFillers_Utils)

## Acknowledgement

Please cite the following paper in work that makes use of this dataset:

[Filler Word Detection and Classification: A Dataset and Benchmark](https://arxiv.org/abs/2203.15135)\
Ge Zhu, Juan-Pablo Caceres and Justin Salamon\
In 23rd Annual Cong. of the Int. Speech Communication Association (INTERSPEECH), Incheon, Korea, Sep. 2022.

### Bibtex
```
@inproceedings{Zhu:FillerWords:INTERSPEECH:22,
  title = {Filler Word Detection and Classification: A Dataset and Benchmark},
  booktitle = {23rd Annual Cong.~of the Int.~Speech Communication Association (INTERSPEECH)},
  address = {Incheon, Korea}, 
  month = {Sep.},
  url = {https://arxiv.org/abs/2203.15135},
  author = {Zhu, Ge and Caceres, Juan-Pablo and Salamon, Justin},
  year = {2022},
}
```
