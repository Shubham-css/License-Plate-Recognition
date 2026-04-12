# 🚗 License Plate Recognition using OpenCV & Tesseract OCR

An end-to-end Automatic License Plate Recognition (ALPR) system that detects vehicle license plates from images and extracts the registration number using computer vision and Optical Character Recognition (OCR).

---

## 📌 Overview

This project implements a computer vision pipeline to:

* Detect license plate regions in an image
* Extract the detected region
* Apply image preprocessing techniques
* Recognize text using Tesseract OCR

The system can be used in applications such as traffic monitoring, parking management, toll systems, and law enforcement.

---

## 🎯 Objectives

* Automate the process of vehicle number plate detection
* Extract readable text from license plates
* Reduce manual effort in vehicle identification systems
* Demonstrate integration of OpenCV with OCR technologies

---

## 🧠 Methodology

The project follows a step-by-step pipeline:

1. **Image Acquisition**

   * Input image containing a vehicle

2. **Preprocessing**

   * Convert image to grayscale
   * Apply noise reduction (e.g., bilateral filtering)

3. **Edge Detection**

   * Use Canny Edge Detection to identify edges

4. **Contour Detection**

   * Identify contours and filter based on shape/size
   * Locate rectangular regions likely to be license plates

5. **Region Extraction**

   * Crop the detected license plate area

6. **OCR Processing**

   * Use Tesseract OCR to extract text from the cropped image

---

## 🛠️ Technologies Used

* **Python**
* **OpenCV** – Image processing and computer vision
* **Tesseract OCR** – Text recognition
* **NumPy** – Numerical operations
* **Matplotlib** – Visualization (optional)

---

## 📂 Project Structure

```
License-Plate-Recognition/
│
├── License_Plate_Recognition_with_OpenCV_and_Tesseract_OCR.ipynb
├── README.md
├── requirements.txt
└── sample_images/   (optional)
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Shubham-css/License-Plate-Recognition.git
cd License-Plate-Recognition
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

OR manually:

```bash
pip install opencv-python pytesseract numpy matplotlib
```

---

### 3️⃣ Install Tesseract OCR

👉 Download from: https://github.com/tesseract-ocr/tesseract

After installation, configure path (Windows):

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

---

## ▶️ Usage

1. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Run:

   ```
   License_Plate_Recognition_with_OpenCV_and_Tesseract_OCR.ipynb
   ```

3. Provide an input image and execute all cells

---

## 📊 Results

* Successfully detects license plate regions
* Extracts alphanumeric text using OCR
* Works well on clear images with visible plates

---

## ⚠️ Limitations

* Performance depends on image quality
* Struggles with:

  * Blurry images
  * Low lighting
  * Skewed or angled plates
* OCR accuracy may vary

---

## 🚀 Future Improvements

* Use Deep Learning (YOLO, CNN) for better detection
* Improve OCR accuracy with preprocessing
* Support real-time video processing

---

## 📸 Sample Output (Optional)

![Detected Image Demo](image.png)

---

## 🤝 Contribution

Contributions are welcome! Feel free to fork this repository and submit pull requests.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

**Shubham**
GitHub: https://github.com/Shubham-css

---

## ⭐ Acknowledgements

* OpenCV Documentation
* Tesseract OCR

---
