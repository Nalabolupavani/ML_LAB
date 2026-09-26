Machine Learning Lab – Experiment 3 -  Face Recognition using PCA, KNN and Artificial Neural Network

📖 Introduction

To develop a face recognition system using **Principal Component Analysis (PCA)** for dimensionality reduction, **K-Nearest Neighbors (KNN)** for classification, and an **Artificial Neural Network (ANN)** for face recognition using the Labeled Faces in the Wild (LFW) dataset.

Face recognition involves identifying individuals from facial images. In this experiment, the **LFW (Labeled Faces in the Wild)** dataset is used to demonstrate a complete machine learning workflow for face classification.

The high-dimensional facial images are first normalized and reduced using **PCA with whitening**. The transformed features are then classified using **KNN** and an **ANN implemented with TensorFlow/Keras**.

Workflow

**LFW Dataset → Data Preprocessing → KNN → PCA Whitening → Feature Scaling → ANN → Performance Evaluation**


📊 Dataset

The experiment uses the **Labeled Faces in the Wild (LFW)** dataset.

* Number of images: **3023**
* Image dimensions: **87 × 65**
* Number of features: **5655**
* Number of classes/persons: **62**
* Maximum images selected per person: **50**

The dataset contains facial images belonging to different individuals and is suitable for face recognition experiments.

🛠️ Technologies Used

* Python
* Jupyter Notebook
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* mglearn
* TensorFlow / Keras


🧠 Artificial Neural Network

An ANN is constructed using TensorFlow/Keras with:

* Input layer: 100 features
* Hidden layer 1: 300 neurons, ReLU
* Hidden layer 2: 100 neurons, ReLU
* Output layer: 62 neurons, Softmax


📌 Key Results

| Technique                  |                       Accuracy |
| -------------------------- | -----------------------------: |
| KNN on original features   |                       **0.22** |
| KNN + PCA Whitening        |                       **0.30** |
| ANN + PCA + MinMax Scaling | *As obtained during execution* |


🎓 Learning Outcomes

After completing this experiment, students will be able to:

* Work with real-world facial image datasets.
* Perform image data preprocessing and normalization.
* Apply KNN for face classification.
* Understand dimensionality reduction using PCA.
* Apply PCA whitening to improve feature representation.
* Scale features for neural network training.
* Build an ANN using TensorFlow/Keras.
* Evaluate machine learning model performance.

🚀 Conclusion

This experiment demonstrates an effective face recognition pipeline by combining **PCA for dimensionality reduction**, **KNN for classification**, and **ANN for deep learning-based recognition**. PCA significantly reduces the feature space from **5655 to 100 dimensions**, while improving the KNN performance from **22% to 30%** in the observed experiment.

The experiment provides practical understanding of **computer vision, dimensionality reduction, classical machine learning, and neural networks**.

 👩‍💻 Author

Nalabolu Pavani
III - year
Department of Artificial Intelligence & Data Science
IFET College of Engineering


