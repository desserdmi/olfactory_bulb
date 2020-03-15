


#  <p align="center"> Project Description

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

 
The main aim of this project is to develop a machine-learning algorithm for prediction of anosmia/dysosmia cause based on clinical parameters like volume/shape of bulbus olfactorius, symptoms duration, TDI,  age and gender.

## Methods  

 1. Clinical data acquisition (already done) 

 <br>

 <br>
 

<br>

3. Data exploration, Data cleaning and Preprocessing of collected dataset: <br><br>

3.1. What clinical populations do we have? <br>

Patients with post-viral (PV), post-traumatic (PT), idiopatic (IP) lost of olfactory function and healthy cohort.  <br>
3.2. How many samples per population? <br>

~ 70 patients and ~ 70 control

3.3. What features/clinical parameters do we have? <br>
Age, sex, duration of olfactorys' function loss, TDI-scores, Volume of olfactory bulb<br><br>

4. MRI Data Preprocessing and manual segmentation<br>
4.1. Original T2 MRI scans (original size: 256x256x32)  were resampled to the size of (1200x1200x32) using scipy resamle function and cubic interpolation method. Then the segmentation and creation of binary masks of olfactory bulbs was performed using ITK Snap 3.8 software. afterwards the masks were resampled back to the original size using nilearn resample function and nearest neighbor interpolation method. This step improved the dice coefficient by **8%** compared to segmentation directly on original images without resampling step.     


6. Developing an automatic feature selection algorithm 
in order to identify biomarkers that are relevant for
the diagnosis.  

<br>


5.  Developing SVM Desease Prediction Algoritm  based on most relevant features.  SVM has
proven state of the art performance in computational biology. It has been already used successfully by
[R.Prashanth et al](https://doi.org/10.1016/j.ijmedinf.2016.03.001) for predicition of Early Parkinson's Disease through Multi-modal Features.  
Due to multi-modal features we are going to have (e.g. label volumes derived from MRI data, clinical functional measurements, psychological test results) it makes sense to try a similar approach.  Sure, the performance of other classifiers like Decision Tree or Random Forest (RF) should be tested. As output of the classifier we expect high accuracy, sensitivity and specificity in predicting disease labels. For now, we are not sure how many different disease labels we are going to have in the dataset and how many of them we will try to predict. It depends on the final version of collected dataset due availability of the data.  
<br><br>
<p align="center"> <img src="https://github.com/desserdmi/olfactory_bulb/blob/master/process.png" width=70% height=70% /></p>

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
eyJoaXN0b3J5IjpbLTE5ODMzOTIyODUsMjEzMzI0NTMxNyw1OD
U3OTc5ODgsMTc5ODQ3MTY4LDExMTkxNzgwMTEsLTE1NDg3Njcw
NDIsLTE0NDI2NDkxNTQsLTcxMDcxMDc5OSwtMTUzNDIzNzkyNS
wtODU1MzEwNjAwLDI5NTI4NzA4OCw5MDgwOTQ3MDUsNjI5NTYy
NjEsMTE3NjE2NDgxMiwtODIzMjAwODMzLC0xNTA0NDgyNTcsMz
U0NTQ2NjAwLC0xMTE2MDM4NTE1LDczNTgzOTczNSwtMjQyMjYy
MDM3XX0=
-->