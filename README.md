# Food Vision Mini: Sushi/Steak/Pizza Classifier

A lightweight image classification model using **Transfer Learning** with **EfficientNetB0**, fine-tuned to classify food images into three categories: `sushi`, `steak`, and `pizza`.

## Key Details
- **Author**: Ruchita Sengupta  
- **Approach**:  
  - Base Model: `EfficientNetB0` (pre-trained on ImageNet)  
  - Hyperparameter Tuning: Fine tuning feature blocks and changing the classifier head.
  - Loss Function: Cross Entropy Loss
  - Optimizer: Adam Optimizer with learning rate 0.0001
  - Augmentation: Crop, Resize, Interpolation
- **Dataset**: Custom-curated dataset of 300 images in train and 100 images in test.  

## Performance Metrics
| Metric          | Test |
|-----------------|----------|
| Accuracy        | 94.67%   |
| Precision       | 94.13%    | 
| Recall          | 94.76%    |
| F1              | 94.35%    |



The notebook has a detailed flowchart by importing data,getting the model architecture,evaluating the model and calculating its evaluation metrics.
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1pptiJdYEklGlDjFZBViOYASuyGWrjVYs/view?usp=sharing)
