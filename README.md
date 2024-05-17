# Bill Text Extraction

This project extracts text from an image of a bill, preprocesses the image to enhance text recognition, and then parses the text to extract relevant information such as item names and prices.

## Features

- Preprocesses the image to convert the background to white and text to black.
- Extracts text from the preprocessed image using `pytesseract`.
- Parses the extracted text to identify consumed items and their prices.
- Dynamically identifies and extracts key-value pairs from the text.

## Requirements

- Python 3.x
- pytesseract
- Pillow
- re
- json

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/H-Neethika/Extraction-of-attributes-from-a-Bill.git
    cd Extraction-of-attributes-from-a-Bill
    ```

2. Install the required packages:

    ```bash
    pip install pytesseract Pillow
    ```

3. Install Tesseract OCR:

    - **Windows:** Download the installer from [Tesseract at UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki) and follow the installation instructions.
    - **macOS:** Install via Homebrew:

      ```bash
      brew install tesseract
      ```

    - **Linux:** Install via your package manager, for example:

      ```bash
      sudo apt-get install tesseract-ocr
      ```

## Usage

1. Place your bill image in the project directory.

2. Update the `image_path` variable in the script to point to your bill image file.

3. Run the script:

4. The script will preprocess the image, extract text, and print the parsed information in JSON format.
