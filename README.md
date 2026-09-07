# PDF RAG Agent with n8n for AI-Powered Software Testing

A hands-on Retrieval-Augmented Generation (RAG) project built with n8n.

## 🎯 Project Overview

PDF
 ↓
Document Loader
 ↓
Text Splitter
 ↓
OpenAI Embeddings
 ↓
Vector Store
 ↓
Retriever
 ↓
AI Agent
 ↓
Grounded Answer

## 🔍 How It Works

### Document ingestion

PDF → Load → Split → Embed → Store

### Question answering

Question → AI Agent → Retrieve relevant content → Grounded response

## 🔄 n8n Workflow

The following workflow demonstrates the complete PDF ingestion and RAG-based question-answering flow.

![PDF RAG Agent n8n Workflow](pdf-rag-agent-workflow.png)

## 🧪 QA Demonstration

### Example 1 — Requirement Retrieval

**Input:**  
Software Requirements Specification (SRS) PDF

**Question:**  
"What are the functional requirements related to user login?"

**RAG Agent:**  
Retrieves the relevant content from the uploaded PDF.

**Output:**  
A grounded answer based on the relevant retrieved content from the document.

---

### Example 2 — Test Scenario Generation

**Question:**  
"Generate test scenarios for the password reset requirement."

**RAG Agent:**  
Retrieves the relevant password reset requirement from the document and uses it as context.

**Example Output:**

1. Verify password reset using a registered email.
2. Verify handling of an unregistered email.
3. Verify an expired password reset link.
4. Verify password policy validation.
5. Verify successful password reset with valid input.
6. Verify appropriate error handling for invalid input.

> **Note:** These examples demonstrate the intended QA use cases. Actual answers depend on the content of the PDF provided to the workflow.

## 🧪 Software Testing Use Cases

- Requirements → Test Scenarios
- BRDs → Test Cases
- API Documentation → API Test Ideas
- Defect History → Defect Analysis
- Release Notes → Regression Testing

## 🛠️ Technology

- n8n
- Retrieval-Augmented Generation (RAG)
- OpenAI embeddings
- Vector Store
- AI Agent
- Conversational Memory

## 🔐 Security

This repository contains a sanitized workflow.

No API keys, passwords, private documents, or production credentials are included.

## ⚠️ Demo / Learning Project

The workflow uses an in-memory vector store and is intended as a hands-on proof of concept and learning project rather than a production deployment.

## 👩‍💻 Author

Lipika Chaliha

AI-Driven QA Test Lead | Software Testing | AI Agent Development with n8n
