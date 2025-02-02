# PDF Utility Script

This repository contains a Python script to perform various PDF operations using the `PyPDF2` library, including merging PDFs, rotating pages, and adding watermarks.

## Features
- **Merge PDFs**: Combine multiple PDF files into a single document.
- **Rotate PDFs**: Rotate the pages of a PDF file.
- **Watermark PDFs**: Apply a watermark to each page of a PDF.

## Prerequisites
- Python 3.x
- `PyPDF2` module (install using `pip install PyPDF2`)

## Installation
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
### Merging PDFs
Run the script and provide a list of PDF files to merge:
```sh
python script.py file1.pdf file2.pdf file3.pdf
```
Output:
```
Merged file saved as main1.pdf
```

### Rotating a PDF Page
Ensure `main2.pdf` exists in the working directory, then run:
```sh
python script.py
```
Output:
```
Rotated page saved as tilt.pdf
```

### Adding a Watermark
Ensure `main3.pdf` (target PDF) and `wtr.pdf` (watermark file) exist in the directory:
```sh
python script.py
```
Output:
```
Watermarked file saved as WMpdf.pdf
```

## Notes
- The script uses `rb` (read binary) and `wb` (write binary) modes as required for handling PDF files.
- The watermark is applied from the first page of `wtr.pdf` to all pages of `main3.pdf`.
- Modify the filenames in the script accordingly to work with different PDFs.

## License
This project is licensed under the MIT License.

