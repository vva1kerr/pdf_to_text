# OCR Web Application

A Streamlit web application that uses PyOCR to extract text from images and PDFs.

## Prerequisites

Before running this application, you need to install Tesseract-OCR and Poppler on your system:

### Ubuntu/Debian
```bash
sudo apt-get update
sudo apt-get install tesseract-ocr poppler-utils
```

### Windows
1. Download and install Tesseract-OCR from: https://github.com/UB-Mannheim/tesseract/wiki
2. Download and install Poppler from: http://blog.alivate.com.au/poppler-windows/
3. Add both Tesseract and Poppler to your system PATH

### macOS
```bash
brew install tesseract poppler
```

## Setup

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install the required Python packages:
```bash
pip install -r requirements.txt
```

## Running the Application

1. Activate your virtual environment if not already activated:
```bash
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Run the Streamlit app:
```bash
streamlit run app.py
```

3. Open your web browser and navigate to the URL shown in the terminal (typically http://localhost:8501)

## Usage

### For Images:
1. Upload an image file (PNG, JPG, or JPEG)
2. Click "Extract Text" to process the image
3. View the extracted text
4. Download the text if needed

### For PDFs:
1. Upload a PDF file
2. Select a specific page to process or choose to process all pages
3. Click "Extract Text" to process the selected page or "Process All Pages" to extract text from all pages
4. View the extracted text
5. Download the text (individual page or all pages)

## Features

- Image upload support (PNG, JPG, JPEG)
- PDF upload support with multi-page processing
- Page selection for PDFs
- Real-time text extraction
- Download extracted text
- User-friendly interface
- Support for multiple file formats

## Notes

- For best results, use clear, well-lit images with good contrast
- The application uses English language by default for OCR
- Processing time may vary depending on file size and complexity
- PDF processing may take longer than image processing due to the conversion step
