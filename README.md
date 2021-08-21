# OCRLinguist
A tool to translate Multilingual Legal Document PDFs to English using Tesseract, EasyOCR and EasyNMT's Opus-MT Machine Translation model locally

### How to use this tool?

1. Clone the repository to your system
2. Run the Setting Up Environment Jupyter Notebook while using it for the first time
3. Place the PDFs in "PDFDataFolder" in your system and specify the document name or "all" feature according to your choice
4. Run the Converting PDF to Image file if you haven't already converted it or directly place the Images in "ImageDataFolder"
5. Choose the models to run accordingly from the following
 - **Primary Model** - OCR-Translation1-(Nolanguagespecified): Using Tesserract and OpusMT model for translation. Automatically detects the language and translates the text to English
 -  OCR-Translation1-(languagespecified): Using EasyOCR and OpusMT model for translation. For EasyOCR, you are required to know the language of the PDF in advance and specify it in the Jupyer Notebook
 -  **Use in case of special characters** - 
6. You will find the translated .txt file in the "OutputText" folder
7. To convert the .txt file to PDF, run the Text2PDF Jupyter Notebook


### For the poppler file 

Windows
1. Download the latest package from http://blog.alivate.com.au/poppler-windows/
2. Extract the package
3. Move the extracted directory to the desired place on your system
4. Add the bin/ directory to your PATH
5. Test that all went well by opening cmd and making sure that you can call pdftoppm -h

### For Tesseract-OCR

pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract'

**Note**:  Note the tesseract path from the installation. Default installation path was: r'C:\Program Files\Tesseract-OCR\tesseract'. It may change so please check the installation path. Change the location according to the location where you set up Tesseract locally
