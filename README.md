# IndicPhotoOCR Dataset & Evaluation Contribution

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

This repository contains a benchmark dataset of 71 natural scene images with text in various Indic scripts (e.g., shop signs, banners, street boards) annotated with polygons and transcriptions. It is intended to test and evaluate the [IndicPhotoOCR](https://github.com/Bhashini-IITJ/IndicPhotoOCR) system. This repo also includes scripts and output results.

---

## 📁 Project Structure
```
IndicPhotoOCR/
├── Dataset/
│ ├── Annotated_Dataset/ # Polygon annotations with transcription + script
│ └── Raw_Images/ # 50 real-world images with Indic text
│
├── Outputs/
│ ├── Batch_OCR_outputs/ # OCR results for all images (batch mode)
│ ├── Detection_outputs/ # Text detection bounding boxes
│ └── Single_OCR_outputs/ # OCR output from single image testing
│
├── Scripts/
│ ├── Single_ImageOCR.py # Run OCR on one image
│ ├── Multiple_ImageOCR.py # Run OCR on multiple images
│ └── Detection.py # Run only detection module
│
├── requirements.txt # Python dependencies
└── README.md # You are here!
```
## 🚀 Features

- ✅ Contains 71 scene-text images from diverse Indian locations
- ✍️ Polygon annotations with transcriptions and script info
- 🧪 Easily testable using IndicPhotoOCR pipeline
- 📁 Organized output folders (batch and single mode)
- 🐍 Python scripts for running full OCR and detection

---

## 🔧 Installation

To run the scripts and evaluate on your machine:


## Clone the repository
```bash
git clone https://github.com/DeepjyotiRoy01/IndicPhotoOCR.git
cd IndicPhotoOCR
```
## Create and activate a virtual environment
```bash
conda create -n indicphotoocr python=3.10 -y
conda activate indicphotoocr
```
## Install dependencies
```bash
pip install -r requirements.txt
```
## 🖼️ Usage
➤ Run OCR on a single image
```bash
python Scripts/Single_ImageOCR.py
```
➤ Run OCR on a folder of images
```bash
python Scripts/Multiple_ImageOCR.py
```
➤ Run detection only (without recognition)
```bash
python Scripts/Detection.py
```
Make sure to update image paths or folder paths inside the scripts as needed.

📦 Output Format
```json
JSON (example):
{
  "image": "IMG_41.jpg",
  "text": "ইলেকট্রিক",
  "bbox": [[1044, 609],
          [1557, 609],
          [1557, 903],
          [1044, 903]],
  "script": "Bengali"
}
```
## CSV (example):
| image       | text     | bbox                         | language  |
|-------------|----------|------------------------------|-----------|
|IMG_41.jpg   |	ইলেকট্রিক |	[[1044, 609],,,[1044, 903]]	| Bengali   |

### 📜 License
This project is licensed under the MIT License.
You may use, modify, or distribute this dataset and code for research, benchmarking, and educational purposes.

## 🙌 Contribution to Main IndicPhotoOCR
This dataset and evaluation result set was created to enhance the IndicPhotoOCR benchmark.

To contribute:

Fork the original repository

Commit your changes to your fork

Open a Pull Request (PR) describing your additions (dataset, annotations, outputs, scripts)

Can access the main project from the following link : 
```
https://github.com/Bhashini-IITJ/IndicPhotoOCR
```
## Credits 
For the successful completion of my project, I would like to thank 

Prof. Anand Mishra Sir

Professor CSE Dept.

Indian Institute of Technology, Jodhpur.

Anek De Sir

Indian Institute of Technology, Jodhpur.

### 📩 For queries or collaboration, feel free to reach out.
