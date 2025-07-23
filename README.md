
# 🫀 Detection of Cardiovascular Diseases from ECG Images

![ECG Banner](https://user-images.githubusercontent.com/placeholder/ecg-banner.png) <!-- Add your custom banner if available -->

## 🧠 Abstract

Electrocardiograms (ECGs) are critical diagnostic tools for detecting cardiovascular anomalies. Traditionally recorded on paper, manual analysis of ECGs is both time-consuming and prone to error. This project automates the diagnosis of cardiovascular diseases by digitizing ECG images and using machine learning to detect abnormalities. By extracting and analyzing key ECG waveform components (P, QRS, T waves), our system can effectively classify heart conditions.

## 📁 Dataset

We use the **ECG Image Signal Dataset** from [Mendeley Data](https://data.mendeley.com/datasets/gwbz3fsgp8/2), which includes ECG records from healthy individuals and those with cardiac issues.

➡️ **Additional Test Images:**  
To test the application manually, download ECG images from our GitHub repo:  
📂 [`ECG_IMAGES_DATASET`](https://github.com/rameshavinash94/Cardiovascular-Detection-using-ECG-images/tree/main/ECG_IMAGES_DATASET)

---

## 🚀 Deployment

The project is deployed using **Google Cloud Platform (GCP)** and can be accessed at:  
🔗 [Live Application](https://cmpe255-project-q4uake3apq-uc.a.run.app)

Simply upload an ECG image to get real-time diagnostic insights.

---

## 🎯 Project Workflow

1. **Upload** ECG image to web application.
2. **Preprocessing**:
   - Convert RGB to Grayscale
   - Apply Gaussian Blur
   - Resize and Threshold to remove gridlines
3. **Signal Extraction**:
   - Use image contours to isolate ECG waveform
   - Convert waveform into a 1D signal
   - Normalize signal
4. **Feature Extraction**:
   - Extract P, QRS, and T waves
5. **Classification** using a pre-trained ML model:
   - Normal
   - Myocardial Infarction
   - Abnormal Heartbeat
   - History of Myocardial Infarction
6. **Result Display**: Visual feedback and prediction rendered on UI

---

## 🧪 Tech Stack

- **Frontend:** HTML, JavaScript, CSS
- **Backend:** Python (Flask)
- **Machine Learning:** Scikit-learn, NumPy, OpenCV
- **Deployment:** Google Cloud Platform (Cloud Run)

---

## 📌 Key Highlights

- Real-time ECG diagnostics through image-based signal analysis
- 1D waveform signal conversion from raw ECG images
- Extraction of P-QRS-T features improves diagnostic accuracy
- Intuitive UI with step-by-step visualization
- Deployed and tested on real-world ECG data

---

## 🏁 How to Run Locally

```bash
git clone https://github.com/rameshavinash94/Cardiovascular-Detection-using-ECG-images.git
cd Cardiovascular-Detection-using-ECG-images
pip install -r requirements.txt
python app.py
```

Then open `http://127.0.0.1:5000` in your browser.

---

---

## 💡 Future Enhancements

- Extend model to detect additional heart conditions
- Support ECG video signals
- Improve grid removal for cleaner waveform extraction
- Model optimization for edge deployment

---
