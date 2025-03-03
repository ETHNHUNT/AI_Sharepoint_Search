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

## requirements.txt
1. requests
2. faiss-cpu
3. ollama
4. gradio
5. python-dotenv
6. numpy
7. PyPDF2
8. docx2txt

## Future Enhancements 🚧

### Planned Features
- **Multi-Language Support**: Add multilingual search capabilities
- **Document Preview**: In-UI file content previews
- **Version Control**: Track document versions in index
- **Access Control**: RBAC integration with Azure AD groups
- **Hybrid Search**: Combine vector + keyword search
- **API Endpoints**: REST API for system integration
- **Notifications**: Email alerts for new matches

### Technical Roadmap
- **Performance Optimization**: 
  - Batch embedding generation
  - GPU-accelerated FAISS
- **Advanced NLP**:
  - Query expansion
  - Synonym recognition
- **Storage**:
  - Cloud sync for indexes
  - Delta indexing
- **Security**:
  - Audit logging
  - Encryption-at-rest

## Current Development 🔨

### In Progress
- **Real-Time Indexing**: Auto-update on document changes
- **UI Improvements**:
  - Paginated results
  - Relevance scoring visualization
- **Advanced Filters**:
  - Date range filtering
  - File type filters
- **Error Handling**:
  - Retry mechanisms
  - Detailed error logging

### Experimental Features
- **Chat Interface**: Conversational document Q&A
- **Cross-Site Search**: Unified search across multiple sites
- **Image OCR**: Text extraction from images/PDFs
- **Custom Models**: Fine-tuned embeddings for SharePoint
