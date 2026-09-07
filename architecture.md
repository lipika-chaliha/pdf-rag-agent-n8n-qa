# Architecture

## Objective

Build a RAG pipeline that allows an AI Agent to answer questions using information retrieved from a PDF rather than relying only on the model's general knowledge.

## Flow

1. **PDF ingestion**
   - A PDF is supplied as the source document.

2. **Text extraction**
   - Text is extracted from the document.

3. **Chunking**
   - The document is divided into smaller chunks so relevant sections can be retrieved efficiently.

4. **Embeddings**
   - Text chunks are converted into vector representations.

5. **Vector storage**
   - Embeddings and their associated text are stored in a vector database/store.

6. **Retrieval**
   - A user question is converted into a search query.
   - Relevant document chunks are retrieved.

7. **AI Agent**
   - The retrieved context is supplied to the AI Agent.
   - The agent generates an answer based on the retrieved information.

## QA-oriented architecture

```text
Requirements / BRD / API Docs / Defect History / Release Notes
                         ↓
                  Document Ingestion
                         ↓
                    Chunk + Embed
                         ↓
                    Vector Store
                         ↓
                       RAG
                         ↓
                    AI Agent
                         ↓
          ┌──────────────┴──────────────┐
          ↓                             ↓
    Testing Questions              QA Outputs
          ↓                             ↓
   Relevant retrieval       Test scenarios / test cases /
                            API ideas / defect analysis /
                            regression suggestions

```

## Key principle

The important part of RAG is not simply asking an AI model a question.

The important part is **retrieving relevant information from the source before generating the answer**.

This helps make the workflow more grounded in project-specific information.

## Security

Never commit:

- API keys
- passwords
- access tokens
- n8n credentials
- private company documents
- customer data
- confidential requirements or defect data

Use environment variables or n8n credentials for secrets.
