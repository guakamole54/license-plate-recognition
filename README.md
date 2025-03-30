# 🔍 ANPR: Automatic Number Plate Recognition (Prototype)

This project is a **prototype ANPR (Automatic Number Plate Recognition)** system using Python, OpenCV, and OCR libraries to detect and read license plates from vehicle images.

---

## 🎯 Purpose

The goal is to build a functional license plate recognition pipeline using traditional computer vision techniques. It processes images step-by-step to locate plates, extract them, and recognize the characters — all using open-source tools.

---

## 🧰 Tech Stack

- **Python**
- **OpenCV** – Image preprocessing & contour detection
- **Tesseract OCR** – Fast character recognition
- **EasyOCR** – More accurate (but slower) OCR option
- **Matplotlib** – For visualization of results

---

## 🚀 Getting Started

1. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```
2. 🛠️ Install Tesseract OCR

Download and install Tesseract from:  
👉 https://github.com/tesseract-ocr/tesseract

Make sure it's added to your system **PATH** so it can be accessed by Python scripts.

---

3. ▶️ Run the Notebook

Open `anpr_notebook.ipynb` and run all cells. The pipeline will:

- 📷 Preprocess and analyze all images in the `img/` folder  
- 🔲 Detect license plates using contour-based detection  
- 🔡 Extract and recognize text using OCR (Tesseract or EasyOCR)  
- 🖼️ Annotate and display results with bounding boxes and recognized plate numbers

---

## ⚠️ Limitations

- 📷 **Highly sensitive to image quality** — Plates must be clear and ideal distance and angle 
- 🐢 **Slow OCR** — EasyOCR especially is too slow for real-time webcam use  
- ❌ **Fragile detection** — Struggles with blurry, angled, or low-light images  
- 🌍 **Limited format support** — Only validates plates from **CZ, SK, UA, and US** using regex





