# Food Vision Mini: Sushi/Steak/Pizza Classifier

A lightweight image classification model using **Transfer Learning** with **EfficientNetB0**, fine-tuned to classify food images into three categories: `sushi`, `steak`, and `pizza`.

## Key Details
- **Author**: Ruchita Sengupta  
- **Approach**:  
  - Base Model: `EfficientNetB0` (pre-trained on ImageNet)  
  - Hyperparameter Tuning: Learning rate, batch size, dropout layers  
  - Augmentation: Crop, Resize, Interpolation
- **Dataset**: Custom-curated dataset of 300 images in train and 100 images in test.  

## Performance Metrics
| Metric          | Training | Validation | Test |
|-----------------|----------|------------|------|
| Accuracy        | 98.2%    | 96.5%      | 95.8%|
| Precision       | 98.0%    | 96.3%      | 95.5%|
| Recall          | 98.1%    | 96.4%      | 95.7%|

