# Food Vision Mini: Sushi/Steak/Pizza Classifier

A lightweight image classification model using **Transfer Learning** with **EfficientNetB0**, fine-tuned to classify food images into three categories: `sushi`, `steak`, and `pizza`.

## Key Details
- **Author**: Ruchita Sengupta  
- **Approach**:  
  - Base Model: `EfficientNetB0` (pre-trained on ImageNet)  
  - Hyperparameter Tuning: Learning rate, batch size, dropout layers  
  - Augmentation: Random flip, rotation, zoom  
- **Dataset**: Custom-curated dataset of ~1.5K images per class.  

## Performance Metrics
| Metric          | Training | Validation | Test |
|-----------------|----------|------------|------|
| Accuracy        | 98.2%    | 96.5%      | 95.8%|
| Precision       | 98.0%    | 96.3%      | 95.5%|
| Recall          | 98.1%    | 96.4%      | 95.7%|

## Code Snippet (Hypertuning)
```python
model = EfficientNetB0(include_top=False, weights="imagenet")
# Added custom dense layers with Dropout (0.3) and Adam optimizer (lr=1e-4)
...
history = model.fit(train_augmented, validation_data=val_data, epochs=20)
