# Image Super-Resolution Using SRCNN

## 📜 Project Overview
This project aims to develop a **machine learning-based super-resolution model** to restore low-resolution images to their original quality. The approach leverages the **Super-Resolution Convolutional Neural Network (SRCNN)** to enhance image resolution, making it suitable for various applications, including image restoration and enhancement.

---

## 🎯 Objectives
1. Acquire random low-resolution images and restore their quality.  
2. Simulate low-resolution images using blurring and undersampling techniques.  
3. Train an SRCNN model to enhance image quality effectively.

---

## 🖼️ Data Collection
- **Size**: 100 images.  
- **Diversity**: Includes various categories to ensure model robustness.  
- **Source**: Random images downloaded from the internet.

---

## 🔧 Image Preprocessing
1. **Blurring**: Applied Gaussian blur to simulate reduced quality.  
2. **Undersampling**: Reduced the number of pixels to mimic low-resolution images.

These preprocessing steps created paired datasets of low-resolution and high-resolution images for training.

---

## 🧠 Model Architecture
**Super-Resolution Convolutional Neural Network (SRCNN)**:  
- **Input Layer**: Accepts RGB images (shape: `(None, None, 3)`).  
- **Convolutional Layers**:  
  - Layer 1: 64 filters, kernel size 9x9, ReLU activation.  
  - Layer 2: 32 filters, kernel size 1x1, ReLU activation.  
  - Layer 3: 3 filters, kernel size 5x5, linear activation (output RGB image).  

---

## 🏋️ Training Details
- **Framework**: Google Colab.  
- **Dataset**: Paired low-resolution and high-resolution images.  
- **Optimizer**: Adam.  
- **Loss Function**: Mean Squared Error (MSE).  
- **Evaluation Metric**: Peak Signal-to-Noise Ratio (PSNR).  
- **Hyperparameters**:  
  - Epochs: 10.  
  - Batch Size: 32.  

---

## 📊 Results
- **Model Performance**: Achieved 67.68% accuracy based on evaluation metrics.  
- **Visual Comparisons**: Demonstrated clear improvements in resolution with examples of low-resolution, high-resolution, and restored images.

---

## 🛠️ Installation and Usage

### Prerequisites
- Python 3.8 or higher.  
- Required libraries: TensorFlow, NumPy, Matplotlib.  

### Steps:
1. Clone this repository:
   ```bash
   git clone <repository_url>
