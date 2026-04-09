# 🚀 Lafz-Aashna — Urdu OCR & Evaluation System

A full-stack OCR system designed to extract, evaluate, and interact with **Urdu text** from PDFs and images — built with a focus on **accuracy, usability, and real-world application**.

---

## 💡 Overview

**Lafz-Aashna** goes beyond traditional OCR.

It not only extracts Urdu text but also:
- 📊 Measures extraction quality (WER & CER)
- ⚡ Provides real-time feedback with confidence scores
- 🎯 Delivers an interactive, user-friendly web interface

---

## 🎯 Key Features

- 📂 **Upload Support**
  - Drag & drop PDFs or images
  - Supports multi-page documents

- 🧠 **Urdu OCR Processing**
  - Tesseract with Urdu language model
  - Optimized preprocessing pipeline

- 📊 **Evaluation Metrics**
  - Word Error Rate (WER)
  - Character Error Rate (CER)
  - Accepts **any named `.txt` file** as ground truth

- 📈 **Confidence Scoring**
  - Page-wise OCR confidence percentages

- 🎨 **Modern UI/UX**
  - Animated results rendering
  - Copy-to-clipboard with smart pop-ups
  - Scroll guidance with visual cues
  - Real-time feedback (no page reloads)

---

## 🏗️ System Architecture

- Frontend (HTML/CSS/JS)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓
- Flask Backend (API)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓
- Preprocessing (OpenCV + PIL)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓
- OCR Engine (Tesseract - Urdu)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓
- Evaluation (JiWER)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓
- JSON Response → UI Rendering

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|------|
| **Backend** | Flask (Python) |
| **OCR Engine** | Tesseract OCR (Urdu) |
| **Image Processing** | OpenCV, Pillow |
| **PDF Handling** | pdf2image |
| **Evaluation** | JiWER |
| **Frontend** | HTML, CSS, JavaScript |
| **Deployment** | Google Colab + Ngrok |

---

## ⚙️ Preprocessing Pipeline

To improve OCR accuracy, the following steps are applied:

1. **Resizing (if needed)** – Enhances low-resolution inputs  
2. **Grayscale Conversion** – Simplifies image structure  
3. **Gaussian Blur** – Reduces noise  
4. **Adaptive Thresholding** – Improves Urdu text clarity  

---

## 📊 Evaluation Metrics

- **WER (Word Error Rate)** → Measures word-level accuracy  
- **CER (Character Error Rate)** → Measures character-level precision  

📌 Supports both manual text input and uploaded `.txt` files for evaluation.

---

## 📸 Sample Output

- Page-wise extracted Urdu text  
- Confidence percentage bars  
- Evaluation metrics (WER & CER)  
- Interactive UI with copy functionality  

---

## ⚠️ Challenges Faced

- Handling **Urdu script complexity** (ligatures, spacing)
- Managing **OCR inconsistencies across fonts**
- Debugging **Flask + Ngrok issues in Colab**
- Ensuring smooth **frontend-backend communication**
- Avoiding crashes while processing large PDFs
  
---

## 🔮 Future Improvements

- 🧠 Fine-tune Tesseract with **Urdu-specific datasets**
- 📚 Support multiple Urdu fonts (**Naskh, Nastaliq**)
- ⚡ Optimize for large-scale document processing
- ☁️ Deploy on cloud infrastructure (AWS/GCP)
- 🤖 Integrate AI-based post-processing for correction

---

## 🎯 Use Cases

- 📄 Digitizing Urdu documents  
- 🏛️ Archival & historical text processing  
- 🏥 Form/document automation in local languages  
- 📚 Educational tools for Urdu text analysis  

---

## 🤝 Contributing

Feel free to fork, improve, or suggest enhancements!

---

## 💻 How to Run 

Use the following link on Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1slUybkoiHpwnu62chVXzPX7ybCX4rLcC#scrollTo=z4vTnZpMZ3VL)
