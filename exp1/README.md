Experiment 1 — Decision Tree Classification on Iris Dataset

**Implementation of Decision Tree Classification using the Iris Dataset**

📖 Introduction

Decision Tree is a **supervised machine learning algorithm** used for both classification and regression tasks.

For classification, a decision tree recursively divides the dataset into smaller subsets using feature-based decision rules. Each internal node represents a decision based on a feature, each branch represents the outcome of that decision, and each leaf node represents the predicted class.

In this experiment, the Decision Tree algorithm is applied to the **Iris dataset** to classify flowers into three species:

* **Setosa**
* **Versicolor**
* **Virginica**

The classification is performed using four morphological features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width


📊 Dataset
Iris Dataset

The Iris dataset is a well-known dataset used for demonstrating machine learning classification techniques.

| Feature      | Description                |
| ------------ | -------------------------- |
| Sepal Length | Length of the sepal in cm  |
| Sepal Width  | Width of the sepal in cm   |
| Petal Length | Length of the petal in cm  |
| Petal Width  | Width of the petal in cm   |
| Species      | Target class of the flower |

Target Classes

The model predicts one of the following three classes:

```text
Setosa
Versicolor
Virginica
```

🛠️ Technologies and Libraries

The experiment is implemented using **Python 3** and the following libraries:

* **Pandas** — Data loading and manipulation
* **NumPy** — Numerical operations
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization and pair plotting
* **Scikit-learn** — Machine learning model, data splitting and evaluation
* **PydotPlus** — Decision tree visualization
* **Graphviz** — Graphical representation of the decision tree
* **Jupyter Notebook** — Interactive development environment

🔄 Experiment Workflow

The experiment follows these major steps:

```text
                 Iris Dataset
                      │
                      ▼
              Load Dataset
                      │
                      ▼
            Explore the Dataset
                      │
                      ▼
        Check Missing Values & Data Types
                      │
                      ▼
             Statistical Analysis
                      │
                      ▼
              Pair Plot Analysis
                      │
                      ▼
          Train-Test Data Splitting
                      │
                      ▼
          Train Decision Tree Model
                      │
                      ▼
             Predict Test Data
                      │
                      ▼
           Model Evaluation
                      │
              ┌───────┴────────┐
              ▼                ▼
     Classification Report  Confusion Matrix
              │
              ▼
       Visualize Decision Tree
              │
              ▼
       Predict New Flower Data

 🌳 How the Decision Tree Works

A decision tree makes predictions by following a sequence of feature-based conditions.

For example:

```text
Is Petal Length <= threshold?
           │
       ┌───┴───┐
      Yes      No
       │        │
   Setosa    Another test
                │
          ┌─────┴─────┐
       Versicolor  Virginica
```

The algorithm selects feature thresholds that provide good separation between the classes.

Result

The class predicted is --> setosa

Therefore, based on the given measurements, the Decision Tree classifier predicts the flower as:

**Setosa**

---
📈 Results

The experiment successfully demonstrates the complete machine learning workflow:

* Dataset loading
* Data exploration
* Missing-value analysis
* Statistical analysis
* Feature relationship visualization
* Training and testing data preparation
* Decision Tree model training
* Test-set prediction
* Classification performance evaluation
* Confusion matrix visualization
* Decision Tree visualization
* Prediction of new unseen data

The model successfully predicts the class of the given flower sample as **Setosa**.

---

🎓 Learning Outcomes

After completing this experiment, the following concepts are demonstrated:

1. Understand the fundamentals of **supervised machine learning**.
2. Understand the working principle of a **Decision Tree Classifier**.
3. Load and explore a real-world dataset using **Pandas**.
4. Perform exploratory data analysis using statistical methods.
5. Visualize feature relationships using **Seaborn pair plots**.
6. Divide data into training and testing subsets.
7. Train a classification model using **Scikit-learn**.
8. Evaluate a classification model using precision, recall and F1-score.
9. Interpret a **confusion matrix**.
10. Visualize the structure of a Decision Tree.
11. Use a trained model to classify new, unseen observations.


🔬 Experiment Summary

| Component             | Description                                |
| --------------------- | ------------------------------------------ |
| Algorithm             | Decision Tree Classifier                   |
| Learning Type         | Supervised Learning                        |
| Problem Type          | Multi-class Classification                 |
| Dataset               | Iris Dataset                               |
| Number of Classes     | 3                                          |
| Input Features        | 4                                          |
| Training Size         | 90%                                        |
| Testing Size          | 10%                                        |
| Evaluation            | Classification Report                      |
| Visualization         | Pair Plot, Confusion Matrix, Decision Tree |
| New Sample Prediction | Setosa                                     |


🚀 Conclusion

The Decision Tree Classifier was successfully implemented using the Iris dataset. The experiment demonstrated the complete machine learning pipeline, starting from dataset exploration and visualization to model training, evaluation, tree visualization, and prediction of new observations.

The experiment provides a practical understanding of how **Decision Tree classification** can be used to learn decision rules from labelled data and make predictions for unseen samples.


👩‍💻 Author

Nalabolu Pavani
III - year
Department of Artificial Intelligence and Data Science



