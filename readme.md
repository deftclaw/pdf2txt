# pdf -> txt  
_converts *.pdf files to plaintext files_  

## Description:  

__Synopsis__  
pdf2txt was originally written for storing web-article walkthroughs as plaintext. This way 
you can collect tons of information in a small form-factor which is easily pushed to github.


__Methodology__  
 - __Dependencies:__  
   - `Imagemagick`  
     - Ensure: `ghostscript` _usually installs as a dependency of Imagemagick_  
   - `Tesseract` _aka_ `Tesseract-ocr`  

1. Converts input PDF file to TIFF image format (compatible with Tesseract)  
  - Note: this _copies_ the PDF -> TIFF with approximately the same file size, depending on colors/text-density  
2. Analyzes the TIFF file with OCR to convert the pixels to text-characters  

## Usage:  
1. `. pdf2txt /path/to/document.pdf` _you could also_ `chmod u+x pdf2txt; ./pdf2txt /path/to/document.txt`  
