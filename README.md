# py_mnistVgg

> 基于 VGG 神经网络的 MNIST 手写数字识别系统，并结合 OpenCV 实现数字图片识别。  
> A VGG-based handwritten digit recognition system for MNIST with OpenCV-based image preprocessing and digit image recognition.

---

# 项目简介 | Introduction

本项目是本科毕业设计（Graduation Project）的实现代码，采用 **VGG（Visual Geometry Group）卷积神经网络** 对 MNIST 手写数字数据集进行训练，并利用 **OpenCV** 对用户上传的数字图片进行预处理和识别。

项目主要包含：

* MNIST 数据集训练
* VGG 网络模型搭建
* 模型训练与测试
* OpenCV 图像预处理
* 自定义数字图片识别

This project is the implementation of my undergraduate graduation project. It uses a **VGG Convolutional Neural Network** for handwritten digit recognition on the MNIST dataset and integrates **OpenCV** for image preprocessing and uploaded digit image recognition.

---

# 功能特点 | Features

* ✅ VGG CNN architecture for digit classification
* ✅ MNIST handwritten digit recognition
* ✅ Model training and evaluation
* ✅ OpenCV image preprocessing
* ✅ Custom digit image recognition
* ✅ Python implementation

---

# 网络结构 | Network Architecture

The project adopts a VGG-style convolutional neural network consisting of:

* Convolution Layers
* ReLU Activation
* MaxPooling Layers
* Fully Connected Layers
* Softmax Output

The network is trained on the MNIST handwritten digit dataset for classification of digits **0–9**.

---

# 项目结构 | Project Structure

```
py_mnistVgg/
│
├── paint_board.py         # Handwritten digit drawing board
├── target_detection.py    # Digit detection and preprocessing
├── vgg_training.py        # VGG model training
├── vgg_testing.py         # VGG model evaluation
├── vgg_main.py            # Main application entry
├── vgg_ui.py              # Graphical user interface
├── demo_video.mp4         # Project demonstration video
└── README.md
```

---

# 环境要求 | Requirements

Python 3.x

Main libraries:

```
torch
torchvision
opencv-python
numpy
matplotlib
```

Install:

```
pip install torch torchvision opencv-python numpy matplotlib
```

---

# 使用方法 | Usage

## 1. Train

```
python train.py
```

Train the VGG model on the MNIST dataset.

---

## 2. Test

```
python test.py
```

Evaluate the trained model.

---

## 3. Predict

```
python predict.py
```

Predict handwritten digits using the trained model.

Users can provide their own handwritten digit images for recognition.

---

# 图像数字识别 | Image-based Digit Recognition

The project supports handwritten digit recognition from uploaded images.

Processing pipeline:

1. Load input image
2. Grayscale conversion
3. Image preprocessing
4. Resize to MNIST format (28×28)
5. VGG model inference
6. Output prediction result

Users can upload custom handwritten digit images, and the system will automatically classify and recognize them.

---

# 数据集 | Dataset

The model is trained using the **MNIST handwritten digit dataset**, containing:

* 60,000 training images
* 10,000 testing images
* 10 digit classes (0–9)

---

# 实验结果 | Experimental Results

The VGG model achieves high recognition accuracy on the MNIST dataset and can successfully recognize handwritten digit images after OpenCV preprocessing.

```
Test Accuracy: 99.86%
```

---

# 毕业设计 | Graduation Project

This repository contains the implementation code corresponding to my undergraduate graduation project and thesis on handwritten digit recognition using deep learning.

---

# Future Work

* Support EMNIST dataset
* Support custom handwriting datasets
* Optimize inference speed
* Deploy with GUI interface
* Deploy on embedded devices

---

# License

This project is released under the MIT License.

Feel free to use it for learning and research purposes.
