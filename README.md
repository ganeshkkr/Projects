PDF Block Diagram Extractor and Langchain Integration
This project focuses on extracting block diagrams and their associated titles from a PDF, performing OCR on the images, and integrating Langchain for document retrieval tasks. The code extracts images and text from PDFs using PyMuPDF, applies OCR with Tesseract, and stores the extracted information. Additionally, Langchain is used to process document embeddings and answer queries based on the stored information.

Features
PDF Processing: Extracts block diagrams and titles from a PDF.
OCR Integration: Uses Tesseract for OCR to analyze image content.
Langchain Integration: Retrieves information from documents using Langchain's BM25 and FAISS retrievers.
Customizable Search: Allows users to search for specific titles and components within the PDF.

Requirements
Install the necessary Python packages using the following commands:
pip install pymupdf pytesseract Pillow langchain transformers faiss-gpu tiktoken sentence-transformers trl Py7zr optimum rank_bm25 pypdf

How to Run
1.Extract Block Diagrams: This function will extract diagrams and perform OCR.
pdf_path = "path/to/your/data.pdf"
output_folder = "path/to/your/output"
search_title = input("Enter the title to search for: ")
search_component = input("Enter the component to search for: ")
data = extract_block_diagrams_with_titles(pdf_path, output_folder, search_title, search_component)

2.
