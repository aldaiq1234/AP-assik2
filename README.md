Here is the `README.md` file for your project written in English:

```markdown
# Ollama Chatbot with File Uploads

## Description

This project is a chatbot that allows users to upload documents and ask questions based on their content. The bot provides answers using the context of the uploaded files and integrates with **Ollama API** to generate responses.

## Features

- Upload files in `.txt`, `.pdf`, and `.docx` formats (either one or multiple files at a time).
- Extract text from uploaded files.
- Save the content of the files to the **ChromaDB** database for context-based search.
- Answer user questions related to the content of uploaded documents.
- Provide a search functionality for query history.


1. Create and activate a Python virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/macOS
   venv\Scripts\activate     # For Windows
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure that the Ollama API is running on a local server (e.g., `http://localhost:11434`).

## Usage

1. Run the application:
   ```bash
   streamlit run src/AP.py
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:8501
   ```

3. Upload files through the interface and ask questions based on their content.

## Examples

- Upload a file named `example.txt` with the content:
  ```
  The capital of France is Paris.
  ```
- Ask the question: `What is the capital of France?`
- The bot will respond: `The capital of France is Paris.`

## Repository Structure

```
Project/
├── README.md            # Documentation
├── LICENSE              # License
├── requirements.txt     # List of dependencies
├── src/                 # Source code
│   ├── AP.py            # Main application
├── test/                # Tests
│   ├── test_main.py     # Tests for functions
```

## Dependencies

- `streamlit`: User interface framework.
- `chromadb`: Database for context-based search.
- `PyPDF2`: For handling `.pdf` files.
- `python-docx`: For handling `.docx` files.
- `requests`: For communication with Ollama API.

Install all dependencies using the `requirements.txt` file.
