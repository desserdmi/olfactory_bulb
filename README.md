


# Project Description

## Introduction
 This is a collaboration project between  the Interdisciplinary Center "Smell & Taste" Dresden, Germany and Center for Music in the Brain Aarhus, Denmark.

Disturbances of smell and taste are common. About 5% of the general population have anosmia (absence of the sense of smell). Olfactory dysfunction can markedly impair the quality of life. 
*([Hüttenbrink, K](https://www.aerzteblatt.de/suche?archivAutor=H%FCttenbrink%2C+K);  [Hummel, T](https://www.aerzteblatt.de/suche?archivAutor=Hummel%2C+T);  [Berg, D](https://www.aerzteblatt.de/suche?archivAutor=Berg%2C+D);  [Gasser, T](https://www.aerzteblatt.de/suche?archivAutor=Gasser%2C+T);  [Hähner, A](https://www.aerzteblatt.de/suche?archivAutor=H%E4hner%2C+A)
https://doi.org/10.3238/arztebl.2013.0001)*


Olfactory and emotional higher processing pathways share common anatomical substrates. Hence, depression is often accompanied by alterations in olfactory function. These alterations are negative in nature and may involve decreased activation in olfactory eloquent structures or decreased volume in the olfactory bulb (OB).
*(Croy, I. & Hummel, T. J Neurol (2017) 264: 631. https://doi.org/10.1007/s00415-016-8227-8)*

Furthermore, anosmia is a common non-motor feature of Parkinson's disease (PD). The  [olfactory tract](https://www.sciencedirect.com/topics/neuroscience/olfactory-tract "Learn more about Olfactory Tract from ScienceDirect's AI-generated Topic Pages")  is involved early in PD as indicated by frequent occurrence of [hyposmia](https://www.sciencedirect.com/topics/neuroscience/hyposmia "Learn more about Hyposmia from ScienceDirect's AI-generated Topic Pages") or anosmia years or decades before motor symptoms and by autopsy studies showing early  [synuclein](https://www.sciencedirect.com/topics/neuroscience/synuclein "Learn more about Synuclein from ScienceDirect's AI-generated Topic Pages")  pathology in the olfactory tract and [anterior olfactory nucleus](https://www.sciencedirect.com/topics/neuroscience/anterior-olfactory-nucleus "Learn more about Anterior Olfactory Nucleus from ScienceDirect's AI-generated Topic Pages") even in the early stages of PD. Testing for  [olfaction](https://www.sciencedirect.com/topics/neuroscience/olfaction "Learn more about Olfaction from ScienceDirect's AI-generated Topic Pages") consists of evaluation of olfactory thresholds, smell identification and discrimination, and  [olfactory memory](https://www.sciencedirect.com/topics/neuroscience/olfactory-memory "Learn more about Olfactory Memory from ScienceDirect's AI-generated Topic Pages").
*(Arjun Tarakad, Joseph Jankovic https://doi.org/10.1016/bs.irn.2017.05.028)*



![olfactory bulb](https://github.com/desserdmi/olfactory_bulb/blob/master/ob.png)
######  *Fig 1: Location of olfactory bulb (my own brain) in T2 MRI contrast, acquired on Siemens Prisma 3T . axial (A), sagittal (B) and coronar (C) views.*

## Aims

 
The main aim of this project is to develop a machine-learning algorithm for prediction of Anosmia/Dysosmia and associated diseases  (e.g. Major Depression, Parkinson's disease) based on clinical parameters like volume/shape of bulbus olfactorius, symptoms duration, TDI,  age or gender.

## Methods  

 1. Clinical data acquisition (already done) 

 <br>
 
 2.  Collecting (merge) data from different studies to one big dataset  (currently under development)

 <br>
 
<img src="https://github.com/desserdmi/olfactory_bulb/blob/master/collect_data.png" width=70% height=70% align="middle" />


<br>

3. Data exploration, Data cleaning and Preprocessing of collected dataset: <br><br>
3.1. What clinical populations do we have? <br>
3.2. How many samples per population? <br>
3.3. How many features/clinical parameters? <br>
3.4. Are features constant between different cohorts? <br>

<br>


4. Developing an automatic feature selection algorithm 
in order to identify biomarkers that are relevant for
the diagnosis.  The most promising way seems to be Recursive Feature Elimination with Support Vector Machine (RFE-SVM). As described in this [paper](https://doi.org/10.1101/711135), this method has shown incredible accuracy and stability of biomarkers selected by this [algorithm](https://www.biorxiv.org/content/10.1101/711135v1.full).
![Fig.3](https://www.biorxiv.org/content/biorxiv/early/2019/07/22/711135/F1.large.jpg?width=800&height=600&carousel=1)
###### *Fig. 2. Overview of the proposed method. Feature selection is performed systematically across different partitions of the original dataset. Robustness of selected biomarkersis assessed from the output of the RFE-SVM algorithm, and the final accuracy is averaged over subsamplings estimations. (*bioRxiv preprint first posted online Jul. 22, 2019; doi: http://dx.doi.org/10.1101/711135. The copyright holder for this preprint (which was not peer-reviewed) is the author/funder, who has granted bioRxiv a license to display the preprint in perpetuity. It is made available under a CC-BY-NC-ND 4.0 International license.)**


<br>


5.  Developing SVM Desease Prediction Algoritm  based on most relevant features.  SVM has
proven state of the art performance in computational biology. It has been already used successfully by
[R.Prashanth et al](https://doi.org/10.1016/j.ijmedinf.2016.03.001) for predicition of Early Parkinson's Disease through Multi-modal Features.  
Due to multi-modal features we are going to have (e.g. label volumes derived from MRI data, clinical functional measurements, psychological test results) it makes sense to try a similar approach.  Sure, the performance of other classifiers like Decision Tree or Random Forest (RF) should be tested. As output of the classifier we expect high accuracy, sensitivity and specificity in predicting disease labels. For now, we are not sure how many different disease labels we are going to have in the dataset and how many of them we will try to predict. It depends on the final version of collected dataset due availability of the data.  
 <img src="https://github.com/desserdmi/olfactory_bulb/blob/master/process.png" width=70% height=70% />

<br>
<br>
<br>
<br>

## Current state:

 - collecting and arranging the data
 - creating of working platform
 - literature review to improve methods


<br><br><br><br><br>

## *Your comments and suggestions are highly appreciated!*


Main Developer: Dmitriy Desser
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTczNzE3MzE5MywxMTE5MTc4MDExLC0xNT
Q4NzY3MDQyLC0xNDQyNjQ5MTU0LC03MTA3MTA3OTksLTE1MzQy
Mzc5MjUsLTg1NTMxMDYwMCwyOTUyODcwODgsOTA4MDk0NzA1LD
YyOTU2MjYxLDExNzYxNjQ4MTIsLTgyMzIwMDgzMywtMTUwNDQ4
MjU3LDM1NDU0NjYwMCwtMTExNjAzODUxNSw3MzU4Mzk3MzUsLT
I0MjI2MjAzNywyMDI5MDQxMzEwLC0yMDMzMjMwNDg4LDE2NzAz
OTIzNDJdfQ==
-->