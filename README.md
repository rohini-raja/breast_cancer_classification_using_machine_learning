# breast_cancer_classification_using_machine_learning
Classification of breast cancer as begin and fatal stage using histopathological images
Hereby I summarize all the results obtained:
1)CNN - Convolutional Neural Network ( + PCA)
  Here,We split the dataset into four different ranges:
   -> training = 0.8 and validation =0.1 --> Accuracy = 0.86 ,Specificity = 0.901,Sensitivity =0.85.
   -> training = 0.6 and validation =0.4 --> Accuracy = 0.84 ,Specificity = 0.983,Sensitivity =0.692.
   -> training=  0.7 and validation =0.3 --> Accuracy = 0.87 ,Specificity = 0.845,Sensitivity =0.883.
   -> training=  0.5 and validation =0.5 --> Accuracy = 0.82 ,Specificity = 0.0  ,Sensitivity =1.
   And all the output screenshots have been attached in the CNN folder.
   
  ->K-fold cross validation is performed and the results are given in Cross validation folder.
  
      Accuracy Obtained=0.85
	  
2)Transfer Learning:

       Accuracy Obtained:0.96

The methods include Deep Learning based approaches to create classifier frameworks which 
->perform end to end data set manipulation, 
->ensembling,
->training, 
->test augmentation and detection.
->Transfer learning using Resnet(ResNet50,ResNet152) and Densenet(DenseNet169) architectures was performed.

We aim to deal with the various discrepancies in the images and the dataset by taking various data pre processing and augmentation
methods.Here we got an accuracy of 0.96 and we have attached the Screenshots and respective code in the Transfer Learning folder.
3)SVM:

         Accuracy Obtained=0.97

The analysis is divided into four sections:
1. Identifying the problem  and Data Sources
2. Exploratory Data Analysis
3. Pre-Processing the Data
4. Build model to predict whether breast cell tissue is  malignant or Benign
We constructed a predictive model using SVM machine learning algorithm to predict the diagnosis of a breast tumor.
The diagnosis of a breast tumor is a binary variable (benign or malignant).
We also evaluated the model using confusion matrix the receiver operating curves (ROC), which are essential in assessing and interpreting the fitted model.

SVM classification gives an accuracy of 0.95
and after performing Principal Component Analysis we get an  optimised accuracy of 0.97.
and we have attached the output screenshots in the SVM folder.
4)RandomForest or Random Decision Tree:
 
                     Accuracy obtained=0.9181

 -Here we used the data obtained from the histopathological images such as 
->texture_mean,
->perimeter_mean,
->smoothness_mean,
->Compactness_mean,
->Symmetry_mean to identify the type of cancer(either beginning state or malignant state).
and  we have attached all the output screenshots and graphs in the RandomForest Folder.
5)Multi-Instance Classifier:
    An interpretable classifier for high-resolution breast cancer screening images utilizing weakly supervised localization:
Highlights:
- High Accuracy: MIC outperformed ResNet-34 and Faster R-CNN.
- High Efficiency: Compared to ResNet-34, GMIC has **28.8%** fewer parameters, uses **78.43%** less GPU memory and is **4.1x** faster during inference and **5.6x** faster during training.
- Weakly Supervised Lesion Localization**: Despite being trained with only image-level labels indicating the presence of any benign or malignant lesion, GMIC is able to generate pixel-level saliency maps (shown below) that provide additional interpretability.
6)Vision Model:
                    Accuracy obtained=0.87
We developed a vision model to detect breast cancer in histopathological images.
Two classes will be used in this project: **Benign and Malignant.**
It includes multiple steps as follows:
   ->Load and preprocess the image dataset
   ->Train the image classifier on your dataset
   ->Use the trained classifier to predict image content
And we have attached the output screenshot files in Vision Model folder.
