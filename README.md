# 🎭 Multimodal Deepfake Video Detection

A deep learning-based system for detecting **deepfake videos** using a **multimodal approach**. Combines **frame-based analysis** (ResNet50), **temporal dynamics** (optical flow + 3D-CNN), and **late fusion** to enhance detection accuracy and robustness.

---
Selecting best 50 real and 50 fake videos on 2-3 parameters due to limited compuation resources.

## 🌟 Features

- 🖼️ **Frame-based classification** using pretrained **ResNet50**  
- 🎥 **Temporal consistency analysis** using **3D-CNN on optical flow**  
- 🧠 **Late fusion** of visual and temporal features for final prediction  
- 📈 Achieved **94.1% accuracy** and **F1-score of 0.91** on FaceForensics++  
- 📁 Modular pipeline for frame extraction, flow computation, training, and evaluation

---

## 🧠 Model Overview

| Component       | Architecture    | Accuracy / Metric |
|----------------|------------------|-------------------|
| Frame Analysis | ResNet50         | 85%               |
| Optical Flow   | 3D-CNN           | 94%               |
| Final Model    | Late Fusion      | 94.1% (F1: 0.91)  |

---

## ⚙️ Getting Started

### 🔧 To Run Locally:

1. Clone the repository:
git clone https://github.com/Vikas717-creator/multimodal-deepfake-detection.git cd multimodal-deepfake-detection

markdown
Copy
Edit

2. Install dependencies:
pip install -r requirements.txt

csharp
Copy
Edit

3. Extract frames from videos:
python utils/extract_frames.py

css
Copy
Edit

4. Compute optical flow:
python utils/compute_optical_flow.py

markdown
Copy
Edit

5. Train individual models:
python resnet50_frame_model.py python optical_flow_model.py

sql
Copy
Edit

6. Apply late fusion for final classification:
python late_fusion.py

yaml
Copy
Edit

---

## 📊 Evaluation

- Dataset: FaceForensics++ (subset of 50 real + 50 fake videos)  
- Accuracy: **94.1%**  
- F1-Score: **0.91**  
- Frame model accuracy: 85%  
- Optical flow model accuracy: 94%

---

## 📊 Technologies Used

- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy / Pandas  
- Matplotlib
- Seaborn
- Scikit-Learn
- FaceForensics++ dataset
- Google Colab

---
## Screenshots


## 🔮 Future Enhancements

- 🧠 Add audio stream analysis for full multimodal detection  
- 📥 Automate video preprocessing and fusion  
- 🌐 Build Streamlit demo to upload and test deepfakes  
- 📊 Visual dashboard for prediction confidence and heatmaps

---

## 🤝 Contributing

Contributions and ideas are welcome! Fork the repo and submit a pull request.


## 🔗 Connect with Me

- GitHub: [@Vikas717-creator](https://github.com/Vikas717-creator)  
- LinkedIn: [Vikas Thakur](https://www.linkedin.com/in/vikas-thakur-2304a6261/)
