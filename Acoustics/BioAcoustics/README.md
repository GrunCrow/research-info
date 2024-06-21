# BioAcoustics

Resources on the use of Deep Learning algorithms in the analysis of sounds and vocalizations of wildlife, especially birds.

## Software

### Models

#### [BirdNET](https://github.com/kahst/BirdNET-Analyzer)

#### OpenSoundScape

#### [BirdAVES: Animal Vocalization Encoder based on Self-Supervision](https://github.com/earthspecies/aves?tab=readme-ov-file#birdaves)

AVES (Animal Vocalization Encoder based on Self-Supervision) is a self-supervised, transformer-based audio representation model for encoding animal vocalizations ("BERT for animals"). It is based on HuBERT (Hsu et al., 2021), a powerful self-supervised model for human speech, but pretrained on large-scale unannotated audio datasets (FSD50K, AudioSet, and VGGSound) which include animal sounds.

## Labs

### [Kitzes Lab](https://www.kitzeslab.org/)

- [BioAcoustic Resources](https://docs.google.com/document/d/10APGahxU_GJewO8mkN2wzG0y-LHw3p_TAcYJDdHAQmg/edit#heading=h.mwbyo5325flj)
- [OpenSoundScape](https://github.com/kitzeslab/opensoundscape)

## Papers

### Birds

| Title | Authors | Year | Abstract | Review |
|-------|---------|------|----------|--------|
| [BirdNET: A deep learning solution for avian diversity monitoring](https://www.sciencedirect.com/science/article/pii/S1574954121000273) | Stefan Kahl, Connor M. Wood, Maximilian Eibl, Holger Klinck | 2021 | ... | ... |

#### PAM - Passive Acoustic Monitoring

Papers that are not focused on the use of Deep Learning techniques for Bioacoustics.

| Title | Authors | Year | Abstract | Review |
|-------|---------|------|----------|--------|
| [Noisy neighbors and reticent residents: Distinguishing resident from non-resident individuals to improve passive acoustic monitoring](https://www.sciencedirect.com/science/article/pii/S2351989421002602) | Dana S. Reid, Connor M. Wood, Sheila A. Whitmore, William J. Berigan, John J. Keane, Sarah C. Sawyer, Paula A. Shaklee, H. Anu Kramer, Kevin G. Kelly, Aimee Reiss, Nick Kryshak, R.J. Gutiérrez, Holger Klinck, M. Zachariah Peery | 2021| ... | ... |
| [soundClass: An automatic sound classification tool for biodiversity monitoring using machine learning](https://dspace.uevora.pt/rdpc/handle/10174/33324) | Silva, Bruno, Mestre, Frederico, Barreiro, Sílvia, Alves, Pedro J., Herrera, José M. | 2022 | Passive acoustic monitoring, a non-invasive technique, is increasingly used to study animal populations and habitats at much larger spatial and temporal scales than standard methods. However, easy to apply tools for reliable detection and classification of signals of interest among hundreds or even thousands of hours of recording are still lacking. We introduce the r package soundClass, a tool to train convolutional neural networks, and employ them to classify sound events in recordings. soundClass provides a sound event classification pipeline, from annotating recordings to automating trained networks usage in real-life situations. We illustrate the package functionality on bat echolocation calls, bird songs and whale echolocation clicks, showing that the package can be used to train networks for several types of sound events, taxonomic groups and environments; and exemplify its application. This tool facilitates the creation and usage of trained networks and was developed with a strong focus on graphical user interfaces to be used by non-specialist scientists in statistics and programming. | R package for sound classification |

## Other repos

[Bioacoustic Software](https://github.com/rhine3/bioacoustics-software)
