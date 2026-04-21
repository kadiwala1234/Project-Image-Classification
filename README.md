**Image Classification using Random Forest & SVM**

**Project Overview**

This project implements an image classification system using traditional machine learning techniques: Random Forest and Support Vector Machine (SVM). The goal is to classify images into different categories after preprocessing them into feature vectors.

**The project includes:**

Image preprocessing (resize, normalization, flattening)
Model training using Random Forest with GridSearchCV
Model training using SVM with GridSearchCV
Performance evaluation and comparison
Feature importance visualization
Prediction on new unseen images
Dataset

The dataset consists of labeled images organized in folder structure:

images/
 ├── pizza/
 ├── dalmatian/
 ├── dollar_bill/

Each folder represents a class label.

Installation

Install the required libraries:

pip install numpy opencv-python matplotlib seaborn scikit-learn
How to Run
1. Clone the repository
git clone https://github.com/kadiwala1234/image-classification-ml.git
cd image-classification-ml
2. Open Jupyter Notebook or Google Colab
Image Classification.ipynb file
Or upload it to Google Colab
3. Upload Dataset

Unzip the dataset:

import zipfile

with zipfile.ZipFile("images.zip", 'r') as zip_ref:
    zip_ref.extractall("images")

4. Run the Notebook
Execute all cells in order:

Preprocessing
Model training
Evaluation
Prediction
Models Used
Random Forest Classifier
Optimized using GridSearchCV
Parameters tuned:
n_estimators
max_depth
min_samples_split
min_samples_leaf
Support Vector Machine (SVM)
Kernel types tested: linear, RBF
Hyperparameter tuning using GridSearchCV
Evaluation Metrics

Models are evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Results
Model	         Accuracy	   Notes
Random Forest	 0.77%	     Stable and fast
SVM	           0.84%	     Good but slower

Features
Image preprocessing pipeline
Hyperparameter tuning using GridSearchCV
Feature importance visualization
Prediction function for new images
Model comparison (RF vs SVM)
Prediction Example
predict_image("test.jpg", best_model)
Output:
sunflower

Visualizations
Confusion Matrix Heatmap
Feature Importance Bar Plot
Model performance comparison
Future Improvements
Replace ML models with CNN (Deep Learning)
Improve accuracy using data augmentation
Deploy using Flask or Streamlit
Convert into real-time image classification app

Author
Project developed as part of Machine Learning assignment
Tools: Python, OpenCV, Scikit-learn, Matplotlib

License
This project is for educational purposes only.
