 Machine Learning Lab – Experiment 2 - SMS Spam Classification using Support Vector Machine (SVM)


**SMS Spam Detection using Support Vector Machine with Count Vectorization**

📖 Introduction

Spam messages are unsolicited or unwanted messages that may contain advertisements, fraudulent content, promotional offers, or malicious links. Automatically identifying such messages is an important application of **Machine Learning and Natural Language Processing (NLP)**.

In this experiment, an SMS spam dataset is used to build a binary classification model. The textual messages are converted into numerical feature vectors using **CountVectorizer**, and an **SVM classifier with an RBF kernel** is trained to distinguish between legitimate (**Ham**) and unwanted (**Spam**) messages.

The experiment demonstrates a complete machine learning workflow:

**Data Loading → Data Exploration → Visualization → Feature Extraction → Train-Test Split → SVM Classification → Accuracy Evaluation**

🧠 Learning Objectives

By completing this experiment, students will learn to:

* Load and explore a real-world text dataset.
* Perform basic dataset preprocessing.
* Visualize the distribution of Spam and Ham messages.
* Separate input features and target labels.
* Convert text into numerical features using `CountVectorizer`.
* Split the dataset into training and testing sets.
* Implement Support Vector Machine classification.
* Evaluate the performance of a classification model using accuracy.
* Understand the application of machine learning to text classification.

 📊 Dataset

The experiment uses an **SMS Spam Collection dataset** containing labeled SMS messages.

The dataset contains two important attributes:

| Column     | Description                   |
| ---------- | ----------------------------- |
| `Category` | Target label: `spam` or `ham` |
| `Message`  | Actual SMS text               |

Example

| Category | Message                               |
| -------- | ------------------------------------- |
| ham      | Ok, see you tomorrow                  |
| spam     | Congratulations! You have won a prize |


🛠️ Technologies Used

* **Python 3**
* **Jupyter Notebook / JupyterLab**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**


📦 Python Libraries

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.feature_extraction.text import CountVectorizer
from sklearn.model_selection import train_test_split
from sklearn.svm import SVC
```


🤖 Support Vector Machine Classification

An SVM classifier with an **RBF (Radial Basis Function) kernel** is used.

```python
classifier = SVC(
    kernel='rbf',
    random_state=0
)

classifier.fit(X_train, y_train)
```
Why SVM?

Support Vector Machine is effective for classification problems, particularly when the feature space is high-dimensional. Text classification naturally produces a large number of features, making SVM a suitable algorithm for this application.

RBF Kernel

The RBF kernel enables SVM to model nonlinear decision boundaries between different classes.



Accuracy

Accuracy represents the proportion of correctly classified messages:

**Accuracy = Correct Predictions / Total Predictions**


💡 Key Concepts Demonstrated

| Concept             | Application                      |
| ------------------- | -------------------------------- |
| Supervised Learning | Spam/Ham classification          |
| Text Classification | SMS message categorization       |
| Feature Extraction  | CountVectorizer                  |
| Train-Test Split    | Model development and evaluation |
| SVM                 | Classification algorithm         |
| RBF Kernel          | Nonlinear classification         |
| Data Visualization  | Spam/Ham distribution            |
| Accuracy            | Model performance evaluation     |


🎓 Learning Outcomes

After completing this experiment, students will be able to:

1. Understand the fundamentals of text classification.
2. Perform basic preprocessing of an SMS dataset.
3. Extract numerical features from textual data.
4. Apply the Support Vector Machine algorithm.
5. Visualize categorical data distributions.
6. Split data into training and testing sets.
7. Evaluate classification performance using accuracy.
8. Identify and correct errors in feature-target assignment.

 🔬 Result

The SMS dataset was successfully analyzed and prepared for machine learning classification. Text messages were converted into numerical representations using **CountVectorizer**, and an **SVM classifier with an RBF kernel** was implemented for Spam/Ham classification.

The experiment also demonstrates the importance of correctly identifying the **input feature (`Message`)** and **target label (`Category`)** when building a supervised machine learning model.

 🚀 Conclusion

This experiment demonstrates the practical application of **Support Vector Machine for SMS Spam Detection**. By combining text feature extraction using **CountVectorizer** with an **RBF-kernel SVM**, textual messages can be transformed into machine-readable representations and classified into Spam or Ham categories.

The experiment provides hands-on experience with the complete machine learning pipeline, from dataset exploration and visualization to feature extraction, model training, and evaluation.


Author

Nalabolu Pavani
III - year
Department of Artificial Intelligence & Data Science
IFET College of Engineering


