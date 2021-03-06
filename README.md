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
|<a href="https://generated.photos/" target="_blank">100K Faces Project </a>  | 10000 | - | njbhjebhr |
| <a href="https://thispersondoesnotexist.com/" target="_blank">This person does not exist </a> | 10000 | - | wehwu |
| <a href="https://github.com/wenbihan/coverage" target="_blank">COVERAGE dataset </a> | 97| 97| jehbrb|
| <a href="https://www.ee.columbia.edu/ln/dvmm/downloads/AuthSplicedDataSet/AuthSplicedDataSet.htm" target="_blank">Columbia Image Splicing Dataset </a> | 180 | 183 | hegrher |
| <a href="https://uporto-my.sharepoint.com/:f:/g/personal/up201606726_up_pt/ElCayyzNd5tMkvCbIFwjtrsBMiuuHpSR10iV8S5Tj5_vBw?e=9U2SFG" target="_blank">Dataset created by us </a> | 14 | 14 | jerherw |
| <a href="https://arxiv.org/abs/1909.12962" target="_blank">Celeb-DFv1* </a> | 795 | 158 | hebghweb|  

**This dataset only contains videos. Between 3-4 fps were extracted from each video and added to the final dataset*


<!--a href="https://www.autopsy.com/download/" target="_blank">Here</a>, it is possible to find the compilation of all datasets already labeled.-->
The final dataset already labeled is available <a href="https://github.com/saraferreirascf/Photos-Videos-Manipulations-Dataset/tree/main/datasets" target="_blank">here</a>

## Features

- Features extraction with Discrete Fourier Transform implementation
- Images and videos classification with SVM-based model
- Combines both objects and faces.

## Experimental setup

![Pipeline](https://github.com/saraferreirascf/Photos-Videos-Manipulations-Dataset/blob/main/experimental_setup_cropped.png)

In order to transform the simple dataset to a labeled dataset it is needed some pre-processing. The goal here is to use the photos and videos present in this dataset to classify other photos and videos. 
To achieve this, the first step is to extract features from each file. Afterwards, it will be possible to compare this features with the features of multimedia content target of investigation, inferring if they are manipulated or not. 
This features will be extracted using the method "Unmasking deepfake using Simple Features". 
To automate this feature extraction process a python script was created. To use this script it is needed to identify the folder where the files to extract features are and the number of files to be analyzed (normally the minimum between the two classes).
After extracting the features of a photo or video frame, this file will be classified considering the folder where it is. All files in the folder "fake" are going to be classified with 0 and all files in the folder "real" will be classified with 1. 
After iterating through all the files, extracting all features and labeling, the result is a fully labeled dataset.

## Publications
- Ferreira, S., Antunes, M., & Correia, M. E. "Forensic analysis of tampered digital photos"; 25th Iberoamerican Congress on Pattern Recognition (CIARP); May 2021; Porto; Portugal; to be published in Springer Lecture Notes on Computer Science. 
  - Paper is available in the proceedings of the conference, at https://ciarp25.org/wp-content/uploads/sites/10/2021/05/CIARP25-Papers.pdf (accessed on 16 June 2021), pp.402-411.
- Ferreira, S., Antunes, M., & Correia, M. E. (2021). Exposing Manipulated Photos and Videos in Digital Forensics Analysis. Journal of Imaging, 7(7), 102. <a href="https://www.mdpi.com/2313-433X/7/7/102" target="_blank">doi:10.3390/jimaging7070102</a>
- Ferreira, S.; Antunes, M.; Correia, M.E. A Dataset of Photos and Videos for Digital Forensics Analysis Using Machine Learning Processing. Data 2021, 6, 87. https://doi.org/10.3390/data6080087

