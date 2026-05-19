<p align="center">
  <img src="assets/icon_256.png" alt="Logo PDF Comparator" width="150">
</p>
  
# **PDF Comparator | Computer Vision & Deep Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Tesseract OCR](https://img.shields.io/badge/Tesseract_OCR-43B02A?style=for-the-badge&logo=tesseract&logoColor=white)
![HTML5/JS](https://img.shields.io/badge/HTML5_&_JS-E34F26?style=for-the-badge&logo=html5&logoColor=white)

> **Business Impact:** Engineered a Computer Vision solution that reduced engineering blueprint analysis time by **99%** (from 48 hours to 5 minutes) while eliminating human error in visual inspections.

## Project Overview
**PDF Comparator** is an automated visual inspection tool built to detect structural and textual discrepancies between complex engineering drawings. 

Initiated and developed independently to solve a critical operational bottleneck, the software processes large batches of high-resolution PDFs, compares them pixel-by-pixel, and generates interactive HTML/JS reports for the engineering team to review.

*Note: This repository serves as a portfolio showcase. The source code and executable are proprietary and not publicly available to ensure corporate data compliance.*

## Key Features

* **High-Performance Batch Processing:** Utilizes Python's `ThreadPoolExecutor` for multithreaded analysis, allowing the system to process entire directories of blueprints concurrently.
* **Intelligent Noise Filtering:** Integrates **Tesseract OCR** to filter out false positives caused by text displacement, focusing only on genuine structural alterations.
* **Interactive HTML Dashboard:** The pipeline ends with a dynamically generated frontend report containing a custom **Sync Scroll** engine, allowing technicians to pan and zoom both blueprints simultaneously in a side-by-side view.
* **Adjustable Sensitivity Profiles:** Built-in thresholding profiles (Conservative to Extreme) and custom parameters (Min Area, Padding Margin) to adapt the Computer Vision engine to different types of engineering plants.
* **Modern UI:** Built with `CustomTkinter`, providing a dark-mode, user-friendly interface for non-technical users to configure parameters and monitor execution.

## Architecture & Tech Stack

1. **Image Processing Engine:** `pdf2image` & `poppler` for high-fidelity vector-to-raster conversion.
   * `OpenCV` (cv2) for grayscale conversion, absolute differencing, binary thresholding, and contour detection.
2. **Text Analysis (OCR):**  `pytesseract` to extract and compare text blobs, ignoring elements that simply moved coordinates without changing content.
3. **Frontend / UX:**  `CustomTkinter` for the desktop application.
   * Native `HTML/CSS/JavaScript` injected programmatically via Python to create the offline, interactive evidence reports.

## Visual Showcase

### 1. Desktop Application Interface
![App UI](assets/menu_UI.gif)  
![App UI](assets/menu_UI2.gif)

### 2. Interactive Side-by-Side Report (Sync Scroll)
![Sync Scroll Demo](assets/sync_scroll.gif)

### 3. Visual Evidence Detection
![Difference Detection](assets/detection_example.png)

---
**Created by Anderson Siqueira Souto / www.linkedin.com/in/anderson-siqueira-souto** | **Role: Apprentice Developer**
