# Skin Aging Classification – Lightweight Models for Mobile Diagnosis

## Project Overview
This project focuses on classifying the level of forehead skin aging into four categories (levels 1 to 4). The goal is to develop a lightweight deep learning model suitable for use in mobile applications, such as smartphone-based skin diagnostics.

Three models were implemented and evaluated for this task: MobileNetV2, SqueezeNet. Each model was fine-tuned and adjusted to improve image classification performance for skin aging analysis.

## Project Files
- **Data** :
  - **image** : 4,825 forehead images from 965 individuals, captured at 5 angles (front, left 15°, left 30°, right 15°, right 30°).
  - **label** : 4,825 JSON files containing forehead aging grades and image size details, assessed by experts
  - `json_to_datframe.csv` : A dataframe created from the 4,825 JSON files
- **Notebook** :
  - `json_to_datframe.ipynb` 
  - `training.ipynb`, 'test.ipynb' : model training and test
- **models** : the trained models are saved
- **assets** : Visualisations, such as confusion matrix and real forehead images can be founded.


## Methodology 
- **Constructing Dataframe** : Generate `json_to_datframe.csv` to make json files handling more easy.
- **Preprocessing**
  - Label rebalancing : Reduced 7 labels to 4 (0, 1 -> 1, 3, 4 -> 2, 5 -> 3, 6 -> 4) to reduce confusion in the confusion matrix and provide more intuitive aging grades for consumers.
  - Image resizing : Resized images based on the bounding box coordinates for each image.
  - Data augmentation 
- **Modeling** : **MobileNetV2*** and **SqueezeNet**(lighter models) were used, and each model underwent processes such as dropout, adjusting the number of nodes, and modifying the batch size to prevent overfitting and improve model performance.

  
- **Traiing and Hyperparameter Optimization**

## Key Findings 
- **Model Performance**
  *** Model comparison using the imsage test set

## Conclusion
**Data-Driven approach to enhancing customer experience and business operation**

## Used Datasets
