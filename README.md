
# Multimodal AI Chatbot with Ollama

## Overview

Multimodal AI Chatbot is a local AI-powered application that enables users to upload and interact with multiple file formats, including PDF documents, Word files, images, and audio files. The system extracts content from uploaded files, processes the information, and generates intelligent responses using locally hosted Large Language Models through Ollama.

This project focuses on privacy-first AI by running inference locally without requiring cloud-based AI services.

---

## Features

### Document Processing

* PDF Text Extraction using PyMuPDF
* Word Document Processing (.docx)
* Multi-file Upload Support
* Automatic Content Extraction

### Image Understanding

* OCR-based Text Extraction
* Supports JPG, JPEG, PNG, GIF, and BMP formats
* Text Recognition using Tesseract OCR

### Audio Processing

* Speech-to-Text Conversion
* WAV, MP3, and FLAC Support
* Automatic Audio Transcription

### AI-Powered Question Answering

* Context-Aware Responses
* Local LLM Inference using Ollama
* TinyLlama Integration
* File-Based Question Answering

### Conversation Management

* Chat History Tracking
* Session-Based Conversations
* PDF Transcript Export

### User Interface

* Interactive Streamlit Dashboard
* Drag-and-Drop File Upload
* Real-Time AI Responses
* Modern Custom CSS Styling

---

## System Architecture

User Upload
↓
PDF / DOCX / Image / Audio
↓
Content Extraction
↓
Text Processing & Chunking
↓
Context Generation
↓
Ollama (TinyLlama)
↓
AI Response
↓
Conversation Storage
↓
PDF Export

---

## Supported File Types

| Category  | Supported Formats                   |
| --------- | ----------------------------------- |
| Documents | PDF, DOCX, DOC                      |
| Images    | JPG, JPEG, PNG, GIF, BMP            |
| Audio     | WAV, MP3, FLAC                      |
| Video     | MP4, AVI, MOV, MKV (Future Support) |

---

## Tech Stack

### Frontend

* Streamlit

### AI & NLP

* Ollama
* TinyLlama

### Document Processing

* PyMuPDF
* python-docx

### OCR

* Tesseract OCR
* OpenCV

### Speech Recognition

* SpeechRecognition

### Data Processing

* NumPy

### PDF Generation

* FPDF

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/multimodal-ai-chatbot.git
cd multimodal-ai-chatbot
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Install Ollama

Download and install Ollama:

https://ollama.com

Pull TinyLlama Model:

```bash
ollama pull tinyllama
```

Verify Installation:

```bash
ollama run tinyllama
```

---

## Run Application

```bash
streamlit run app.py
```

Application will be available at:

```text
http://localhost:8501
```

---

## Project Structure

```text
multimodal-ai-chatbot/

│
├── app.py
├── styles.css
├── requirements.txt
├── README.md
│
├── assets/
│   ├── screenshots/
│   ├── demo_images/
│
├── docs/
│   └── architecture.png
│
└── outputs/
    └── conversation.pdf
```

---

## Workflow

1. Upload one or more files.
2. Extract text from files.
3. Enter a question.
4. Generate AI response using TinyLlama.
5. View answer.
6. Export conversation as PDF.

---

## Example Use Cases

### Academic Research Assistant

Upload research papers and ask questions.

### Resume Analyzer

Upload resumes and extract insights.

### Document Q&A System

Query contracts, reports, and manuals.

### Image Text Reader

Extract information from screenshots and scanned documents.

### Audio Transcript Assistant

Convert speech recordings into searchable text.

---

## Future Enhancements

* Video Content Understanding
* RAG Pipeline Integration
* FAISS Vector Database
* ChromaDB Integration
* Llama 3 Support
* Mistral Support
* Multi-Agent Workflow
* Real-Time Voice Chat
* Document Summarization
* Local Embedding Models
* GPU Acceleration

---

## Skills Demonstrated

* Artificial Intelligence
* Large Language Models (LLMs)
* Natural Language Processing (NLP)
* OCR Systems
* Speech Recognition
* Python Development
* Streamlit Applications
* Local AI Deployment
* Multimodal AI Systems
* Document Intelligence

---

## Author

Suriya V

Computer Science Engineer | AI & Machine Learning Enthusiast

GitHub: https://github.com/YOUR_USERNAME

LinkedIn: https://linkedin.com/in/YOUR_LINKEDIN
