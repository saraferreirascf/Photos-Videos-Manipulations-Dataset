## Authors

- Sara Ferreira - Department of Computer Science; Faculty of Sciences; University of Porto, Porto, Portugal; sara.ferreira@fc.up.pt
- Mário Antunes - Computer Science and Communication Research Centre (CIIC), School of Technology and Management, Polytechnic of Leiria; Leiria; Portugal; mario.antunes@ipleiria.pt  <br>
INESC TEC, CRACS; Porto; Portugal
- Manuel E. Correira - Department of Computer Science; Faculty of Sciences; University of Porto, Porto, Portugal;  mdcorrei@fc.up.pt <br>
INESC TEC, CRACS; Porto; Portugal 

## Objects and faces manipulations dataset

This dataset represents a compilations of several dataset that contains real photos and video frames and forged ones. This forged photos and video frames contais several types of manipulation like copy-move, splicing and deepfake.

| Name  |  Fake | Real | 
| ----------- | ----------- | ----------- | 
| <a href="https://arxiv.org/abs/1710.10196" target="_blank">CelebA-HQ dataset</a> |   -     | 10000 | 
| <a href="https://arxiv.org/abs/1812.04948" target="_blank">Flickr-Faces-HQ dataset </a>   | -       | 10000 | jewknjrw |
| 100K Facesproject | 10000 | - | njbhjebhr |
| <a href="https://thispersondoesnotexist.com/" target="_blank">This person does not exist </a> | 10000 | - | wehwu |
| <a href="https://github.com/wenbihan/coverage" target="_blank">COVERAGE dataset </a> | 97| 97| jehbrb|
| <a href="https://www.ee.columbia.edu/ln/dvmm/downloads/AuthSplicedDataSet/AuthSplicedDataSet.htm" target="_blank">Columbia Image Splicing Dataset </a> | 180 | 183 | hegrher |
| <a href="https://uporto-my.sharepoint.com/:f:/g/personal/up201606726_up_pt/ElCayyzNd5tMkvCbIFwjtrsBMiuuHpSR10iV8S5Tj5_vBw?e=9U2SFG" target="_blank">Dataset created by us </a> | 14 | 14 | jerherw |
| <a href="https://arxiv.org/abs/1909.12962" target="_blank">Celeb-DFv1* </a> | 795 | 158 | hebghweb|  

**This dataset only contains videos. Between 3-4 fps were extracted from each video and added to the final dataset*


<!--a href="https://www.autopsy.com/download/" target="_blank">Here</a>, it is possible to find the compilation of all datasets already labeled.-->
The final dataset already labeled is available <a href="https://github.com/saraferreirascf/Deep-fake-detector/tree/main/datasets" target="_blank">here</a>

## Features

- Features extraction with Discrete Fourier Transform implementation
- Images and videos classification with SVM-based model
- Combines both objects and faces.

## Experimental setup

![Pipeline](https://github.com/saraferreirascf/Objects-faces-manipulations-dataset/blob/main/experimental_setup.png)

In order to transform the simple dataset to a labeled dataset it is needed some pre-processing. The goal here is to use the photos and videos present in this dataset to classify other photos and videos. 
To achieve this, the first step is to extract features from each file. Afterwards, it will be possible to compare this features with the features of multimedia content target of investigation, inferring if they are manipulated or not. 
This features will be extracted using the method "Unmasking deepfake using Simple Features". 
To automate this feature extraction process a python script was created. To use this script it is needed to identify the folder where the files to extract features are and the number of files to be analyzed (normally the minimum between the two classes).
After extracting the features of a photo or video frame, this file will be classified considering the folder where it is. All files in the folder "fake" are going to be classified with 0 and all files in the folder "real" will be classified with 1. 
After iterating through all the files, extracting all features and labeling, the result is a fully labeled dataset.

