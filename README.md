# adisangarak.github.io
POC
# PDF Annotation Tool Proof of Concept Documentation

## Introduction

This documentation provides an overview of a simple web-based PDF annotation tool implemented using HTML, JavaScript, and two PDF libraries: pdf.js for rendering PDFs and pdf-lib for adding annotations/comments to the PDF. The purpose of this proof of concept is to showcase the basic functionality of the tool for adding comments to a PDF document.

## Features

1. **Displaying the Original PDF:**
   - The tool allows users to load and view a PDF document on an HTML canvas.
   - It uses pdf.js to render the original PDF on the canvas.
2. **Adding Comments:**
   - Users can enter comments in a text input field and add them to the PDF.
   - The added comments are displayed on the canvas at user-specified coordinates.
   - Comments are also embedded into the PDF document using pdf-lib.
3. **Displaying the Modified PDF:**
   - The tool displays the modified PDF (with comments) on a separate canvas.
   - pdf.js is used to render the modified PDF.
4. **Resetting the Comment Input:**
   - After adding a comment, the input field is reset for further annotations.

## Code Overview

### HTML Structure:

- The HTML structure includes two `<canvas>` elements for displaying the original and modified PDFs.
- It provides an input field for entering comments and a button for adding comments.
- Script tags load the required libraries for PDF rendering and manipulation.

### JavaScript Function (`main`):

- The `main` function is the entry point for the application.
- It initializes variables, including PDF URLs, canvas references, and an array to store comments.
- The function handles the following functionalities:
  - Displaying the original PDF on the canvas.
  - Adding comments to the canvas and embedding them into the PDF.
  - Displaying the modified PDF with comments.
  - Resetting the comment input field.

## Demonstration

1. **Load the Original PDF:**
   - Open the web application in a browser.
   - The original PDF is loaded and displayed on the canvas.
2. **Add Comments:**
   - Enter comments in the input field.
   - Click the "Add Comment" button to add comments to the canvas.
   - The comments are displayed on the canvas at the specified location.
3. **View Modified PDF:**
   - The modified PDF (with comments) is displayed on a separate canvas.
   - Users can observe the added comments in the PDF.
4. **Reset Comment Input:**
   - After adding comments, the input field is reset for further annotations.

## Usage Guidelines

- Replace the `'./example.pdf'` value in the code with the actual path or URL of the PDF you want to annotate.
- Adjust the comment display coordinates as needed in the code.
- Customize the font size, font type, and color for comment display.
- Ensure that the required PDF libraries (pdf.js and pdf-lib) are accessible via their specified URLs.

## Conclusion

This proof of concept demonstrates a basic PDF annotation tool that allows users to add comments to a PDF document. It combines the power of pdf.js for rendering PDFs and pdf-lib for annotating them. This tool can serve as a foundation for more advanced PDF annotation features in a web application.
