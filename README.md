# Breast Cancer Classification with Neural Network

This project implements a neural network model for breast cancer classification using patient data. The model is trained on a dataset containing features extracted from breast tissue samples and classifies them as **benign** or **malignant**.

##  Features
- Uses **TensorFlow/Keras** to build a deep learning model.
- Implements **data preprocessing**, including encoding categorical labels and feature scaling.
- Handles **class imbalance** using computed class weights.
- Evaluates performance across different **batch sizes** (16, 32, 64).
- Saves trained models for each batch size.

##  Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/breast-cancer-classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd breast-cancer-classification
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

##  Dataset
- The dataset used in this project should be a CSV file (`breast_cancer.csv`).
- It should include numerical features and a target label (`label` column).
- Labels: `0 = Benign`, `1 = Malignant`

##  How to Run
1. Ensure the dataset (`breast_cancer.csv`) is placed in the project directory.
2. Run the script:
   ```bash
   python breast_cancer_with_nn.py
   ```

##  Results
- The script trains a **feedforward neural network** and evaluates accuracy on a test set.
- It visualizes **training accuracy** and **loss curves**.
- Final models are saved as `.h5` files.

##  Model Architecture
- **Input Layer**: Number of features in the dataset
- **Hidden Layers**:
  - Dense (32 neurons, ReLU activation)
  - Dropout (0.3)
  - Dense (16 neurons, ReLU activation)
  - Dropout (0.2)
- **Output Layer**: Dense (1 neuron, Sigmoid activation)

