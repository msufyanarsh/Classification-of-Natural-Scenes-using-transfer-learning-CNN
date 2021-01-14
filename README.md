# Classification-of-Natural-Scenes-using-transfer-learning-Resnet-CNN
# Introduction:
  This repository contains Files required to reproduce the results image classification of natural images using CNN, Resnet50 and transfer learning.

Two approaches were used to get the results. In first approach,categorical cross entropy loss function and SGD optimizer along with data augmentation was used including width shift, shear, height shift, rotation and horizontal flipping. While in second implementation, Images were resized to the size of 224,224. Optimizer used was Adam with low learning rate value 2e-5. Details regarding settings, attempts, and the methodology can be found in the report attached in the repository.
# Dataset:
   Dataset used is of natural scenes.This Data contains around 25k images of size 150x150 distributed under 6 categories
   i.e. Buildings, Forest, Glacier , Mountain, Sea and Street. Dataset is used as
  1. Training set = 14k+ 150x150 Images in seg_train folder for training spread.
  2. Validation set = 3k+ 150x150 Images in seg_test folder for cross-validation spread.
  3. Test set = 7k+ 150x150 Images in seg_pred folder as test spread.
  
Dataset can be downloaded from: https://drive.google.com/drive/folders/1oTlf7HlyrhNSn_WRFbEqq4mAZYZLTAJR?usp=sharing


Test.npy link: https://drive.google.com/file/d/1ULbGjA8p968bPVookUqTUMRFKNyNj7Dp/view?usp=sharing

train.npy link: https://drive.google.com/file/d/1AHrGfl6LivoL-gKcjzNKBEL75R6Qfbx7/view?usp=sharing

Val.npy link:  https://drive.google.com/file/d/1w9l0b3GUCMawoYdigeDWvk_nLFYi8bjv/view?usp=sharing

Approach 1 weights "weights_of_mdl0.41.h5" link:  https://drive.google.com/file/d/1-2HjiiimAPgvxc50qNAXygugqsJMy3EV/view?usp=sharing

Pretrained weights "dbs-frozen.h5" link for implementation2 : https://drive.google.com/file/d/1DJFJkQdxp4gEvnN_Bcz2uc4zf9Zc78vj/view?usp=sharing
# Reproducing results using First Method(SGD optimizer and data augmentation)
  1. Download the dataset and extract in the google drive.
  2. The code is produced using colab so for better replication of the results, run this code on colab with the gpu available from google.
  3. After opening the code in colab, dataset needs to be loaded into the colab. mount the drive using the access link and load the data sets.
  4. Train the model, and move further with the code blocks.
  5. To reproduce the results, download weights file via link(weights_of_mdl0.41.h5 link) and load model weights by typing load model command below training code block. move further in the code blocks and check accuracy.(you dont have to retrain the model for this)
 # Reproducing results using Adam, and resizing dataset to 224*224
  1. I loaded and saved the dataset as npy, Download and save them into the google drive.
  2. After opening the code in colab, load the npy files.
  3. Run the code, train the model, and move further with the code blocks.
  4. To reproduce the results, download weights file and load model weights by for impl 2. move further in the code blocks and check accuracy.(you dont have to retrain the model for this)
  
# Results
![](Results/acc_f.png)
![](Results/los_f.png)


![](Results/heatmapf.png)

![](Results/com_mat_f.JPG)

![](Results/class_rep_f.JPG)

Test Accuracy:

![](Results/testaccf.JPG)

# Visual Classification results:

![](Results/CLASSREP.png)
