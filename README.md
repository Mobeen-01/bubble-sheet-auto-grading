# 📄 Automated Bubble Sheet Grading System

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg?style=flat&logo=python)](https://www.python.org)
[![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00.svg?style=flat&logo=googlecolab)](https://colab.research.google.com)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.x-blue.svg?style=flat&logo=opencv)](https://opencv.org/)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## 📌 Process Single Images & PDFs for Auto-Grading with Barcode Tracking

This Google Colab-based system automates bubble sheet grading for Spanish-language multiple-choice tests. It detects marked answers, extracts barcodes for student identification, and saves results in a CSV file.

It supports: <br> 
✅ Single image processing (`Image_input.ipynb`). <br> 
✅ Multi-page PDF processing (`Pdf_input.ipynb`). <br> 

The system automatically grades 60 blocks per sheet, stores student responses, and marks detected answers on the output image.

## 📌 Features
✅ **Single Image & Multi-Page PDF Support** – Process individual or batch answer sheets.  
✅ **Automated Answer Detection** – Extracts responses from bubble sheets.  
✅ **Barcode Recognition** – Identifies students via barcode.  
✅ **Auto-Saves to CSV** – Results are stored in `processed_blocks_info.csv`.  
✅ **No Manual Setup Needed** – Creates a CSV file if it doesn't exist.  
✅ **Marks & Highlights Answers** – Generates annotated output images.  
✅ **Sample Inputs & Outputs Included** – Test with pre-loaded files.  

## 🚀 How to Use

### 1️⃣ Open Google Colab
Go to [Google Colab](https://colab.research.google.com/).

### 2️⃣ Choose the Right Notebook
📌 For a **single image**, use `Image_input.ipynb`.  
📌 For **PDFs with multiple sheets**, use `Pdf_input.ipynb`.  

### 3️⃣ Upload Your Files
- Click the folder icon in Colab's left panel.  
- Upload your image or PDF in the `inputs/` folder.  

### 4️⃣ Update File Paths  
Modify the file paths accordingly:

```python
# For image input
image_path = '/content/inputs/your_uploaded_image.jpg'  # Replace with your file

# For PDF input
pdf_path = '/content/inputs/your_uploaded_file.pdf'  # Replace with your file
```

### 5️⃣ Run the Notebook  
Click **Runtime > Run all** to process the sheets.  

### 6️⃣ View Results  
📄 **Results CSV**: Located at `/content/processed_blocks_info.csv`.  
🖼 **Annotated Image Output**: View in `outputs/`, highlighting detected answers.  

## 📂 Input & Output Files

### 📥 Inputs (Located in `inputs/`)
- **Sample Answer Sheet (Image & PDF)** – Use for testing.  
- **Barcodes** – Automatically extracted from student sheets.  

### 📤 Outputs (Located in `outputs/`)
- **Annotated Answer Sheet Image** – Shows detected answers with markings.  
- **Processed CSV File (`processed_blocks_info.csv`)** – Stores student answers (60 blocks).  
📌 *Even if the CSV does not exist, the system automatically creates it and records responses!*  

## 💡 Impact
🔹 **Eliminates Manual Grading Errors** – Ensures accurate and reliable evaluation.  
🔹 **Saves Time** – Fully automates bubble sheet assessment.  
🔹 **Student Barcode Tracking** – Associates answers with individual students.  
🔹 **Data-Driven Insights** – Generates structured reports.  
🔹 **Visual Answer Marking** – Helps review and verify detected responses.  

## 🛠 Tech Stack
🔹 **Python** – Core processing logic.  
🔹 **Google Colab** – Cloud execution environment.  
🔹 **OpenCV** – Image processing for answer detection.  
🔹 **NumPy & Pandas** – Data handling and CSV integration.  
🔹 **Tesseract OCR** – Extracting barcode data.  
🔹 **PyMuPDF / PDFPlumber** – Processing multi-page PDFs.  
🔹 **Matplotlib** – Generating annotated answer sheets.  

## 📜 Notes
📌 The system marks all **60 blocks per sheet**, ensuring complete grading.  
📌 A **sample output format** is provided based on client requirements.  
📌 Works for **Spanish-language bubble sheets**.  
