


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
Fig 1: *Location of olfactory bulb (my own brain) in T2 MRI contrast, acquired on Siemens Prisma 3T . axial (A), sagittal (B) and coronar (C) views.* 

### Aims

 
The main aim of this project is to develop a machine-learning algorithm for prediction of Anosmia/Dysosmia and associated diseases  (e.g. Major Depression, Parkinson's disease) based on clinical parameters like volume/shape of bulbus olfactorius, symptoms duration, TDI,  age or gender.

### Methods  

 1. Clinical data acquisition (already done) 
 2.  Collecting (merge) data to one big dataset  (currently under development)
 3. Preprocessing of collected dataset
4. Developing an automatic feature selection algorithm 
in order to identify biomarkers that are relevant for
the diagnosis.  The most promising way seems to be Recursive Feature Elimination with Support Vector Machine (RFE-SVM). As described in this [paper](https://doi.org/10.1101/711135), this method has shown incredible accuracy 

- desease  prediction algoritm (SVM) based on most relevant features
*(Jörn Lötsch, Dario Kringel and Thomas Hummel https://doi.org/10.1093/chemse/bjy067)*

- cross-validation (CV)

### Current state:

 - collecting and arranging the data
 - creating of working platform
 - literature review to improve methods


<br><br><br><br><br>

## *Your comments and suggestions are highly appreciated!*


Main Developer: Dmitriy Desser
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU3NTY2MDA3LC0xMjcxNTg5MjEyLDg5OT
kxMTY5XX0=
-->