# 🧬 U-Net for Biomedical Image Segmentation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Joseph1997-eng/U-Net/blob/main/UNet_Assignment.ipynb)

---

## 📘 Project Overview

This project implements a **U-Net architecture** for **biomedical image segmentation**, focusing on **neuron labeling** using electron microscopy data.  

Unlike GAN-based models, U-Net performs **supervised learning**, mapping input images to corresponding segmentation masks. This architecture forms the basis of the **generator** used in the **Pix2Pix** model (covered in the next module).

> 🧠 In short, this is a *neural network for neural tissue segmentation!*

---

## 🎯 Goals

1. Implement your own **U-Net** architecture from scratch.  
2. Observe the U-Net’s performance on a **challenging biomedical segmentation** task.  

---

## 🧩 Learning Objectives

- Understand the **contracting (encoder)** and **expanding (decoder)** paths of U-Net.  
- Build key components such as:
  - Contracting Blocks  
  - Expanding Blocks  
  - Cropping Function  
  - Feature Mapping Layer  
- Train and evaluate the full **U-Net** model on real microscopy data.

---

## 🧠 Dataset

The dataset used is an **Electron Microscopy Neuron Segmentation Dataset** from:

> Arganda-Carreras et al., *“Crowdsourcing the creation of image segmentation algorithms for connectomics”*,  
> *Frontiers in Neuroanatomy (2015)*  
> [🔗 Dataset Information](https://www.ini.uzh.ch/~acardona/data.html)

Each image is paired with a corresponding labeled mask for neuron segmentation.

![Dataset Example](Neuraldatasetexample.png)

---

## ⚙️ U-Net Architecture Overview

The **U-Net** model, introduced by *Ronneberger et al. (2015)*, is a convolutional neural network designed for **semantic segmentation** of biomedical images.

It consists of:
- A **contracting path** (encoder): captures context using convolution and pooling.
- An **expanding path** (decoder): enables precise localization via upsampling and skip connections.

![U-Net Architecture](https://drive.google.com/uc?export=view&id=1XgJRexE2CmsetRYyTLA7L8dsEwx7aQZY)

---

## 🚀 How to Run

### 🧑‍💻 Option 1: Run in Google Colab  
Click below to open the notebook in Colab:  
👉 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Joseph1997-eng/U-Net/blob/main/UNet_Assignment.ipynb)

### ⚙️ Option 2: Run Locally
Clone the repository and install dependencies:

```bash
git clone https://github.com/Joseph1997-eng/U-Net.git
cd U-Net
pip install torch torchvision matplotlib scikit-image tqdm
