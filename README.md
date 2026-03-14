# DentalAI  
### A Deep Learning-Based Diagnostic Tool  

This project focuses on developing a machine learning model to predict oral diseases using medical images. By experimenting with various state-of-the-art architectures, DenseNet emerged as the top performer, achieving an accuracy of **91.04%**.  

---

## 📌 Project Overview 
Oral health plays a critical role in overall well-being. Early detection of oral diseases such as dental caries, gingivitis, and oral cancer is essential for effective treatment. This system automates the diagnostic process, leveraging deep learning for accurate and efficient predictions.  

---

## ⚙️ Model Comparison  

| **Architecture**  | **Accuracy** | **Why It Was/Wasn't Chosen**                             |  
|--------------------|--------------|---------------------------------------------------------|  
| **DenseNet-121**   | 91.04%       | Exceptional performance, faster convergence, and generalization. |  
| **ResNet-50**      | 86%          | Strong feature extraction but prone to overfitting.     |  
| **InceptionV3**    | 85%          | Good accuracy but struggled with some rare classes.     |  
| **VGG-16**         | 82%          | Computationally heavy with relatively lower accuracy.   |  
| **MobileNet**      | 79%          | Lightweight, but underperformed for this dataset.       |  

DenseNet-121 was chosen for its superior accuracy, efficiency, and ability to generalize well across the dataset.  

---

## 📊 Key Results  
- **Accuracy**: 91.04%  
- **Precision**: 86%  
- **Recall**: 88%  
- **F1 Score**: 87%  

### Confusion Matrix  
Below is the confusion matrix for the model's performance:  

![Confusion Matrix](https://github.com/sajaltandon/OralGuard-AI/blob/main/result/Confusion%20Matrix.jpg)  

---

### Classification Report  

| CLASS                 | PRECISION | RECALL | F1-SCORE | SUPPORT |  
|-----------------------|-----------|--------|----------|---------|  
| **Dental Caries**     | 0.86      | 0.88   | 0.87     | 476     |  
| **Gingivitis**        | 0.65      | 0.90   | 0.76     | 469     |  
| **Mouth Ulcer**       | 0.94      | 0.94   | 0.94     | 588     |  
| **Tooth Discoloration** | 0.87      | 0.84   | 0.86     | 366     |  
| **Hypodontia**        | 0.95      | 0.83   | 0.89     | 250     |  
| **Accuracy**          |           |        | 0.91     | 2069    |  
| **Macro avg**         | 0.85      | 0.88   | 0.86     | 2069    |  
| **Weighted avg**      | 0.82      | 0.92   | 0.90     | 2069    |  

---

## 🚀 How It Works  
1. **Data Preprocessing**:  
   - Images were resized, normalized, and augmented to improve model robustness.  

2. **Model Architecture**:  
   - DenseNet-121, known for its compact and efficient design, was used as the base model.  
   - Additional custom classification layers were added for multi-class prediction.  

3. **Training and Evaluation**:  
   - The model was fine-tuned on a labeled dataset of oral disease images.  
   - Evaluated using metrics like accuracy, precision, and recall.  

---

## 🤔 Why DenseNet?  
- **Compact Design**: Fewer layers and better parameter efficiency compared to other architectures.  
- **Feature Propagation**: Directly connects each layer to every other layer, preventing vanishing gradients.  
- **Performance**: Achieved the highest accuracy with faster training times.  

---

## Future Enhancements  
- Expand the dataset to include more diverse and balanced samples.  
- Add interpretability features like Grad-CAM to visualize model focus.  
- Deploy the system as a web or mobile application for real-world use.  

---

