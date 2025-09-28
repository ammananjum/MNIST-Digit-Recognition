# MNIST Handwritten Digit Recognition

## Project Overview
This project demonstrates the implementation of machine learning models to recognize and classify handwritten digits (0–9) from the MNIST dataset. It covers the full ML workflow, including data preprocessing, model training, evaluation, and visualization.

---

## Dataset
- Source: [MNIST dataset via OpenML](https://www.openml.org/d/554)  
- Total samples: 70,000 images (60,000 training, 10,000 testing)  
- Image size: 28x28 pixels (flattened to 784 features for classical ML models)  
- Pixel values: 0–255 (normalized to 0–1 for model input)  

---

## Models Implemented
| Model | Type | Accuracy | Notes |
|-------|------|----------|-------|
| Logistic Regression | Linear | ~90.1% | Baseline model, fast training |
| Random Forest | Ensemble | ~94% | Captures non-linear patterns, slightly slower |
| Support Vector Machine (SVM) | Kernel-based | ~89.6% | Trained on a small subset for computational efficiency |

---

## Key Steps
1. **Data Exploration:** Loaded MNIST, checked shapes, visualized sample digits.  
2. **Preprocessing:** Normalized pixel values, split into training and test sets.  
3. **Baseline Model:** Trained Logistic Regression on a smaller subset to establish baseline accuracy.  
4. **Model Evaluation:** Generated confusion matrix, classification report, and visualized misclassified digits.  
5. **Advanced Model:** Trained Random Forest classifier, compared accuracy with Logistic Regression.  
6. **Training Time Comparison:** Measured training time vs accuracy for Logistic Regression and Random Forest.  
7. **SVM Model:** Trained on small subset, compared performance with other models.  
8. **Final Comparison:** Visualized accuracy vs training time for all models.

---

## Observations
- Random Forest achieved the highest accuracy, capturing complex patterns in the data.  
- Logistic Regression was faster but slightly less accurate.  
- SVM showed reasonable performance on small subsets but is computationally intensive on full data.  
- Visualization of misclassified digits highlighted the types of errors the models make, such as confusing similar digits (e.g., 5 with 3, 9 with 4).  

---

## Conclusion
- Ensemble models like Random Forest provide strong performance for MNIST classification.  
- There is a trade-off between model accuracy and training time.  
- The project demonstrates skills in data preprocessing, classical machine learning models, evaluation metrics, and result visualization, making it suitable for portfolio or internship purposes.  

---

## Repository Contents
- `MNIST_Handwritten_Digit_Recognition.ipynb` — Jupyter notebook containing all code, plots, and explanations.  
- `README.md` — This file, providing an overview and summary of the project.
