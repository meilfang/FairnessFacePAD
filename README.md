# Fairness in Face Presentation Attack Detection
---
## Note
This is the official repository of the work:   [Fairness in Face Presentation Attack Detection](https://arxiv.org/abs/2209.09035).

## Motivation
The fairness of face PAD is an understudied issue, mainly due to the lack of appropriately annotated data. To address this issue, this work first presents a Combined Attribute Annotated PAD Dataset (CAAD-PAD) by combining several well-known PAD datasets where we provide seven human-annotated attribute labels. This work then comprehensively analyses the fairness of a set of face PADs and its relation to the nature of training data and the Operational Decision Threshold Assignment (ODTA) on different data groups by studying four face PAD approaches on CAAD-PAD. To simultaneously represent both the PAD fairness and the absolute PAD performance, we introduce a novel metric, namely the Accuracy Balanced Fairness (ABF). Extensive experiments on CAAD-PAD show that the training data and ODTA induce unfairness on gender, occlusion, and other attribute groups. Based on these analyses, we propose a data augmentation method, FairSWAP, which aims to disrupt the identity/semantic information and guide models to mine attack cues rather than attribute-related information. Detailed experimental results demonstrate that FairSWAP generally enhances both the PAD performance and the fairness of face PAD.

## Data description
### CAAD-PAD
CAAD-PAD dataset contains annotations covering demographic and non-demographic attributes of six publicly available face PAD datasets: CASIA-FASD, Idiap Replay-Attack, MSU-MFSD, HKBU-MARs, OULU-NPU, and SWFFD.
Specifically, CAAD-PAD provides the following labels: gender, Beard, eyeglasses, bangs, makeup, Long/short hair, Curly/straight hair. CAAD-PAD can be downloaded via [Google drive](https://drive.google.com/file/d/1Ko_n0V09nDG8FdEvks4mi5kgb_gmLYyV/view?usp=share_link).
For using face PAD data (images/videos) in each dataset, please download the data from their official webpages.

## To-do
- [ ] Add FairSWAP and scripts

## Citation
if you use CAAD-PAD dataset, please cite the following paper:
```
@article{DBLP:journals/corr/abs-2209-09035,
  author    = {Meiling Fang and
               Wufei Yang and
               Arjan Kuijper and
               Vitomir Struc and
               Naser Damer},
  title     = {Fairness in Face Presentation Attack Detection},
  journal   = {CoRR},
  volume    = {abs/2209.09035},
  year      = {2022}
}
```

## License
The implementation or trained models use is restricted to research purpuses. The use of the implementation/trained models for product development or product competetions (incl. NIST FRVT MORPH) is not allowed. This project is licensed under the terms of the Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) license. Copyright (c) 2020 Fraunhofer Institute for Computer Graphics Research IGD Darmstadt.
