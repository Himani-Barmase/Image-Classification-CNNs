# Image-Classification-CNNs
This repository contains a complete implementation of an image classification project using Convolutional Neural Networks (CNNs) on the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html). The objective is to build, train, evaluate, and improve a CNN model to classify images into 10 distinct categories.
📚 Dataset
**CIFAR-10** contains 60,000 32x32 color images in 10 different classes:
- airplane ✈️
- automobile 🚗
- bird 🐦
- cat 🐱
- deer 🦌
- dog 🐶
- frog 🐸
- horse 🐎
- ship 🚢
- truck 🚛

Split: 50,000 training images + 10,000 test images.

---

## ✅ Tasks Completed

### 🔍 Task 1: Data Exploration & Preparation
- Loaded and visualized sample images with labels.
- Normalized pixel values to [0, 1].
- Converted labels to one-hot encoding.
- Split training data into training (80%) and validation (20%).

### 🏗️ Task 2: CNN Model Design & Training
- Built a CNN with:
  - 3x Conv2D + ReLU + MaxPooling2D + Dropout
  - Flatten + Dense + Softmax layers
- Compiled using categorical crossentropy and `Adam` optimizer.
- Trained over 15 epochs and plotted accuracy/loss curves.

### 📊 Task 3: Evaluation
- Achieved high test accuracy (~75–80%).
- Generated a confusion matrix and classification report.
- Displayed examples of both correctly and incorrectly classified images.

### 🔁 Task 4: Optimizer Experimentation
- Compared model performance using:
  - `Adam`
  - `RMSprop`
  - `SGD`
- Logged validation accuracies for comparison.

---

## 🧠 Model Summary
Conv2D(32) → ReLU → MaxPooling → Dropout
Conv2D(64) → ReLU → MaxPooling → Dropout
Conv2D(128) → ReLU → MaxPooling → Dropout
Flatten → Dense(128) → Dropout → Output(10 classes, Softmax)

yaml
Copy
Edit

---

## 📈 Results

- **Best Accuracy Achieved:** ~78% on test data  
- **Confusion Matrix:** Visualized with `scikit-learn`  
- **Optimizer Comparison:** RMSprop provided slightly better generalization than SGD

---

## 🛠️ Technologies Used

| Tool            | Purpose                           |
|-----------------|-----------------------------------|
| Python          | Programming Language              |
| TensorFlow/Keras| CNN model and training            |
| NumPy           | Numerical operations              |
| Matplotlib      | Data visualization                |
| scikit-learn    | Confusion matrix, classification  |

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/cifar10-cnn-classification.git
cd cifar10-cnn-classification
