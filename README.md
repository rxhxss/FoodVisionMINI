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
| Metric          | Test |
|-----------------|----------|
| Accuracy        | 94.67%   |
| Precision       | 94.13%    | 
| Recall          | 94.76%    |
| F1              | 94.35%    |

