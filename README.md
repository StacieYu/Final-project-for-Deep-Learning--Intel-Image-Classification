# Final-project-for-Deep-Learning--Intel-Image-Classification

## 📌 Project Overview

This project aims to classify aerial/satellite images into six land-use categories using deep learning. We experiment with multiple convolutional neural network (CNN) architectures and transfer learning approaches on the Intel Image Classification dataset. The objective is to explore the effects of model complexity, regularization, and fine-tuning strategies on classification performance.

---

## 🧠 Problem Statement

The task is to classify images into one of the following six classes:

- Buildings  
- Forest  
- Glacier  
- Mountain  
- Sea  
- Street  

This problem has practical applications in environmental monitoring, urban planning, and automated satellite image analysis.

---

## 🛠️ ML Methods and Techniques Used

### Model Variants:

1. **Baseline CNN** – a simple CNN trained from scratch.  
2. **CNN with Early Stopping** – same model with early stopping for regularization.  
3. **Transfer Learning** – MobileNetV2 with frozen base layers.  
4. **Fine-Tuned Transfer Learning** – MobileNetV2 with top layers unfrozen and retrained.

### Techniques Applied:

- Data Augmentation  
- Dropout Regularization  
- Learning Rate Scheduling  
- Transfer Learning with MobileNetV2  
- Validation curve analysis  
- Model comparison with metrics and plots  

---

## 📊 Results Summary

| Model                     | Training Acc. | Validation Acc. | Validation Loss | Strength                        |
|--------------------------|---------------|------------------|------------------|----------------------------------|
| Baseline CNN             | ~85%          | ~87–88%          | ~0.35            | Fast training baseline           |
| Early Stopping           | ~84–86%       | ~88%             | ~0.33–0.35       | Prevented overfitting            |
| Transfer Learning        | ~85%          | ~88.5%           | ~0.34            | Leveraged pretrained features    |
| **Fine-Tuned Transfer**  | **~88%**      | **~89%**         | **~0.32**        | **Best performance overall**     |

---

## 📈 Key Takeaways

- Transfer learning significantly improves performance over training from scratch.
- Fine-tuning pretrained models further enhances results, especially when learning rates are adjusted.
- Early stopping helps avoid overfitting but can limit learning if misconfigured.
- Validation accuracy generally exceeds training accuracy, indicating good generalization.

---

## 💡 Suggestions for Future Work

- Stronger and more diverse data augmentation  
- Gradual (layer-wise) unfreezing of pretrained models  
- Explore more advanced architectures like EfficientNet or ResNet  
- Use cosine annealing or ReduceLROnPlateau for learning rate scheduling  
- Apply k-fold cross-validation or model ensembling for better generalization  

---
