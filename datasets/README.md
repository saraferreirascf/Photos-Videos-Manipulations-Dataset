## Datasets
All datasets are labeled and balanced.

- <a href="https://github.com/saraferreirascf/Photos-Videos-Manipulations-Dataset/blob/main/datasets/train_videos.pkl" target="_blank">train_videos.pkl </a><br/> only contains the frames extracted from videos.
- <a href="https://github.com/saraferreirascf/Photos-Videos-Manipulations-Dataset/blob/main/datasets/train_photos.pkl" target="_blank">train_photos.pkl </a><br/> only contains photos.
- <a href="https://github.com/saraferreirascf/Photos-Videos-Manipulations-Dataset/blob/main/datasets/train_all.pkl" target="_blank">train_all.pkl </a><br/> contains all photos and frames extracted from videos. 

### How to use them:

- In python 3:

  ``` pkl_file = open("train_photo_final.pkl", 'rb')
   data = pickle.load(pkl_file)
   pkl_file.close()
   X_train = data["data"]
   y_train= data["label"] 
   
 - Convert pkl file to txt:
  
  ``` py pkl_to_txt.py <pkl filename> <output filename> ```
  
 - Convert pkl file to csv:

  ``` py pkl_to_csv.py <pkl filename> <output filename> ```
  *this script generates two .csv files. One for the features and one for the labels.
