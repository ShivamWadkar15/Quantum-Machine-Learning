# Quantum-Machine-Learning
📌 README: Quantum Machine Learning (QML) for MNIST Classification 🚀
📖 Project Overview
This project explores Quantum Machine Learning (QML) by using a Quantum Neural Network (QNN) to classify handwritten digits (5 and 9) from the MNIST dataset. It integrates Quantum Computing with Deep Learning using TensorFlow Quantum (TFQ) and Cirq, creating a hybrid quantum-classical model.

📌 Technologies Used
TensorFlow Quantum (TFQ) – To integrate quantum circuits with TensorFlow.
Cirq – To create and simulate quantum circuits.
TensorFlow – For deep learning and model training.
NumPy – For handling numerical data.
Scikit-learn – For dataset splitting.
Matplotlib – For plotting accuracy and results.
📌 Project Workflow
1️⃣ Load and Preprocess Data
The MNIST dataset (handwritten digits 0-9) is used.
Only digits 5 and 9 are selected for binary classification.
The labels are converted to binary format (5 → 1, 9 → 0).
2️⃣ Convert Images to Binary
Each grayscale image is converted into 0s and 1s.
Pixels greater than 0.5 → 1, otherwise 0.
3️⃣ Encode Data into Quantum Circuits
Each binary pixel is mapped to a quantum qubit.
If a pixel is 1, an X gate is applied to the corresponding qubit.
4️⃣ Build the Quantum Neural Network (QNN)
A Quantum Circuit is designed using Cirq.
Parameterized Quantum Gates are applied to enable learning.
The quantum model is integrated with TensorFlow.
5️⃣ Train the Quantum Model
The model is trained using Binary Cross-Entropy Loss and Adam Optimizer.
It is trained for 20 epochs, with accuracy measured at each step.
6️⃣ Evaluate & Analyze the Model
Training and validation accuracy are compared.
Accuracy graphs are plotted over multiple epochs.
Performance is analyzed for overfitting/underfitting.
📌 Expected Outcomes
The Quantum Neural Network should achieve around 80-90% accuracy.
Accuracy stabilizes after a few epochs due to quantum circuit limitations.
The model should perform similarly to classical machine learning models.
