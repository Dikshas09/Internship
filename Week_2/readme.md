# Data Classification Using AI (KNN on Iris Dataset)

This project demonstrates a fundamental Artificial Intelligence and Machine Learning workflow by classifying flower species using the **K-Nearest Neighbors (KNN)** algorithm on the classic **Iris Dataset**.

## 📌 Project Overview
The goal of this project is to predict the specific species of an iris flower based on its physical measurements. The Iris dataset consists of 150 samples from three species of Iris flowers:
*   Iris setosa
*   Iris virginica
*   Iris versicolor

Four features were used to predict these classifications:
1.  Sepal length (cm)
2.  Sepal width (cm)
3.  Petal length (cm)
4.  Petal width (cm)

---

## 🛠️ Technologies & Libraries Used
*   **Python 3**
*   **NumPy & Pandas**: For data manipulation and preprocessing.
*   **Scikit-Learn (sklearn)**: For implementing the KNN model, splitting data, and evaluation.
*   **Matplotlib / Seaborn** *(Optional: keep if you plotted graphs)*: For data visualization.

---

## 🚀 Workflow Implementation

### 1. Data Loading & Exploration
*   Imported the Iris dataset using `sklearn.datasets` or a CSV file.
*   Explored the data structure, shape, and target distributions.

### 2. Data Preprocessing
*   Split the dataset into training and testing sets (typically an 80/20 or 70/30 split) to evaluate model performance accurately.
*   *(Optional)* Standardized/Scaled the features to optimize KNN performance.

### 3. Model Training
*   Initialized the `KNeighborsClassifier`.
*   Trained (fitted) the model using the training feature vectors and corresponding labels.

### 4. Evaluation
*   Predicted classifications on the unseen test data.
*   Evaluated the model using performance metrics such as an **Accuracy Score**, **Confusion Matrix**, and a **Classification Report** (Precision, Recall, F1-Score).

---

## 📈 Results & Performance
*   **Model Accuracy:** [Insert your accuracy here, e.g., 96.67%]
*   The model successfully distinguishes between the three species, showcasing high precision specifically for well-separated clusters like *Iris setosa*.

---

## 🏃 How to Run the Project

1. **Clone the repository:**
```bash
   git clone [https://github.com/Dikshas09/Internship.git](https://github.com/Dikshas09/Internship.git)
   cd Internship/Week_2/Data_Classification_Using_AI
