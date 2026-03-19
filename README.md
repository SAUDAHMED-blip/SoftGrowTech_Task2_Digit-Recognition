# SoftGrowTech_Task2_Digit-Recognition
Handwritten Digit Recognition using CNN and TensorFlow on the MNIST dataset. This project trains a deep learning model to accurately classify digits (0–9) with high accuracy and visualizes predictions using Matplotlib.
# 🧠 Handwritten Digit Recognition using CNN

This project implements a **Handwritten Digit Recognition System** using a **Convolutional Neural Network (CNN)** built with TensorFlow and Keras.
The model is trained on the **MNIST dataset**, which contains thousands of labeled handwritten digit images (0–9).

---

## 🚀 Features

* 📊 Uses MNIST dataset for training and testing
* 🧠 Deep Learning model using CNN
* ⚡ Fast and efficient training
* 📈 Accuracy evaluation on test data
* 🖼️ Visualizes predictions with actual vs predicted labels

---

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib

---

## 📦 Installation

First, clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

Install required dependencies:

```bash
pip install tensorflow matplotlib numpy
```

---

## 📂 Project Workflow

### 1. Load Dataset

* Uses built-in MNIST dataset from TensorFlow

### 2. Data Preprocessing

* Normalize pixel values (0–255 → 0–1)
* Reshape images for CNN input (28x28x1)

### 3. Model Architecture

* Conv2D (32 filters)
* MaxPooling
* Conv2D (64 filters)
* MaxPooling
* Flatten
* Dense (128 neurons)
* Output Layer (10 classes)

---

## 🏋️ Model Training

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Epochs: 5

---

## 📊 Results

* Achieves high accuracy on test data (~98% depending on training)
* Displays predictions with actual labels

---

## 🖼️ Sample Output

The model predicts handwritten digits and displays:

```
Predicted: 7, Actual: 7
Predicted: 2, Actual: 2
```

---

## 📌 Code Snippet

```python
model = models.Sequential([
    layers.Conv2D(32, (3,3), activation='relu', input_shape=(28,28,1)),
    layers.MaxPooling2D((2,2)),

    layers.Conv2D(64, (3,3), activation='relu'),
    layers.MaxPooling2D((2,2)),

    layers.Flatten(),
    layers.Dense(128, activation='relu'),
    layers.Dense(10, activation='softmax')
])
```

---

## 🎯 Future Improvements

* 🔍 Add real-time digit recognition using webcam
* 🌐 Deploy as a web app (Flask / Streamlit)
* 📱 Convert to mobile app using TensorFlow Lite
* 📊 Add confusion matrix and performance metrics

---

## 🤝 Contributing

Feel free to fork this repository and contribute by submitting a pull request.


## 👨‍💻 Author

**Saud Ahmed**
BS Artificial Intelligence Student

---

## ⭐ Support

If you like this project, don’t forget to ⭐ the repository!
