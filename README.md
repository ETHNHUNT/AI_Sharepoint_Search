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

## Security 🔒
1. Credentials stored in environment variables
2. Azure AD OAuth2 client credentials flow3. 
Local FAISS index storage
4. Token-based SharePoint access

## Troubleshooting 🐛
  Issue	                  Solution
1. 401 Errors	            Verify Azure AD permissions
2. Missing Documents	    Check SharePoint API access
3. Embedding Failures	    Confirm Ollama service running
4. Index Errors	          Rebuild FAISS index

## requirements.txt
1. requests
2. faiss-cpu
3. ollama
4. gradio
5. python-dotenv
6. numpy
7. PyPDF2
8. docx2txt
