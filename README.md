# 🧠 VisionX

### Cross-Generator Deepfake Detection with CUDA Acceleration

<p align="center">
  <img src="Banner1.gif" width="400" height="300" alt="VisionX Banner"/>
</p>

<p align="center">
  <img src="https://svg-banners.vercel.app/api?type=glitch&text1=VISIONX&text2=Deepfake%20Detection&width=900&height=200&color=%231EB5FF&bgColor=%230B0F19" alt="VisionX Banner"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=1EB5FF&center=true&vCenter=true&width=750&lines=AI-Powered+Deepfake+Detection;Cross-Generator+Detection;CUDA+Accelerated+Inference;Video+%26+Face+Analysis" alt="Typing SVG"/>
</p>

---

## 🔍 About VisionX

**VisionX** is an AI-powered deepfake detection system designed to identify manipulated facial content in images and videos.

The project combines **deep learning, computer vision, GPU acceleration, and a deployable inference pipeline** to analyze visual content and determine whether it is **Real** or **Fake**.

Unlike a simple image-classification project, VisionX focuses on building an end-to-end detection pipeline:

```text
Video / Image
      │
      ▼
Frame Extraction
      │
      ▼
Face Detection
      │
      ▼
Face Preprocessing
      │
      ▼
Deepfake Detection Model
      │
      ▼
CUDA Accelerated Inference
      │
      ▼
Prediction + Confidence
      │
      ▼
Real / Fake
```

---

## 🚀 Key Features

* 🎭 **Deepfake Detection**
* 🎥 **Video-based analysis**
* 🖼️ **Image-based face analysis**
* 👤 **Automatic face extraction**
* 🧠 **PyTorch-based deep learning model**
* ⚡ **CUDA/GPU acceleration**
* 🔄 **Cross-generator detection**
* 📊 **Confidence-based predictions**
* 🌐 **API-based inference**
* 🖥️ **Interactive detection interface**
* 🔒 **Privacy-focused local processing**
* 📦 Modular and extensible architecture

---

## 🧠 What Problem Does VisionX Solve?

Modern generative AI systems can create highly realistic manipulated videos and images.

Traditional detection systems often struggle when they encounter **deepfakes generated using techniques or generators that were not present in their training data**.

VisionX aims to address this through:

### Cross-Generator Detection

Instead of focusing only on detecting a particular deepfake generation technique, VisionX is designed around the broader problem of detecting manipulation across different generators and manipulation methods.

### GPU-Accelerated Processing

Deepfake detection involves computationally expensive operations such as:

* Video frame processing
* Face detection
* Image preprocessing
* Neural network inference

VisionX uses **CUDA acceleration** to utilize NVIDIA GPUs and reduce inference time.

---

## 🏗️ System Architecture

```text
                    ┌──────────────────┐
                    │   User Input     │
                    │ Image / Video    │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │ Input Validation │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │ Frame Extraction │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │  Face Detection  │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │ Preprocessing    │
                    │ Resize / Normalize│
                    └────────┬─────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │ Deepfake Detector    │
                  │      PyTorch         │
                  └──────────┬───────────┘
                             │
                      CUDA / GPU
                             │
                             ▼
                    ┌──────────────────┐
                    │ Prediction Layer │
                    └────────┬─────────┘
                             │
                    ┌────────┴────────┐
                    ▼                 ▼
                 REAL              FAKE
```

---

## 🛠️ Tech Stack

### Programming Languages

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
</p>

### AI / Machine Learning

<p>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
</p>

### Computer Vision

<p>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
</p>

### GPU Computing

<p>
<img src="https://img.shields.io/badge/NVIDIA%20CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white"/>
</p>

### Backend / Deployment

<p>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
</p>

### Data / Infrastructure

<p>
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DD0031?style=for-the-badge&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
</p>

### Development

<p>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white"/>
</p>

---

## 📂 Project Structure

```text
VisionX/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── test_output/
│
├── src/
│   ├── models/
│   │   └── detector.py
│   │
│   ├── pipeline/
│   │   ├── dataset.py
│   │   ├── extract_faces.py
│   │   └── ...
│   │
│   └── ...
│
├── tests/
│
├── notebooks/
│
├── scripts/
│
├── requirements.txt
├── README.md
└── ...
```

---

## ⚡ CUDA Acceleration

VisionX is designed to take advantage of NVIDIA GPUs through CUDA-enabled PyTorch.

The model automatically uses the available computation device:

```python
device = torch.device(
    "cuda" if torch.cuda.is_available() else "cpu"
)

model = model.to(device)
```

You can verify CUDA availability using:

```bash
python3 -c "import torch; print(torch.cuda.is_available())"
```

To check the detected GPU:

```bash
python3 -c "import torch; print(torch.cuda.get_device_name(0))"
```

---

## 🧪 Model Pipeline

The detection pipeline consists of several stages.

### 1. Input

VisionX accepts visual content such as:

```text
Image
Video
```

### 2. Frame Extraction

For video input, frames are sampled from the video for analysis.

### 3. Face Detection

Faces are extracted from the frames so that the model focuses on the facial region where manipulation artifacts are most relevant.

### 4. Preprocessing

Detected faces are:

* Resized
* Normalized
* Converted into tensors
* Prepared for model inference

### 5. Deepfake Classification

The processed face is passed through the VisionX detection model.

The model produces a prediction representing:

```text
REAL
   or
FAKE
```

along with a confidence score.

---

## 📊 Evaluation

VisionX can be evaluated using standard classification metrics:

| Metric         | Purpose                               |
| -------------- | ------------------------------------- |
| Accuracy       | Overall classification correctness    |
| Precision      | Reliability of fake predictions       |
| Recall         | Ability to detect manipulated samples |
| F1 Score       | Balance between precision and recall  |
| ROC-AUC        | Overall classification performance    |
| Inference Time | Detection speed                       |
| FPS            | Video processing performance          |

---

## 🔬 Cross-Generator Evaluation

A major goal of VisionX is evaluating how well the detector performs when the **generation technique differs between training and testing data**.

```text
Training Generator
        │
        ▼
   VisionX Model
        │
        ▼
Different Generator
        │
        ▼
Generalization Test
```

This helps measure whether the model is learning meaningful manipulation artifacts rather than simply memorizing characteristics of a particular dataset or generator.

---

## 🖥️ Demo

### Detection Interface

<p align="center">
  <img src="assets/demo.png" width="850" alt="VisionX Demo"/>
</p>

### Example Output

```text
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
        VISIONX RESULT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Prediction : FAKE
Confidence : 94.72%

Frames Analyzed : 32
Faces Detected  : 29

Device : NVIDIA CUDA GPU

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

> Replace `assets/demo.png` with an actual screenshot from your VisionX application.

---

## 🔐 Privacy

VisionX is designed with privacy in mind.

Where supported by the deployment configuration, media can be processed locally without requiring the user's original image or video to be uploaded to an external third-party AI service.

---

## 📈 Future Improvements

* [ ] Temporal video analysis
* [ ] Transformer-based detection
* [ ] Multi-face tracking
* [ ] Better cross-dataset generalization
* [ ] Explainable AI / manipulation heatmaps
* [ ] Real-time webcam detection
* [ ] Distributed GPU inference
* [ ] Model quantization
* [ ] ONNX/TensorRT inference
* [ ] Large-scale benchmark evaluation
* [ ] Production monitoring

---

## 🎯 Project Goals

VisionX is being developed with four main goals:

**1. Accuracy**
Detect manipulated facial content reliably.

**2. Generalization**
Perform well against previously unseen manipulation techniques.

**3. Performance**
Use GPU acceleration to make inference practical for video workloads.

**4. Deployability**
Move beyond a research notebook into a complete, usable detection system.

---

## 👨‍💻 Developer

<p align="center">

<b>Siddharth</b>

<br>

AI/ML • Computer Vision • CUDA • Backend Development

</p>

---

## ⭐ Project Status

```text
VisionX
│
├── Dataset Pipeline       ██████████░░  In Progress
├── Face Extraction        ██████████░░  In Progress
├── Detection Model        █████████░░░  In Progress
├── CUDA Acceleration      ████████░░░░  In Progress
├── Evaluation             ██████░░░░░░  In Progress
└── Deployment              ████░░░░░░░░  Planned
```

> VisionX is an actively developed project. Results and architecture may change as the model and evaluation pipeline improve.

---

<p align="center">
  <b>VisionX • Detecting What Isn't Real</b>
</p>
