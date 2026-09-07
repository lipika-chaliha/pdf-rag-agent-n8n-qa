# PDF RAG Agent with n8n for AI-Powered Software Testing

A hands-on Retrieval-Augmented Generation (RAG) project built with n8n.

The goal is simple:

**PDF → searchable knowledge → AI Agent → relevant retrieval → grounded answer**

This project explores how the same architecture can support Software Testing and Quality Engineering use cases such as:

- Requirements → Test Scenarios
- BRDs → Test Cases
- API Documentation → API Test Ideas
- Defect History → Defect Analysis
- Release Notes → Regression Testing

## Why this project?

A normal LLM can generate an answer from its general knowledge, but a RAG workflow first retrieves relevant information from a source document and uses that information to ground the response.

For QA teams, this creates opportunities to connect AI assistance with project-specific testing knowledge.

## High-level workflow

```text
PDF Document
    ↓
Document/Text Extraction
    ↓
Chunking
    ↓
Embeddings
    ↓
Vector Store
    ↓
Retriever
    ↓
AI Agent
    ↓
Question + Retrieved Context
    ↓
Grounded Answer
```

## Repository structure

```text
pdf-rag-agent-n8n-qa/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── architecture.md
│   ├── qa-use-cases.md
│   └── setup-checklist.md
├── examples/
│   ├── sample-questions.md
│   └── sample-qa-scenarios.md
└── workflows/
    └── README.md
```

## Important note

The repository intentionally does **not** contain API keys, credentials, private company documents, or other secrets.

The n8n workflow export can be added under `workflows/` after removing credentials/secrets from the exported workflow.

## Current status

- [x] PDF RAG concept documented
- [x] QA use cases documented
- [x] Architecture documented
- [x] Example questions and QA scenarios added
- [ ] Sanitized n8n workflow export
- [ ] Demo screenshots
- [ ] Short demo video

## Author

**Lipika Chaliha**

AI-Driven QA Test Lead | Manual Testing Expert | AI Agent Building with n8n

LinkedIn: https://www.linkedin.com/in/lipika-chaliha-5b4902b

---

If you find this useful, feel free to ⭐ the repository or share ideas for additional RAG-based QA use cases.
