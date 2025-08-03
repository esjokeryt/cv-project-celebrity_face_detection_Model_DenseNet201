📌 CV Project – Multi-Class Image Classification with Transfer Learning
This project is a computer vision pipeline designed for multi-class image classification using transfer learning and fine-tuning. The dataset includes 16 distinct classes (from -1 to 14), and the model is trained and evaluated based on accuracy, F1 score, and Top-2 accuracy.

📂 Contents
Data loading and preprocessing

Label encoding and one-hot encoding

Transfer learning using pretrained networks (EfficientNet)

Fine-tuning and unfreezing top layers

Training with learning rate schedulers and class weights

Validation using confusion matrix and classification report

Final test prediction and submission file creation

🚀 Technologies Used
Python

TensorFlow / Keras

Scikit-learn

NumPy

Matplotlib

📊 Model Training Steps
Configuration Setup
Define batch size, learning rate, input shape, and other training parameters.

Data Preparation

Load images and labels.

Encode labels using LabelEncoder.

Apply one-hot encoding for categorical output.

Splitting Dataset

Split the data into training and validation sets using stratified sampling.

Model Architecture

Use a pretrained EfficientNet model (e.g., EfficientNetB0).

Freeze base layers initially.

Add custom classification head.

Training Phase 1 – Feature Extraction

Train only the custom layers.

Apply callbacks: ModelCheckpoint, ReduceLROnPlateau, and EarlyStopping.

Training Phase 2 – Fine-Tuning

Unfreeze top layers of the base model.

Re-compile with a smaller learning rate.

Continue training to improve performance.

📈 Evaluation Metrics
Accuracy

Weighted F1 Score

Top-2 Accuracy

Confusion Matrix

Classification Report

🧪 Final Prediction & Submission
Load and preprocess test images.

Predict class probabilities using the trained model.

Decode predicted labels (from one-hot back to original label).

Save the submission file in CSV format for competition or evaluation.

### 📥 Dataset
Dataset used in this project is from Kaggle competition:
[S-2025 Multi-Class Pretrained Network Project](https://www.kaggle.com/competitions/s-2025-multi-class-pretraied-network-project/overview)
