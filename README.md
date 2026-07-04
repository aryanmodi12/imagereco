<div align="center">

# 🔍 VisionIQ — AI Image Recognition System

**A production-grade deep learning web application for real-time image classification using pretrained CNN models**

![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.19-FF6F00?style=for-the-badge\&logo=tensorflow\&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.1-000000?style=for-the-badge\&logo=flask\&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.11-5C3EE8?style=for-the-badge\&logo=opencv\&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)

<br/>

**3 CNN Models · 1000 ImageNet Classes · Real-Time Inference · REST API · Modern UI**

<br/>

</div>

---

## 🚀 Overview

**VisionIQ** is a fully functional AI-powered image recognition system that enables users to classify images instantly using state-of-the-art pretrained convolutional neural networks.

Instead of building complex pipelines from scratch, VisionIQ provides a **plug-and-play solution** combining deep learning, computer vision, and a modern web interface — all running locally without external APIs or keys.

---

## 🎯 Key Features

### 🧠 Multiple Deep Learning Models

* **MobileNetV2** — fast and lightweight
* **ResNet-50** — balanced performance
* **EfficientNet-B0** — optimized accuracy

✔ Models can be switched dynamically without restarting the server

---

### 📤 Flexible Input Options

* Drag & drop image upload
* File selection from device
* Direct image URL prediction

---

### 📊 Intelligent Output

* Top-5 predictions with confidence scores
* Real-time inference timing
* Clean visualization with progress indicators

---

### 🔬 Image Analysis (OpenCV)

Each image is automatically analyzed for:

* Brightness
* Contrast
* Edge density
* Dominant color

---

### 🌐 REST API Support

* `/predict` → upload image
* `/predict/url` → classify via URL
* `/api/models` → list available models
* `/api/switch-model` → change model dynamically
* `/api/health` → system diagnostics

---

## 🛠 Tech Stack

| Layer               | Technology         |
| ------------------- | ------------------ |
| Backend             | Flask              |
| Deep Learning       | TensorFlow / Keras |
| Image Processing    | Pillow             |
| Computer Vision     | OpenCV             |
| Numerical Computing | NumPy              |
| HTTP Requests       | Requests           |
| Testing             | Pytest             |
| CI/CD               | GitHub Actions     |

---

## ⚡ Quick Start

### 1. Clone Repository

```bash
git clone https://github.com/Bansaripatel02/VisionIQ-Image-Recognition.git
cd VisionIQ-Image-Recognition
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Environment

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run Application

```bash
python app.py
```

Open: **http://localhost:5000**

---

## 📁 Project Structure

```
VisionIQ-Image-Recognition/
│
├── app.py
├── src/
│   ├── config.py
│   ├── model_manager.py
│   └── preprocessor.py
│
├── templates/
├── static/
├── tests/
├── uploads/
└── README.md
```

---

## 🏗 Architecture

```
User Interface (Browser)
        │
        ▼
Flask Backend (API Routes)
        │
 ┌───────────────┬───────────────┐
 ▼               ▼               ▼
Preprocessing   Model Manager   OpenCV Analysis
        │
        ▼
TensorFlow Models (ImageNet)
```

---

## 🧪 Testing

Run test suite:

```bash
pytest tests/ -v
```

✔ Ensures reliability across:

* Configuration
* Image preprocessing
* API endpoints

---

## 🌐 Deployment

### Production (Gunicorn)

```bash
pip install gunicorn
gunicorn -w 2 -b 0.0.0.0:5000 app:app
```

---

### Docker (Optional)

```dockerfile
FROM python:3.12-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5000
CMD ["gunicorn", "-w", "2", "-b", "0.0.0.0:5000", "app:app"]
```

---

## 🗺 Roadmap

* Grad-CAM visualization
* Batch image prediction
* Custom model upload
* YOLO object detection
* Prediction history dashboard

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Submit a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Aryan Modi**

---

<div align="center">

⭐ *If you found this project useful, consider starring the repository*

</div>
