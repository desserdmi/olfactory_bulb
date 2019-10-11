


# Project description Dima

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

 - develop a CNN for automated segmentation of bulbus olfactorius based on T2 - MRI scans
 - develop a machine-learning algorithm for prediction of Anosmia/Dysosmia and associated diseases  (e.g. Major Depression, Parkinson's disease) based on clinical parameters like volume/shape of bulbus olfactorius, symptoms duration, TDI,  age or gender.

### Methods  

 - manual segmentation of olfactory bulb based on T2 - contrast MRI images using 3DSlicer and ITK-SNAP
 - clinical data acquisition (already done) 
 - collect (merge) data to one big dataset 
 - data preprocessing (e.g. with pandas)
- automatic feature selection procedure
in order to identify biomarkers that are relevant for
the diagnosis using Recursive Feature
Elimination with Support Vector Machine (RFE-SVM)
*(Leonardo Gutiérrez-Gómez,  Jean-Charles Delvenne https://doi.org/10.1101/711135)*

- desease  prediction algoritm (SVM) based on most relevant features
*(Jörn Lötsch, Dario Kringel and Thomas Hummel https://doi.org/10.1093/chemse/bjy067)*

- cross-validation

### Current state:

 - collecting and arranging the data
 - creating of working platform
 - literature review to improve methods

# *Your comments and suggestions are highly appreciated!*

<p><a href="https://commons.wikimedia.org/wiki/File:Beelden_in_Leiden_2016_04_crop.jpg#/media/File:Beelden_in_Leiden_2016_04_crop.jpg"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/28/Beelden_in_Leiden_2016_04_crop.jpg/1200px-Beelden_in_Leiden_2016_04_crop.jpg" alt="Beelden in Leiden 2016 04 crop.jpg"></a><br>By <a href="//commons.wikimedia.org/wiki/User:Bic" title="User:Bic">User:Bic</a> - <a href="//commons.wikimedia.org/wiki/File:%27Beelden_in_Leiden%27_2016_04.jpg" title="File:'Beelden in Leiden' 2016 04.jpg">File:'Beelden in Leiden' 2016 04.jpg</a>, <a href="https://creativecommons.org/licenses/by-sa/4.0" title="Creative Commons Attribution-Share Alike 4.0">CC BY-SA 4.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=58167980">Link</a></p>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyNzY4NTgyNDIsMjE0Njc0NjYxNywxNz
UyODU0MTY0LC03MjI2OTcwMDQsLTEwNDk1NDQ0MzgsMTgzNDMy
OTY4Niw1ODgzMTkzNjIsMTMwNDAwMTgxMCwtMTMzMjk3ODkzOC
wtNTYyMDU4NzY1LC0xMjc2NDA0OTQsMTU4NDg2OTU1NiwtMTUx
MzU1MTM2NiwxNTA1MTc5MDc3LDYzMjY3OTY0Myw3MDc3MDMyNz
UsMTg5OTMwOTUyNSwtMTk5NTczMzg4LC01MzI0NTQ1OTMsMTk4
MTcyNDc4MV19
-->