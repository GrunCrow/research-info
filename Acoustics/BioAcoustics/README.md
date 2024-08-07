# BioAcoustics

Resources on the use of Deep Learning algorithms in the analysis of sounds and vocalizations of wildlife, especially birds.

## Software

### Models

#### [BirdNET](https://github.com/kahst/BirdNET-Analyzer)

#### [OpenSoundScape](https://github.com/kitzeslab/opensoundscape)

OpenSoundscape (OPSO) is free and open source Python utility library analyzing bioacoustic data.

#### [BirdAVES: Animal Vocalization Encoder based on Self-Supervision](https://github.com/earthspecies/aves?tab=readme-ov-file#birdaves)

AVES (Animal Vocalization Encoder based on Self-Supervision) is a self-supervised, transformer-based audio representation model for encoding animal vocalizations ("BERT for animals"). It is based on HuBERT (Hsu et al., 2021), a powerful self-supervised model for human speech, but pretrained on large-scale unannotated audio datasets (FSD50K, AudioSet, and VGGSound) which include animal sounds.

#### [PERCH](https://github.com/google-research/perch)

A bioacoustics research project.

### Tools

#### [CCAI Tutorial: Agile Modeling for Bioacoustic Monitoring](https://colab.research.google.com/drive/1gPBu2fyw6aoT-zxXFk15I2GObfMRNHUq?usp=sharing)

An interactive tutorial (requires user engagement) that demonstrates analyzing an unlabeled bioacoustic dataset for a target species given a vocalization of that species to help provide insights for ecologists, conservationists, land managers, and other domain experts. We achieve this by leveraging a high-quality, bioacoustic pre-trained model, searching over the unlabeled corpus conditioned on a single species example, and applying an efficient ML technique to produce matches.

#### [BTOAcousticPipelineVerificationApp](https://github.com/BritishTrustForOrnithology/BTOAcousticPipelineVerificationApp)

An RShiny App to help with manual checking of short audio clips. A typical use case is where you have a folder of clips that the Acoustic Pipeline has suggested are of a certain species. This app can be used to display a spectrogram of a sound clip, allow the sound to be played, and then a decision can be made whether the identity is true or false resulting in the clip being moved to a 'True' subfolder or a 'False' subfolder. The app can be customised for more complex workflows, such as if multiple species are present, or to perform simple clip-level labelling.

## Datasets

[BirdSet](https://github.com/DBD-research-group/BirdSet): A benchmark dataset collection for bird sound classification

## Labs

### [Kitzes Lab](https://www.kitzeslab.org/)

- [BioAcoustic Resources](https://docs.google.com/document/d/10APGahxU_GJewO8mkN2wzG0y-LHw3p_TAcYJDdHAQmg/edit#heading=h.mwbyo5325flj)
- [OpenSoundScape](https://github.com/kitzeslab/opensoundscape)

### [Meridian](https://meridian.cs.dal.ca/2015/07/31/detection-and-classification-of-marine-animal-sounds-using-deep-learning/)

Detection and classification of marine animal sounds using deep learning

## Papers

### Birds

| Title | Authors | Year | Abstract | Review |
|-------|---------|------|----------|--------|
| [BirdNET: A deep learning solution for avian diversity monitoring](https://www.sciencedirect.com/science/article/pii/S1574954121000273) | Stefan Kahl, Connor M. Wood, Maximilian Eibl, Holger Klinck | 2021 | ... | ... |
| [Assessing the potential of BirdNET to infer European bird communities from large-scale ecoacoustic data](https://www.sciencedirect.com/science/article/pii/S1470160X24006034?via%3Dihub) | David Funosas, Luc Barbaro, Laura Schillé, Arnaud Elger, Bastien Castagneyrol, Maxime Cauchoix| 2024 | ---------- | As noted in a recent review (Pérez‐Granados 2023), BirdNET’s prediction accuracy increases with confdence score, but substantial confusion remains about how to interpret BirdNET’s confdence scores [...] After analyzing the performance of nearly 1000 species, we have yet to encounter a class in BirdNET for which prediction accuracy does not increase with confdence score. While there is generally a positive relationship between prediction accuracy and confdence score, the shape of this relationship varies across classes, making it important to evaluate the meaning of BirdNET scores on a class-by-class basis [...] The technical description of sensitivity is that changes the sigmoid activation curve which determines how much neuron activation (aka less “signal” or “evidence” for a species) is required to reach higher output (confdence) scores. Lower sensitivity yields a steeper curve and increasingly binary outputs; higher sensitivity yields a shallower curve and a more uniform distribution of scores. [...] Translating BirdNET confdence scores, or the output scores of any detector, to prediction accuracy requires manual evaluation of model performance on a subset of the data |
| [Bird Species Use of Bioenergy Croplands in Illinois, USA—Can Advanced Switchgrass Cultivars Provide Suitable Habitats for Breeding Grassland Birds?](https://www.mdpi.com/2071-1050/16/11/4807) | Kirk E. LaGory... | 2024 | Grassland birds have sustained significant population declines in the United States through habitat loss, and replacing lost grasslands with bioenergy production areas could benefit these species and the ecological services they provide. Point count surveys and autonomous acoustic monitoring were used at two field sites in Illinois, USA, to determine if an advanced switchgrass cultivar that is being used for bioenergy feedstock production could provide suitable habitats for grassland and other bird species. At the Brighton site, the bird use of switchgrass plots was compared to that of corn plots during the breeding seasons of 2020–2022. At the Urbana site, the bird use of restored prairie, switchgrass, and Miscanthus × giganteus was studied in the 2022 breeding season. At Brighton, Common Yellowthroat, Dickcissel, Grasshopper Sparrow, and Sedge Wren occurred on switchgrass plots more often than on corn; Common Yellowthroat and Dickcissel increased on experimental plots as the perennial switchgrass increased in height and density over the study period; and the other two species declined over the same period. At Urbana, Dickcissel was most frequent in prairie and switchgrass; Common Yellowthroat was most frequent in miscanthus and switchgrass. These findings suggest that advanced switchgrass cultivars could provide suitable habitats for grassland birds, replace lost habitats, and contribute to the recovery of these vulnerable species. | BirdNET-Analyzer provided an estimate of the confidence level of each species identification. For this analysis, only detections with confidence levels ≥ 0.75 were used. |

### Submarine acoustics

| Title | Authors | Year | Abstract | Review |
| ------- | --------- | ------ | ---------- | -------- |
| [Acoustic Classification of Surface and Underwater Vessels in the Ocean Using Supervised Machine Learning](https://www.mdpi.com/1424-8220/19/16/3492) | Jongkwon Choi, Youngmin Choo and Keunhwa Lee | 2019 | Four data-driven methods—random forest (RF), support vector machine (SVM), feed-forward neural network (FNN), and convolutional neural network (CNN)—are applied to discriminate surface and underwater vessels in the ocean using low-frequency acoustic pressure data. Acoustic data are modeled considering a vertical line array by a Monte Carlo simulation using the underwater acoustic propagation model, KRAKEN, in the ocean environment of East Sea in Korea. The raw data are preprocessed and reorganized into the phone-space cross-spectral density matrix (pCSDM) and mode-space cross-spectral density matrix (mCSDM). Two additional matrices are generated using the absolute values of matrix elements in each CSDM. Each of these four matrices is used as input data for supervised machine learning. Binary classification is performed by using RF, SVM, FNN, and CNN, and the obtained results are compared. All machine-learning algorithms show an accuracy of >95% for three types of input data—the pCSDM, mCSDM, and mCSDM with the absolute matrix elements. The CNN is the best in terms of low percent error. In particular, the result using the complex pCSDM is encouraging because these data-driven methods inherently do not require environmental information. This work demonstrates the potential of machine learning to discriminate between surface and underwater vessels in the ocean. |--------|
| [Underwater Acoustic Image Classification Based on Image Denoising and Transfer Learning](https://ieeexplore.ieee.org/abstract/document/10451620) | Kexin Zhu; Yuxin Zhao; Liangfeng Zheng; Dequan Yang; Jianxin He; Xiong Deng | 2024 | With the potential shown by artificial intelligence in recent years, deep learning has been widely used in the field of marine environment monitoring such as underwater image classification. It will be disturbed by the marine environment in the acquisition process of underwater acoustic images, which will lead to the acquisition of images containing a lot of noise information. In addition, it is very difficult to collect a large amount of underwater acoustic image data because it is expensive and time-consuming to do so. Both of these factors will reduce the accuracy of underwater acoustic image classification. In order to overcome the influence of the above factors, we proposed an underwater acoustic image classification method based on image denoising and transfer learning. Firstly, we use curvature filtering for image denoising to eliminate the noise contained in the image, which can effectively remove noise while maintaining the edge information of the image. Then we utilize the transfer learning technique to improve the accuracy of underwater acoustic image classification. The experimental results show that the curvature-filtered images have better image evaluation indexes than other methods. Moreover, the classification methods based on transfer learning has better classification accuracy than the ones without transfer learning. | -------- |
| [Surface and underwater acoustic target recognition using only two hydrophones based on machine learning](https://pubs.aip.org/asa/jasa/article/155/6/3606/3295956) | Qiankun Yu; Wen Zhang; Min Zhu; Jian Shi; Yan Liu; Shuo Liu | 2024 | Surface and underwater (S/U) acoustic targets recognition is an important application of passive sonar. It is difficult to distinguish them due to the mixture of underwater target radiation noise and marine environmental noise. In previous studies, although using a single hydrophone was able to identify S/U acoustic targets, there were still a few hydrophones that had poor accuracy. In this paper, S/U acoustic targets recognition using two hydrophones based on Gradient Boosting Decision Tree is proposed, and it is first found out as high as 100% accuracy could be achieved with the implementation of SACLANT 1993 data. The real experimental data are always rare and insufficient. The big training dataset is generated using environmental information by acoustic model named KRAKEN. Simulation and experimental data used in the model are heterogeneous, and the differences between these two kinds of data are assimilated by using vertical linear array feature extraction method. The model realizes the recognition of S/U acoustic targets based on channel information besides source spectrum information. By using the combination of two hydrophones, the surface and underwater targets recognition accuracy reached 1 and 0.9384, while they are only 0.4715 and 0.5620 using a single hydrophone, respectively. | -------- |
| [Underwater Passive Target Classification based on β Variational Autoencoder and MFCC](https://ieeexplore.ieee.org/abstract/document/10256865) | Adarsh Sunilkumar; Shamju Joseph K; Manoj Kumar K | 2023 | Underwater passive target classification is an open set classification problem, where quite often test data of those classes, which were not present during training phase is encountered and it is a challenging task due to the intrinsic complexity of the radiated noise from the target. Conventional classification architectures with spectral processing often fail miserably. Supervised learning methods like deep learning, offers higher success rate but they require enormous amount of data for training and their performance in open set classification is again a challenge. This paper presents an effective method for underwater target classification by the beta variational autoencoder (β − VAE) model with Mel Frequency Cepstral Coefficients (MFCCs) features. MFCC effectively utilises the non-linear auditory effect of the human ear with different frequencies. β – VAE, being one of the generative models, is capable of generalizing with less amount of data. Classification experiments on various underwater targets have been performed with the proposed method, and results indicate that the proposed method is effective in underwater passive target classification. | -------- |

#### PAM - Passive Acoustic Monitoring

Papers that are not focused on the use of Deep Learning techniques for Bioacoustics.

| Title | Authors | Year | Abstract | Review |
|-------|---------|------|----------|--------|
| [Noisy neighbors and reticent residents: Distinguishing resident from non-resident individuals to improve passive acoustic monitoring](https://www.sciencedirect.com/science/article/pii/S2351989421002602) | Dana S. Reid, Connor M. Wood, Sheila A. Whitmore, William J. Berigan, John J. Keane, Sarah C. Sawyer, Paula A. Shaklee, H. Anu Kramer, Kevin G. Kelly, Aimee Reiss, Nick Kryshak, R.J. Gutiérrez, Holger Klinck, M. Zachariah Peery | 2021| ... | ... |
| [soundClass: An automatic sound classification tool for biodiversity monitoring using machine learning](https://dspace.uevora.pt/rdpc/handle/10174/33324) | Silva, Bruno, Mestre, Frederico, Barreiro, Sílvia, Alves, Pedro J., Herrera, José M. | 2022 | Passive acoustic monitoring, a non-invasive technique, is increasingly used to study animal populations and habitats at much larger spatial and temporal scales than standard methods. However, easy to apply tools for reliable detection and classification of signals of interest among hundreds or even thousands of hours of recording are still lacking. We introduce the r package soundClass, a tool to train convolutional neural networks, and employ them to classify sound events in recordings. soundClass provides a sound event classification pipeline, from annotating recordings to automating trained networks usage in real-life situations. We illustrate the package functionality on bat echolocation calls, bird songs and whale echolocation clicks, showing that the package can be used to train networks for several types of sound events, taxonomic groups and environments; and exemplify its application. This tool facilitates the creation and usage of trained networks and was developed with a strong focus on graphical user interfaces to be used by non-specialist scientists in statistics and programming. | R package for sound classification |

## Other repos

[Bioacoustic Software](https://github.com/rhine3/bioacoustics-software)
