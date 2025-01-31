# Document Analysis Tool

The **Document Analysis Tool** is a powerful application designed to analyze and process documents in various formats. It supports **PDFs**, **Word documents**, **text files**, and **images** (using OCR). The tool provides advanced features like **grammar checking**, **sentiment analysis**, **keyword extraction**, **summarization**, and more. It comes in two versions:

1. **Local Version**: A fully local version that does not rely on external APIs.
2. **API Version**: A version that integrates with OpenAI's GPT-3 for advanced features like **AI-powered writing continuation** and **tone adjustment**.

---

## Features

### Supported File Types
- **PDF**: Extract text from PDF files.
- **Word Documents**: Extract text from `.docx` files.
- **Text Files**: Read plain text files.
- **Images**: Extract text from images using **Tesseract OCR**.

### Core Features
- **Text Extraction**: Extract text from documents and images.
- **Word Frequency Analysis**: Identify the most common words in the document.
- **Summarization**: Generate a concise summary of the document.
- **Sentiment Analysis**: Determine the sentiment of the text (positive, negative, neutral).
- **Named Entity Recognition**: Extract entities like people, organizations, and locations.
- **Keyword Extraction**: Identify the most relevant keywords in the document.
- **Grammar Checking**: Check for grammar and spelling errors using LanguageTool.
- **Find and Replace**: Find and replace specific words or phrases in the document.

### Advanced Features (API Version Only)
- **AI-Powered Writing Continuation**: Use OpenAI's GPT-3 to continue writing based on the document's content.
- **Tone Adjustment**: Rewrite the document in a specified tone (e.g., formal, casual, persuasive).

---

## Installation

### Prerequisites
- Python 3.7 or higher.
- Tesseract OCR (for image text extraction).

### Step 1: Install Required Libraries
Run the following command to install the required Python libraries:

```bash
pip install PyPDF2 python-docx pytesseract pillow nltk spacy language-tool-python
```

For the **API version**, also install the OpenAI library:

```bash
pip install openai
```

### Step 2: Download NLTK Data and spaCy Model
Download the necessary NLTK data files and spaCy model:

```bash
python -m nltk.downloader punkt stopwords vader_lexicon
python -m spacy download en_core_web_sm
```

### Step 3: Install Tesseract OCR
- **Windows**: Download and install Tesseract from [here](https://github.com/tesseract-ocr/tesseract).
- **macOS**: Install via Homebrew:
  ```bash
  brew install tesseract
  ```
- **Linux**: Install via package manager:
  ```bash
  sudo apt install tesseract-ocr
  ```

---

## Usage

### Local Version
1. Run the tool:
   ```bash
   python local_document_analysis_tool.py
   ```
2. Use the GUI to:
   - Select a document (PDF, Word, text, or image).
   - View analysis results (text, word frequency, summary, sentiment, entities, keywords, grammar issues).
   - Perform advanced operations like **find and replace** and **tone adjustment**.

### API Version
1. Replace `"your_openai_api_key_here"` in the code with your OpenAI API key.
2. Run the tool:
   ```bash
   python api_document_analysis_tool.py
   ```
3. Use the GUI to:
   - Select a document.
   - View analysis results.
   - Perform advanced operations like **AI-powered writing continuation** and **tone adjustment**.

---

## Contributing
Contributions are welcome! If you'd like to contribute, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes.
4. Submit a pull request.

---

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **NLTK**: For natural language processing tasks.
- **spaCy**: For named entity recognition.
- **LanguageTool**: For grammar and spell-checking.
- **Tesseract OCR**: For text extraction from images.
- **OpenAI**: For AI-powered writing and tone adjustment (API version).

---

## Contributing
For any questions or support, please contact us:

1. **Feedback or cooperation suggestions**:  
   If you have ideas for features, improvements, or collaborations for another project, please contact us at:  
-chidungtran@proton.me

2. **Personal communication**:  
 - tranchidung152@protonmail.com

---
## Donations
Consider donating if you find this project helpful and would like to support its development. Your support helps maintain and improve the tool.

[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://www.paypal.com/donate?hosted_button_id=DE7NL3HFQYQ5Y)

Thank you for your generosity!
