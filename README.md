# Real-Time Object Detection API using TensorFlow

A **Transfer Learning-based Object Detection system** that detects multiple objects from **images, video files, and real-time webcam streams** using pretrained **SSD** and **Faster R-CNN** models with **TensorFlow** and **OpenCV**.

## 🚀 Features

* 🖼️ Object detection from images
* 🎥 Object detection from video files
* 📷 Real-time webcam object detection
* 🧠 SSD-based object detection
* 🔍 Faster R-CNN-based object detection
* 🔄 Transfer learning using pretrained models
* 🏷️ COCO dataset label mapping
* ⚡ Real-time video processing with OpenCV

## 🧠 Models Used

### SSD — Single Shot Detector

SSD performs object detection in a single forward pass, making it suitable for applications where detection speed is important.

### Faster R-CNN

Faster R-CNN uses a Region Proposal Network to identify potential object regions before performing classification and bounding-box regression. It generally provides strong detection accuracy while requiring more computation than SSD.

### MobileNet

MobileNet is used as a lightweight feature-extraction backbone, making the detection pipeline suitable for real-time applications.

## 🛠️ Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **OpenCV**
* **Jupyter Notebook**
* **COCO Dataset**
* **TensorFlow Object Detection API**

## 📂 Detection Sources

| Input  | SSD | Faster R-CNN |
| ------ | :-: | :----------: |
| Image  |  ✅  |       ✅      |
| Video  |  ✅  |       ✅      |
| Webcam |  ✅  |       ✅      |

## 📸 Results

### SSD — Image Detection

Add your SSD image detection screenshot here.

### SSD — Video Detection

Add your SSD video detection screenshots here.

### SSD — Webcam Detection

Add your SSD webcam detection screenshot here.

### Faster R-CNN — Image Detection

Add your Faster R-CNN image detection screenshot here.

### Faster R-CNN — Video Detection

Add your Faster R-CNN video detection screenshots here.

### Faster R-CNN — Webcam Detection

Add your Faster R-CNN webcam detection screenshot here.

## 🔬 Technical Concepts

### Transfer Learning

The project uses pretrained object detection models rather than training an object detector completely from scratch. This allows the system to leverage features learned from large-scale datasets.

### Label Map

A TensorFlow label map associates object classes with numerical IDs. These IDs are used during inference to convert model predictions into recognizable object labels.

### Inference Graph

The inference graph represents the trained detection model used during prediction. It contains the operations required to process an input and produce object classes, confidence scores, and bounding boxes.

### Protocol Buffers

TensorFlow Object Detection models use serialized configuration and model information that can be represented using Protocol Buffers (`.proto` / `.pb`).

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Real-Time-Object-Detection-API-using-TensorFlow.git
cd Real-Time-Object-Detection-API-using-TensorFlow
```

### 2. Install dependencies

```bash
pip install tensorflow opencv-python keras jupyter
```

### 3. TensorFlow Object Detection API

Install and configure the TensorFlow Object Detection API according to the TensorFlow Models documentation.

### 4. Run the notebooks

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run the appropriate notebook for:

* Image detection
* Video detection
* Webcam detection
* SSD inference
* Faster R-CNN inference

## 📱 Smartphone Camera

A smartphone camera can also be used as a video source with a compatible IP-camera application.

Start the camera server on the smartphone, obtain its local IP address, and configure the corresponding notebook to use that stream as the input source.

## 📊 Detection Pipeline

```text
Image / Video / Webcam
          ↓
       OpenCV
          ↓
   Preprocessing
          ↓
 ┌─────────────────┐
 │ SSD / Faster    │
 │     R-CNN       │
 └─────────────────┘
          ↓
 Object Predictions
          ↓
Bounding Boxes + Labels
          ↓
     Visualization
```

## 🎯 Project Objective

The objective of this project is to demonstrate how **pretrained deep learning models and transfer learning** can be applied to build an object detection system capable of processing different visual input sources in real time.

## 📌 Future Improvements

* Add a REST API using **FastAPI**
* Add a web-based detection interface
* Support additional detection models such as YOLO
* Add configurable confidence thresholds
* Add object tracking
* Add FPS and inference-time monitoring
* Containerize the application using Docker

## ⭐ Support

If you find this project useful, consider giving the repository a **⭐ Star** and sharing your feedback.

## 📄 License

Add the appropriate license for your implementation and verify the license of any pretrained models, datasets, or source code used in this project.
