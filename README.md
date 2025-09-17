# RAGUdemy - Document Parsing and RAG Implementation

This project contains examples and implementations for document parsing, text processing, and Retrieval Augmented Generation (RAG) using LangChain.

## Project Structure

```
RAGUdemy/
├── 0-DocumentParsing/          # Document processing examples
│   ├── 1-documentIngestion.ipynb      # Text document ingestion
│   ├── 2-pdfingestion.ipynb          # PDF document processing
│   ├── 3-databaseingestion.ipynb     # Database integration
│   ├── 4-documentembedding.ipynb     # Document embeddings
│   ├── 5-practise.ipynb              # Practice exercises
│   ├── 6-graph-knowledge-search.ipynb # Graph-based search
│   └── data/                          # Sample data files
├── .gitignore                     # Comprehensive gitignore for ML projects
├── .env.template                  # Environment variables template
├── requirements.txt               # Python dependencies
└── pyproject.toml                # Project configuration
```

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/jchowdhary/RAGPractice.git
cd RAGPractice
```

### 2. Create Virtual Environment
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables
```bash
# Copy the template and add your API keys
cp .env.template .env

# Edit .env and add your actual API keys:
# OPENAI_API_KEY=your_actual_api_key_here
```

### 5. Start Jupyter Notebook
```bash
jupyter notebook
```

## Features

- **Document Ingestion**: Load and process various document types
- **Text Splitting**: Chunk documents for optimal processing
- **Vector Embeddings**: Convert text to vector representations
- **ChromaDB Integration**: Persistent vector storage
- **RAG Implementation**: Retrieval Augmented Generation examples
- **Graph Knowledge Search**: Advanced search using knowledge graphs

## Important Notes

### Security
- ⚠️ **Never commit API keys to version control**
- Use the provided `.env.template` to set up your environment variables
- All notebook outputs have been cleared to prevent accidental key exposure

### Large Files
- The `.gitignore` is configured to exclude:
  - Large data files (PDFs, binary files)
  - Database files and ChromaDB storage
  - Model weights and checkpoints
  - Virtual environments

### Getting API Keys
- **OpenAI**: Get your API key from [OpenAI Platform](https://platform.openai.com/api-keys)
- **Anthropic**: Get your API key from [Anthropic Console](https://console.anthropic.com/)
- **HuggingFace**: Get your token from [HuggingFace Settings](https://huggingface.co/settings/tokens)

## Usage Examples

1. **Start with `1-documentIngestion.ipynb`** for basic document loading
2. **Progress to `2-pdfingestion.ipynb`** for PDF processing
3. **Try `4-documentembedding.ipynb`** for vector embeddings
4. **Explore `6-graph-knowledge-search.ipynb`** for advanced search

## Troubleshooting

### Common Issues

1. **Missing API Key Error**: Make sure you've created `.env` file with your API keys
2. **Module Not Found**: Ensure you're in the virtual environment and have installed dependencies
3. **Large File Errors**: The `.gitignore` should prevent this, but if you encounter issues, check for accidentally committed large files

### Data Directory Structure
The data directory contains sample files for testing:
- `text_files/`: Sample text documents
- `pdf/`: Sample PDF files (excluded from git)
- `database/`: Sample database files
- `chroma/`: ChromaDB storage (excluded from git)

## Contributing

When contributing:
1. Never commit API keys or secrets
2. Clear notebook outputs before committing
3. Keep data files under the size limits
4. Update the `.gitignore` if you add new file types

## License

This project is for educational purposes as part of the KrishAcademy curriculum.