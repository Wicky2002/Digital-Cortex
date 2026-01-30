# AI Service

Python-based AI/ML service for Digital Cortex.

## Setup

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Structure

```
ai-service/
├── app/
│   ├── models/         # ML models
│   ├── services/       # AI services
│   ├── utils/          # Utility functions
│   └── api/            # API endpoints
├── tests/              # Test files
├── notebooks/          # Jupyter notebooks
└── requirements.txt
```

## Technology Stack

- Python 3.10+
- FastAPI
- TensorFlow
- LangChain
- OpenAI API
- Vector Database (Pinecone/Weaviate)
- NLTK/spaCy

## Features

### NLP Processing
- Text classification
- Named entity recognition
- Sentiment analysis
- Keyword extraction

### Semantic Search
- Vector embeddings
- Similarity search
- Contextual search

### Knowledge Graph
- Entity extraction
- Relationship detection
- Graph construction

## Development

```bash
python -m uvicorn app.main:app --reload  # Start development server
pytest                                     # Run tests
python -m app.scripts.train_model         # Train ML models
```

## API Endpoints

- `POST /api/ai/analyze` - Analyze text
- `POST /api/ai/search` - Semantic search
- `POST /api/ai/embeddings` - Generate embeddings
- `POST /api/ai/extract` - Extract entities
