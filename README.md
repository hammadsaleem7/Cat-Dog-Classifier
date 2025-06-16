# 🐶🐱 Cat vs Dog Image Classifier

This project is a deep learning-based image classification model that distinguishes between images of **cats** and **dogs**. It leverages **Convolutional Neural Networks (CNNs)** and **transfer learning** using the **VGG16** model pre-trained on ImageNet.

## 📌 Project Overview

* **Goal:** Build an accurate binary classifier to identify whether an image contains a cat or a dog.
* **Model Used:** VGG16 (pre-trained on ImageNet) with custom top layers.
* **Framework:** TensorFlow / Keras
* **Dataset:** Custom image dataset organized into `train`, `validation`, and `test` directories.
* **Techniques:**

  * ImageDataGenerator for data preprocessing and augmentation
  * Early stopping and model checkpointing to prevent overfitting
  * Visualization of training performance and prediction results

## 🧠 Model Architecture

* **Base Model:** VGG16 with `include_top=False` (feature extraction only)
* **Added Layers:** Flatten → Dense (256, relu) → Dropout → Dense (1, sigmoid)

## 🖼️ Sample Outputs

The model is trained to achieve high accuracy and provides visual feedback on predictions for unseen images.

## 🛠️ Installation & Usage

1. Clone the repo:

   ```bash
   git clone https://github.com/yourusername/cat-dog-classifier.git
   cd cat-dog-classifier
   ```

2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   * Launch Jupyter or Colab and open `Cat_Dog_Classifier.ipynb`
   * Ensure your dataset path is correctly set in the ImageDataGenerator section

## 📊 Results

* **Training Accuracy:** \~99%
* **Validation Accuracy:** \~96%
* The model generalizes well on unseen test data.

## 🚀 Future Improvements

* Deploy the model using Streamlit or Flask
* Train on a larger, more diverse dataset
* Add support for real-time image upload and prediction
