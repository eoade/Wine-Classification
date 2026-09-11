# Traditional Machine Learning vs Neural Network

# 📌 Project Overview

This project provides a practical demonstration of the relationship between Artificial Intelligence (AI), Machine Learning (ML), Deep Learning (DL), and Neural Networks.

It compares two Machine Learning approaches on the same Wine Quality dataset:

- 🌳 Random Forest — Traditional Machine Learning
- 🧠 Multi-Layer Perceptron (MLP) — Neural Network / Deep Learning approach

The objective is to understand how the two approaches learn patterns and how their performance compares on a classification problem.

---

# 🎯 Project Objective

The project aims to:

1. Explain the relationship between AI, ML, Deep Learning, and Neural Networks.
2. Build a traditional Machine Learning classification model.
3. Build a neural-network-based classification model.
4. Compare their performance using standard evaluation metrics.
5. Understand when traditional ML or neural networks may be more appropriate.

---

# 📊 Dataset

The project uses the Wine Quality dataset.

The dataset contains chemical characteristics of red wine, including:

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

# Target Variable

The original wine quality score was converted into a binary classification:

Quality >= 7  → Good Wine
Quality < 7   → Not Good Wine

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook / Google Colab

---

# 🔄 Project Workflow

Wine Quality Dataset
        ↓
Data Loading
        ↓
Data Preparation
        ↓
Create Classification Target
        ↓
Train/Test Split
        ↓
Feature Scaling
        ↓
 ┌──────────────────┬──────────────────┐
 ↓                  ↓
Random Forest      Neural Network
Traditional ML     Deep Learning
 ↓                  ↓
Prediction         Prediction
 └────────┬─────────┘
          ↓
Performance Evaluation
          ↓
Model Comparison

---

# 🤖 Models

# 1. Random Forest

Random Forest represents the traditional Machine Learning approach.

It combines multiple decision trees to make a final prediction.

rf = RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

# 2. Neural Network

A Multi-Layer Perceptron (MLP) represents the neural-network-based approach.

The model uses two hidden layers:

11 Input Features
       ↓
32 Neurons
       ↓
16 Neurons
       ↓
Output
       ↓
Good / Not Good

Implementation:

nn = MLPClassifier(
    hidden_layer_sizes=(32, 16),
    activation="relu",
    max_iter=1000,
    random_state=42
)

---

# 📈 Evaluation Metrics

The models are compared using:

- Accuracy — Overall percentage of correct predictions.
- Precision — How many predicted positive cases were actually positive.
- Recall — How many actual positive cases were correctly identified.
- F1 Score — Balance between precision and recall.
- Training Time — Time required to train each model.

Confusion matrices are also generated to examine correct and incorrect classifications.

---

# 🧪 Results

The Python notebook automatically generates a performance comparison after training.

Example output format:

Model| Accuracy| Precision| Recall| F1 Score| Training Time
Random Forest| Run code| Run code| Run code| Run code| Run code
Neural Network| Run code| Run code| Run code| Run code| Run code

«Note: Results depend on the environment and model configuration. The values should be taken directly from the experiment rather than manually entered.»

---

# 🧠 Key Learning

The project demonstrates the relationship between the major AI concepts:

Artificial Intelligence
        ↓
Machine Learning
        ↓
Neural Networks
        ↓
Deep Learning

- AI is the broad field of creating intelligent systems.
- Machine Learning allows systems to learn patterns from data.
- Neural Networks are Machine Learning models based on interconnected computational units.
- Deep Learning uses neural networks with multiple layers to learn complex representations.

An important lesson from the project is that Deep Learning is not automatically better than traditional Machine Learning. Model performance depends on the nature, size, and complexity of the data.

---

# ⚠️ Challenges

Some challenges encountered during the project include:

- Preparing the dataset for binary classification.
- Scaling features appropriately for the neural network.
- Selecting suitable model parameters.
- Comparing models fairly using the same test data.
- Interpreting multiple evaluation metrics.
- Understanding why different algorithms can produce different results.

---

# 🚀 Future Improvements

Possible improvements include:

- Hyperparameter tuning.
- Cross-validation.
- Testing Gradient Boosting and Logistic Regression.
- Using a larger dataset.
- Building a deeper neural network.
- Comparing training and validation loss.
- Deploying the best model as a simple prediction application.

---

# 📁 Project Structure

Traditional-ML-vs-Neural-Network/
│
├── README.md
├── wine_quality_ml_vs_nn.ipynb
└── requirements.txt

---

# ▶️ How to Run

# 1. Clone the repository

git clone https://github.com/your-username/Traditional-ML-vs-Neural-Network.git

# 2. Install dependencies

pip install pandas numpy matplotlib scikit-learn

# 3. Open the notebook

Run:

wine_quality_ml_vs_nn.ipynb

The notebook will load the dataset, train both models, evaluate their performance, and generate visualizations.

---

# 🏁 Conclusion

This project demonstrates that traditional Machine Learning and neural networks can solve the same classification problem using fundamentally different learning approaches.

Random Forest learns through an ensemble of decision trees, while the neural network learns through interconnected layers and adjustable weights.

The comparison provides a practical foundation for understanding why Deep Learning has become an important part of modern Artificial Intelligence, while also showing that traditional Machine Learning remains highly valuable for structured datasets.

---

👤 Author

Emmanuel Adegoke

Data Engineering | Machine Learning | Artificial Intelligence

---

📜 License

GNU General Public License v3.0.
