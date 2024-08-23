# Exploring-Textual-Data-Analysis-Using-SpaCy
Exploring Textual Data Analysis with SpaCy

# Project 2: Exploring Textual Data Analysis Using SpaCy

## Overview
This project involved exploring textual data analysis using SpaCy and other machine learning models. The project included data preprocessing, model selection, training, performance evaluation, and analysis of results.

## Project Structure

### 1. Data Preprocessing with SpaCy
- Utilized SpaCy for text preprocessing tasks such as:
  - Tokenization
  - Lemmatization
  - Removing stop words
- Ensured the dataset was cleaned and prepared for modeling.

### 2. Model Selection and Group Formation

- **Model Selection**:
  - two models for classification 
  
### 3. Model Training and Hyperparameter Tuning
- Trained selected models on the preprocessed data.
- Each model was trained with two hyperparameters, and each hyperparameter was tested with two different values.
- For classification tasks:
  - Ensured at least one model utilized SpaCy for classification.
  - Other models included algorithms like SVM, Random Forest, or Neural Networks.
- For clustering tasks:
  - Considered models like K-means, DBSCAN, or hierarchical clustering.

### 4. Classification Models

#### 1. Regression with SpaCy Embeddings

- **Initial Hyperparameters:**
  - Regularization Strength: 0.1 and 1.0
  - Penalty: l1 and l2

- **Adjusted Hyperparameters:**
  - Regularization Strength: 0.1, 0.5, 1.0 (previously applied 0.1 and 1.0)
  - Penalty: No changes
  - Solver: Added `saga`
  - Maximum number of iterations: Added `100`

#### 2. Support Vector Machine (SVM)

- **Initial Hyperparameters:**
  - Regularization Parameter: 0.1 and 1.0
  - Kernel: linear and rbf

- **Adjusted Hyperparameters:**
  - Regularization Parameter: 0.1, 0.5, 1.0 (previously applied 0.1 and 1.0)
  - Kernel: Added `poly` (previously applied linear and rbf)
  - Gamma: `auto`
  - Degree: `2, 3`
  - Coefficient (for poly): `0.5, 1.0`

### Analysis and Conclusion

The dataset used in this project was relatively simple, containing only three emotion categories. This simplicity facilitated the models' learning process, allowing them to classify the emotions effectively, which was reflected in the decent performance of both the Logistic Regression and SVM models.

The limited number of labels may have restricted the models' depth of understanding and their ability to generalize to more complex emotional nuances. However, this characteristic allowed the models to achieve reasonable accuracy without the need for overly complex architectures or extensive preprocessing.

Upon evaluating the models, it was observed that the SVM model outperformed Logistic Regression across all performance metrics. This indicates that SVM had a superior ability to capture the underlying patterns in the data, especially after fine-tuning the hyperparameters.

The use of SpaCy embeddings was beneficial in achieving reasonable results for both models. The embeddings were particularly helpful for Logistic Regression, which is a simpler model and benefits significantly from well-prepared data.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Thanks to the SpaCy development team for their powerful NLP library.
- Special thanks to [Your Instructor's Name] for guidance throughout this project.
