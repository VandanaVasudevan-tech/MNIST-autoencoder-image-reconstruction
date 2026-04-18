# MNIST-autoencoder-image-reconstruction
A deep learning autoencoder built using the MNIST dataset to learn latent representations and reconstruct handwritten digit images.
# 🧠 MNIST Autoencoder for Image Reconstruction

## 📌 Overview

This project implements a **basic Autoencoder** using Deep Learning techniques to learn compressed representations of handwritten digits from the **MNIST dataset** and reconstruct them.

An autoencoder is an unsupervised neural network that consists of:

* **Encoder** → Compresses the input image into a lower-dimensional latent space
* **Decoder** → Reconstructs the original image from the compressed representation

---

## 🎯 Objective

* Build and train an autoencoder model
* Learn latent representations of image data
* Reconstruct handwritten digit images
* Evaluate model performance using loss curves and visual comparison

---

## 🗂️ Dataset

* **Dataset Used:** MNIST Handwritten Digits
* **Image Size:** 28 × 28 grayscale images
* **Training Samples:** 60,000
* **Test Samples:** 10,000

---

## ⚙️ Model Architecture

### 🔹 Encoder

* Input Layer: 28 × 28 image
* Flatten Layer
* Dense Layer (64 neurons, ReLU)
* Dense Layer (32 neurons, ReLU) → *Latent Representation*

### 🔹 Decoder

* Dense Layer (64 neurons, ReLU)
* Dense Layer (784 neurons, Sigmoid)
* Reshape to 28 × 28 image

---

## 🏋️ Training Details

* **Loss Function:** Binary Crossentropy
* **Optimizer:** Adam
* **Epochs:** 20
* **Batch Size:** 256
* **Validation:** Test dataset

---

## 📊 Results

### ✅ Loss Curve

* Training and validation loss decrease steadily
* Indicates effective learning without major overfitting

### ✅ Reconstruction Quality

* Reconstructed images closely resemble original digits
* Slight blurriness due to compression in latent space

---

## 🖼️ Output Visualization

The model output includes:

* 📉 Training vs Validation Loss Graph
* 🔄 Side-by-side comparison:

  * Original Images
  * Reconstructed Images

---

## 📁 Project Structure

```
mnist-autoencoder-image-reconstruction/
│
├── assignment11.ipynb        # Main implementation
├── README.md                # Project documentation

```

---

## 🚀 How to Run

### 1. Clone Repository

```bash
git clone https://github.com/your-username/mnist-autoencoder-image-reconstruction.git
cd mnist-autoencoder-image-reconstruction
```

### 2. Install Dependencies

```bash
pip install numpy matplotlib tensorflow
```

### 3. Run the Notebook

* Open in Jupyter Notebook / Google Colab
* Run all cells

---

## 💡 Key Learnings

* Understanding of encoder–decoder architecture
* Working with image data in neural networks
* Dimensionality reduction using latent space
* Visualization of deep learning model performance

---

## 📌 Conclusion

This project demonstrates how autoencoders can effectively learn compressed representations of images and reconstruct them with good accuracy. It highlights the power of unsupervised learning in feature extraction and data compression.

---


