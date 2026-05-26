# AI Duplicate Document Detection System

An AI-powered multi-format duplicate document detection system using OCR, Sentence Transformers, and semantic similarity analysis.

---

# Features

✅ Detect duplicate documents  
✅ Supports PDF, DOCX, JPG, JPEG, PNG  
✅ OCR support for scanned documents  
✅ Semantic similarity detection using transformers  
✅ Cosine similarity comparison  
✅ Near-duplicate detection  
✅ Google Colab compatible  

---

# Technologies Used

- Python
- Sentence Transformers
- all-MiniLM-L6-v2
- Tesseract OCR
- OpenCV
- PyPDF2
- pdf2image
- NumPy

---

# System Architecture

1. Upload files
2. Extract text
3. OCR processing (if needed)
4. Generate embeddings
5. Calculate cosine similarity
6. Detect duplicates

---

# Supported File Formats

| Format | Supported |
|--------|-----------|
| PDF | ✅ |
| DOCX | ✅ |
| JPG | ✅ |
| JPEG | ✅ |
| PNG | ✅ |

---

# Installation

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/AI-Duplicate-Document-Detection-System.git
```

## Open Project

```bash
cd AI-Duplicate-Document-Detection-System
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Run Project

```bash
python projectDL.py
```

---

# Google Colab Setup

Install required packages:

```python
!pip install sentence-transformers pytesseract pdf2image python-docx opencv-python PyPDF2
!apt-get install -y tesseract-ocr
!apt-get install -y poppler-utils
```

---

# How It Works

The system extracts text from uploaded documents using:

- PyPDF2 for digital PDFs
- OCR for scanned PDFs/images
- python-docx for DOCX files

Then:

- Text embeddings are generated using `all-MiniLM-L6-v2`
- Cosine similarity is computed
- Files above 90% similarity are marked as duplicates

---

# Similarity Threshold

| Similarity | Result |
|------------|--------|
| >= 90% | Duplicate |
| < 90% | Not Duplicate |

---

# Sample Output

```text
🆚 file1.pdf VS file2.docx
📊 Similarity: 95.32%
✅ DUPLICATE FILES
```

---

# Research Paper

This project is based on transformer embeddings and OCR-based semantic duplicate detection research.

---

# Future Improvements

- Add database integration
- Add Flask web app
- Add chunk-level embeddings
- Add support for TXT/HTML
- Improve OCR preprocessing
- Add GPU acceleration

---

# Screenshots

Add your screenshots inside the `screenshots/` folder.

---

# Author

Your Name

---

# License

This project is licensed under the MIT License.
