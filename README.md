## Authors

- Sara Ferreira - Department of Computer Science; Faculty of Sciences; University of Porto, 4169-007 Porto, Portugal; sara.ferreira@fc.up.pt
- Mário Antunes - Computer Science and Communication Research Centre (CIIC), School of Technology and Management, Polytechnic of Leiria; 2411-901 Leiria; Portugal; mario.antunes@ipleiria.pt  <br>
INESC TEC, CRACS; 4200-465 Porto; Portugal
- Manuel E. Correira - Department of Computer Science; Faculty of Sciences; University of Porto, 4169-007 Porto, Portugal;  mdcorrei@fc.up.pt <br>
INESC TEC, CRACS; 4200-465 Porto; Portugal 

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



