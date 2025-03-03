# SharePoint AI Search 🔍

An intelligent search solution for SharePoint documents using Ollama embeddings and FAISS vector search.

## Features ✨
- Natural language document search
- Secure Azure AD authentication
- FAISS vector indexing
- Gradio web interface
- Support for PDF/DOCX/XLSX files

## Architecture 🏛️

![image](https://github.com/user-attachments/assets/edfe3346-c426-4890-95a4-dbc91bd837ba)


## Installation 📦
1. Clone repo:
git clone https://github.com/yourusername/sharepoint-ai-search.git
cd sharepoint-ai-search

2. Install dependencies:
pip install -r requirements.txt

3. Configure environment (rename .env.example to .env):
TENANT_ID="your_tenant_id"
CLIENT_ID="your_client_id"
CLIENT_SECRET="your_client_secret"

## Usage 🚀
1. Start Jupyter notebook:
2. Run cells in order:
  Authentication
  Site/Drive configuration
  Document indexing
  Launch search interface

3. Access Gradio UI at http://localhost:7860

Security 🔒
Credentials stored in environment variables
Azure AD OAuth2 client credentials flow
Local FAISS index storage
Token-based SharePoint access

Troubleshooting 🐛
Issue	Solution
401 Errors	Verify Azure AD permissions
Missing Documents	Check SharePoint API access
Embedding Failures	Confirm Ollama service running
Index Errors	Rebuild FAISS index

## requirements.txt

requests==2.32.3
faiss-cpu==1.10.0
ollama==0.4.6
gradio==5.20.0
python-dotenv==1.0.0
numpy==2.2.2
PyPDF2==3.0.1
docx2txt==0.8
LICENSE (MIT template)

text
Copy
MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted...
For the architecture diagram:

Create an architecture.png using the mermaid code

Place in docs/ folder

Update the README image reference

Before committing:

Remove/obfuscate credentials

Delete notebook outputs

Verify .env is in .gitignore

Add sample documents for testing

This structure provides:

Clear documentation

Security best practices

Easy replication

Proper licensing

Troubleshooting help

Version control hygiene
