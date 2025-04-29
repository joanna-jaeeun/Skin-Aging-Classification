# Skin Aging Classification – Lightweight Models for Mobile Diagnosis

## Project Overview
This project focuses on classifying the level of forehead skin aging into four categories (levels 1 to 4). The goal is to develop a lightweight deep learning model suitable for use in mobile applications, such as smartphone-based skin diagnostics.

Three models were implemented and evaluated for this task: MobileNetV2, SqueezeNet. Each model was fine-tuned and adjusted to improve image classification performance for skin aging analysis.

## Project Files
- **Data** : Orignal images are stored in 'data/raw', new generated data is in 'data'..?
- **Notebook** : The notebook for traning and testing is in the 'notebook' folder.
- **Result** : The trained models are saved in the `results/models` folder. Visualisations, such as confusion matrix, can be found in the `results/figures` folder, which also includes screenshots of the face mask detection in the video.

## Methodology 
- **Preprocessing** : Image were resized / level were adjusted according to image similarity check using open CV 
- **Modeling**
  
  ***MobieNetV2***
- **Traiing and Hyperparameter Optimization**

  Fine-tyned with a lower learing rate -> 자동조정 하면 좋은뎅...

## Key Findings 
- **Model Performance**
  *** Model comparison using the imsage test set

## Conclusion
**Data-Driven approach to enhancing customer experience and business operation**

## Used Datasets
