# Texture Feature Classification

This project develops and evaluates machine learning models for classifying images based on texture features. The dataset contains natural images of **grass**, **sand**, and **stairs**, and the goal is to determine which classifier best distinguishes between these categories using extracted image features.

## 📁 Dataset

- **Source**: Images are collected from [Unsplash](https://unsplash.com/)
- **Classes**: `grass`, `sand`, `stairs`
- **Size**: 185 images
- **Preprocessing**:
  - Resized to a uniform size
  - Converted to grayscale
  - Quantized into 8 levels

## 🧠 Features

A total of **10 features** were extracted from each image, primarily using the **Gray-Level Co-occurrence Matrix (GLCM)**, which captures key texture properties without relying on raw pixel values.

## 🔍 Machine Learning Models

Three classifiers were implemented and compared:

- **Ridge Classifier**
- **Random Forest**
- **Multi-Layer Perceptron (MLP)**

### Training & Evaluation:

- **Hyperparameter Tuning**: Performed using `GridSearchCV` with **5-fold Stratified Cross-Validation**
- **Performance Estimation**: Used **Nested Cross-Validation** (4-fold inner, 5-fold outer)
- **Metrics**: Accuracy and Confusion Matrix

## 📊 Results

- All models were evaluated on classification accuracy.
- Random Forest included feature importance analysis to interpret the results.

## 🧪 Project Structure

1. Data preparation and preprocessing
2. Feature extraction
3. Model training and hyperparameter tuning
4. Cross-validation and performance evaluation
5. Results discussion and conclusion

## 🛠 Technologies Used

- Python
- NumPy, Pandas, Matplotlib
- Scikit-learn
- OpenCV (for image processing)

## 👩‍💻 Author

**Ayesha Sultana**  
📧 [mst.ayesha1702@gmail.com] 
- Course: *Machine Learning and Pattern Recognition* - 2025
- University of Turku, Finland
