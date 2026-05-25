<p align="center">
  <img src="assets/icon_256.png" alt="PDF Comparator Logo" width="120">
</p>

<h1 align="center">PDF Comparator</h1>

<p align="center">
  <em>Computer Vision & Deep Learning for Engineering Blueprint Analysis</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python">
  <img src="https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white" alt="OpenCV">
  <img src="https://img.shields.io/badge/Tesseract_OCR-43B02A?style=for-the-badge&logo=tesseract&logoColor=white" alt="Tesseract OCR">
  <img src="https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Production-brightgreen?style=flat-square" alt="Status">
  <img src="https://img.shields.io/badge/Type-Proprietary-red?style=flat-square" alt="Type">
  <img src="https://img.shields.io/badge/Role-Apprentice_Developer-blue?style=flat-square" alt="Role">
  <img src="https://img.shields.io/badge/Since-September%202025-orange?style=flat-square" alt="Since">
</p>

---

## 🚀 Business Impact

> Engineered a Computer Vision solution that reduced engineering blueprint analysis time by **99%** — from **12 hours** to **5 minutes** — while completely eliminating human error in visual inspections.

---

## 📌 Overview

**PDF Comparator** is an automated visual inspection tool built to detect structural and textual discrepancies between complex engineering drawings.

Initiated and independently developed since **September 2025** to solve a critical operational bottleneck, the software processes large batches of high-resolution PDFs, compares them pixel-by-pixel, and generates interactive HTML/JS reports for the engineering team to review.

> ⚠️ **Note:** This repository is a portfolio showcase. Source code and executables are proprietary and not publicly available to ensure corporate data compliance.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| ⚡ **Batch Processing** | Multithreaded via `ThreadPoolExecutor` — processes entire directories concurrently |
| 🧠 **Noise Filtering** | Tesseract OCR filters false positives from text displacement, focusing on structural changes |
| 📊 **Interactive Reports** | Dynamically generated HTML dashboards with custom **Sync Scroll** engine |
| 🎛️ **Sensitivity Profiles** | Built-in presets (Conservative → Extreme) plus custom Min Area and Padding Margin parameters |
| 🖥️ **Modern UI** | Dark-mode desktop app built with `CustomTkinter`, designed for non-technical users |

---

## 🏗️ Architecture & Tech Stack

```text
PDF Input
   │
   ▼
┌─────────────────────────────┐
│   Image Processing Engine   │  pdf2image + poppler (vector → raster)
│   OpenCV Pipeline           │  grayscale → diff → threshold → contours
└─────────────┬───────────────┘
              │
              ▼
┌─────────────────────────────┐
│   Text Analysis (OCR)       │  pytesseract — filters moved-but-unchanged text
└─────────────┬───────────────┘
              │
              ▼
┌─────────────────────────────┐
│   Report Generation         │  HTML/CSS/JS injected via Python
│   Desktop Interface         │  CustomTkinter dark-mode GUI
└─────────────────────────────┘
```

### Libraries & Tools

- **`pdf2image`** + **`poppler`** — High-fidelity vector-to-raster PDF conversion
- **`OpenCV (cv2)`** — Grayscale conversion, absolute differencing, binary thresholding, contour detection
- **`pytesseract`** — OCR text extraction to filter non-structural differences
- **`CustomTkinter`** — Modern dark-mode desktop interface
- **Native HTML/CSS/JavaScript`** — Programmatically generated offline inspection reports

---

## 🎬 Visual Showcase

### Desktop Application Interface

![App UI](assets/menu_UI.gif)  

---

![App UI](assets/menu_UI2.gif)  

---  

![App UI](assets/menu_UI3.gif)

---

### Interactive Side-by-Side Report (Sync Scroll)

![Sync Scroll Demo](assets/sync_scroll.mp4)

---

### Visual Evidence Detection

![Difference Detection](assets/detection_example.png)

---

## 👤 Author

**Anderson Siqueira Souto** — Apprentice Developer  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230A66C2.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anderson-siqueira-souto)
