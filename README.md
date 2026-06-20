# Arabic Dialect Identification Project

## Overview
This project focuses on **Arabic Dialect Identification (ADI)** using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to automatically classify Arabic text into its corresponding regional dialect.

The project compares the performance of traditional machine learning models with a transformer-based deep learning model (AraBERT) to determine the most effective approach for Arabic dialect classification.

---

## Dataset
The project uses the **IADD (Arabic Dialect Dataset)**, which contains Arabic text samples labeled according to their dialect regions.

Dataset source:
- https://github.com/JihadZa/IADD

---

## Project Workflow

### 1. Data Collection
- Load the IADD dataset
- Explore dialect distribution
- Visualize class frequencies

### 2. Text Preprocessing
The preprocessing pipeline includes:
- Removing non-Arabic characters
- Normalizing Arabic letters
- Removing extra spaces
- Cleaning noisy text

### 3. Traditional Machine Learning Models
Text data is converted into numerical features using:

- TF-IDF Vectorization

The following classifiers are trained and evaluated:

- Logistic Regression
- Support Vector Machine (SVM)

### 4. Deep Learning Model
A transformer-based approach is implemented using:

- AraBERT
- Hugging Face Transformers
- PyTorch

The model is fine-tuned for multi-class dialect classification.

### 5. Evaluation
Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

A final comparison is performed between all models.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- PyTorch
- Hugging Face Transformers
- Datasets Library

---

## Project Structure

```text
Arabic_Dialect_Identification_Project.ipynb
│
├── Data Loading
├── Exploratory Data Analysis
├── Text Preprocessing
├── TF-IDF Feature Extraction
├── Logistic Regression Model
├── SVM Model
├── AraBERT Fine-Tuning
├── Evaluation Metrics
└── Model Comparison
Results

The project compares:

Model	Description
Logistic Regression	Baseline machine learning classifier
SVM	Traditional machine learning classifier
AraBERT	Transformer-based Arabic language model

Performance is measured using classification metrics and visualized through confusion matrices and comparison charts.

How to Run
Clone the Repository
git clone https://github.com/your-username/your-repository.git
cd your-repository
Install Dependencies
pip install pandas numpy matplotlib seaborn scikit-learn torch transformers datasets
Run the Notebook
jupyter notebook Arabic_Dialect_Identification_Project.ipynb
Future Improvements
Experiment with larger Arabic language models
Hyperparameter optimization
Support for additional Arabic dialects
Deploy the model as a web application using Gradio
Author

Ghadeer Alharbi

Master's Student in Data Science
Bachelor's Degree in Information Technology
License

This project is intended for educational and research purposes.
