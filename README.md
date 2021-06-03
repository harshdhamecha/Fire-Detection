# Fire-Detection
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/harshdhamecha/Fire-Detection/blob/main/Fire-Detector.ipynb)  

This repo consists of the Fire Detection project, gives 0.96 ROC-AUC score using MobileNetV2. 

## Datasets 
I have used [this](https://www.kaggle.com/phylake1337/fire-dataset) dataset and few more images from the Google. At the end, I have `867` images for a class **`fire`** and `787` images for a class **`non-fire`**.

### Data Preprocessing


### Data Augmentation


## Model Architecture
I have used `MobileNetV2` as a basemodel and a few more `Dense`, `AveragePooling2D` and `Dropout` layers on top of it.  

### Hyperparameters  

Following is the Hyperparameters values which I have used in this porject.  

Name | Value
-----|------
Learning Rate | 0.0001
Epochs | 20
Batch Size | 32
Optimizer | Adam
Activation Function | Relu(Hidden layers) and Softmax(Last layer)
Loss Function | Binary Cross Entropy

## Results 

### On Test-set Images
![](Results/test_set.PNG)
### On Custom Images
![](Results/custom_test_imgs.PNG)

## Evaluation
### Classification Report
![](Results/classification-report.PNG)  

### ROC-AUC Curve
![](Results/roc-auc-curve.PNG)
