# OCRLinguist
A tool to translate Multilingual Legal Document PDFs to English using Tesseract, EasyOCR and EasyNMT's Opus-MT Machine Translation model locally

### How to use this tool?

1. Clone the repository to your system
2.


### For the poppler file 

Windows
1. Download the latest package from http://blog.alivate.com.au/poppler-windows/
2. Extract the package
3. Move the extracted directory to the desired place on your system
4. Add the bin/ directory to your PATH
5. Test that all went well by opening cmd and making sure that you can call pdftoppm -h

### For Tesseract-OCR

1. Install tesseract using windows installer available at: https://github.com/UB-Mannheim/tesseract/wiki

2. Note the tesseract path from the installation.Default installation path at the time the time of this edit was: C:\Users\USER\AppData\Local\Tesseract-OCR. It may change so please check the installation path.

3. pip install pytesseract

4. Set the tesseract path in the script before calling image_to_string:

pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract'

**Note**: Change the location according to the location where you set up Tesseract locally
