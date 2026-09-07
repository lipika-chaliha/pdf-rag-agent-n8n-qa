# Setup Checklist

## Before publishing

- [ ] Remove API keys
- [ ] Remove passwords
- [ ] Remove access tokens
- [ ] Remove private/company PDFs
- [ ] Remove customer or production data
- [ ] Remove n8n credentials from exported workflow files
- [ ] Check screenshots for sensitive information

## n8n

1. Build or open the RAG workflow in n8n.
2. Export the workflow as JSON.
3. Review the exported JSON carefully.
4. Remove or sanitize any credentials/secrets.
5. Save the sanitized file under `workflows/`.
6. Add a short explanation of the nodes and their purpose.

## Recommended repository additions

- Sanitized workflow JSON
- Architecture screenshot
- Example input PDF using public/non-confidential content
- Example questions
- Example outputs
- Short demo video

## Reproducibility

Document:

- n8n version
- LLM/provider used
- Embedding model
- Vector store
- Chunking approach
- Retrieval settings
- Any important prompts
