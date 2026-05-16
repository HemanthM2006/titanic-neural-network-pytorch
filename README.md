# 🚢 Titanic Survival Prediction using PyTorch Neural Network

### My Second Neural Network & Deep Learning Project using PyTorch

A Deep Learning project that predicts whether a passenger survived the Titanic disaster using a **Feedforward Neural Network implemented from scratch in PyTorch**.

Before this project, I had already built a **Titanic Survival Prediction model using Logistic Regression with scikit-learn**.
This project helped me understand the transition from:

```text id="wmv3rk"
Traditional Machine Learning
→
Deep Learning using Neural Networks
```

and how Neural Networks differ from classical ML models.

---

# 🚀 Project Overview

The goal of this project is to predict Titanic passenger survival using passenger information such as:

```text id="v5t2fa"
(Pclass, Sex, Age, Fare, Family Features, Title Features) → Survived (0 or 1)
```

The neural network learns patterns from passenger attributes and predicts survival probability.

---

# 🔄 From Logistic Regression to Neural Networks

My previous Titanic project used:

```text id="x1p7nl"
Logistic Regression (scikit-learn)
```

This project replaces it with:

```text id="n8u4qw"
Feedforward Neural Network (PyTorch)
```

Key differences I learned:

| Logistic Regression          | Neural Network                  |
| ---------------------------- | ------------------------------- |
| Linear model                 | Non-linear learning             |
| Simpler architecture         | Hidden layers & activations     |
| Limited feature interactions | Learns complex feature patterns |
| Easier to interpret          | More expressive learning        |

This project helped me understand how Deep Learning extends beyond traditional Machine Learning.

---

# 🧠 Concepts Used

This project covers:

* PyTorch Tensors
* Feedforward Neural Networks
* Binary Classification
* Linear Layers
* ReLU Activation
* Sigmoid Function
* Adam Optimizer
* BCEWithLogitsLoss
* Dropout Regularization
* Weight Decay (L2 Regularization)
* Hyperparameter Tuning
* Loss Visualization
* Model Evaluation
* Saving & Loading Model Parameters

---

# 📊 Dataset

The project uses the Titanic passenger dataset.

| Property         | Value                 |
| ---------------- | --------------------- |
| Total Passengers | 891                   |
| Training Split   | 80%                   |
| Test Split       | 20%                   |
| Prediction Type  | Binary Classification |

---

# ⚙️ Data Cleaning & Feature Engineering

The dataset was cleaned and preprocessed before training.

### Included:

* Missing value handling
* Title extraction from names
* Family-based features
* One-hot encoding
* Feature scaling using `StandardScaler()`

Engineered features include:

* FamilyCategory
* IsAlone
* Passenger Titles

---

# 🧠 Neural Network Architecture

```text id="c7m2zy"
12 → 16 → 8 → 1
```

Where:

* 12 → Input features
* 16, 8 → Hidden layers
* 1 → Output neuron

The final output predicts survival probability.

---

# 📉 Loss Function & Optimizer

### Loss Function

```python id="z4n1kg"
nn.BCEWithLogitsLoss()
```

Used for binary classification.

---

### Optimizer

```python id="u9v6rt"
torch.optim.Adam()
```

Used for gradient-based optimization.

---

# 🛡️ Regularization Techniques

The project experimented with:

* Dropout
* Weight Decay (L2 Regularization)
* Different epoch counts

to observe how regularization affects neural network performance.

---

# 💾 Saving & Loading Model Parameters

### Save Trained Model

```python id="y5x2fd"
torch.save(model.state_dict(), "titanic_nn_model.pth")
```

---

### Load Saved Model

```python id="g2m8ql"
model.load_state_dict(torch.load("titanic_nn_model.pth"))
model.eval()
```

The trained model parameters are stored in a `.pth` file, allowing the neural network to be reused later without retraining.

---

# 📈 Final Results

```text id="r6k3pa"
Accuracy ≈ 79.33%
```

The project also includes:

* Training Loss Visualization
* Hyperparameter Experiments
* Neural Network Performance Analysis

---

# 🔍 Key Learning Outcomes

Through this project, I learned:

* How Binary Classification Neural Networks work
* Difference between Logistic Regression and Neural Networks
* How sigmoid converts logits into probabilities
* Importance of preprocessing and feature engineering
* How regularization improves generalization
* How to save and reload trained model parameters
* Real-world PyTorch Deep Learning workflow

---

# 📂 Project Structure

```text id="m4j7hx"
titanic-logistic-regression-vs-neural-network
│
├── titanic_nn.ipynb
├── titanic_nn_model.pth
├── train.csv
├── README.md
```

---

# 🌱 Deep Learning Journey

This project strengthened my understanding of Neural Networks and Deep Learning beyond simple tutorials.

I’m excited to continue learning and building more projects involving:

* Regression Neural Networks
* CNNs
* Computer Vision
* Transformers
* LLMs

---

# 👨‍💻 Built By

**Hemanth M**

Computer Science Student | Machine Learning Enthusiast
