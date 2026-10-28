# MNIST Handwritten Digit Classification 🧠

A deep learning project that recognizes handwritten digits (0–9) using a feedforward neural network built with TensorFlow and Keras. This project demonstrates an end-to-end deep learning workflow, including data preprocessing, model training, evaluation, and prediction visualization.

## 📌 Project Overview

The objective of this project is to build and train a neural network that can accurately classify handwritten digit images from the MNIST dataset.

The project covers:
- Loading and exploring the MNIST dataset
- Data preprocessing and normalization
- Building a neural network using TensorFlow/Keras
- Understanding forward propagation and backpropagation
- Training and validating the model
- Evaluating model performance using test data
- Visualizing predictions and the confusion matrix

## 📊 Dataset

The MNIST dataset contains 70,000 grayscale images of handwritten digits.

- **Training images:** 60,000
- **Testing images:** 10,000
- **Image dimensions:** 28 × 28 pixels
- **Number of classes:** 10 (digits 0–9)

The dataset is loaded directly using `tf.keras.datasets.mnist.load_data()`.

## 🛠️ Technologies Used

- **Python** — Programming language
- **TensorFlow and Keras** — Neural network development and training
- **NumPy** — Numerical computations
- **Matplotlib** — Data visualization
- **Scikit-learn** — Model evaluation metrics
- **Google Colab** — Cloud-based development environment
- **Jupyter Notebook** — Interactive coding and documentation

## 🧠 Model Architecture

The project uses a feedforward neural network with the following architecture:

1. **Input:** 28 × 28 grayscale images
2. **Flatten Layer:** Converts each image into 784 features
3. **Dense Layer:** 128 neurons with ReLU activation
4. **Dropout Layer:** 20% dropout to help reduce overfitting
5. **Output Layer:** 10 neurons with Softmax activation for digit classification

### Model Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Cross-Entropy |
| Batch Size | 128 |
| Maximum Epochs | 10 |
| Early Stopping | Enabled |
| Output Classes | 10 |

## 📈 Model Performance

The trained model was evaluated on the unseen MNIST test dataset.

| Evaluation Metric | Result |
|---|---:|
| Test Loss | 0.0755 |
| Test Accuracy | 97.47% |

The model achieved **97.47% test accuracy**, demonstrating that a relatively simple feedforward neural network can effectively classify handwritten digits.

## 🔍 Evaluation and Visualization

The Jupyter Notebook includes:

- Sample handwritten digit images
- Training and validation accuracy curves
- Training and validation loss curves
- Classification report with precision, recall, and F1-score
- Confusion matrix
- Actual versus predicted digit visualizations

These visualizations help assess model performance and identify digit classes that may be misclassified.

## ⚙️ How to Run the Project

### Option 1: Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/).
2. Download or clone this repository.
3. Upload `MNIST_Handwritten_Digit_Classification.ipynb` to Colab.
4. Select **Runtime → Run all**.
5. Wait for the dataset to load and the model to train.
6. Review the evaluation metrics, confusion matrix, and prediction visualizations.

The MNIST dataset downloads automatically when the notebook is run for the first time, so an internet connection may be required.

### Option 2: Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/mehakgarg22/mnist-handwritten-digit-classification.git
cd mnist-handwritten-digit-classification
```

**2. Create a virtual environment (recommended)**

```bash
python -m venv .venv
```

Activate it on macOS/Linux:

```bash
source .venv/bin/activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `MNIST_Handwritten_Digit_Classification.ipynb` and run the cells from top to bottom.

## 📁 Project Structure

```text
mnist-handwritten-digit-classification/
│
├── MNIST_Handwritten_Digit_Classification.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 🎯 Key Learnings

Through this project, I explored:

- Fundamentals of artificial neural networks
- Forward propagation and backpropagation
- Data preprocessing and normalization
- Model training, validation, and testing
- Multiclass classification using Softmax
- Loss functions and optimization using Adam
- Model evaluation using accuracy, loss, precision, recall, and F1-score
- Confusion matrices and prediction visualization

## 🚀 Future Improvements

- Implement a Convolutional Neural Network (CNN) for image classification
- Experiment with different neural network architectures
- Tune hyperparameters to improve model performance
- Build an interactive web application for handwritten digit prediction

## 📚 References

- [MNIST Dataset — TensorFlow](https://www.tensorflow.org/datasets/catalog/mnist)
- [TensorFlow Documentation](https://www.tensorflow.org/)
- [Keras Documentation](https://keras.io/)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)

## 👩‍💻 Author

**Mehak Garg**

- GitHub: [@mehakgarg22](https://github.com/mehakgarg22)

---

⭐ If you find this project useful, consider giving the repository a star!
