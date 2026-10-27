# Bedrock Banking Document Assistant

An AI-powered banking document assistant built with **Java, Spring Boot, and Amazon Bedrock**.

## Overview

This project allows users to upload banking procedure documents and ask questions about their content. The application uses a Large Language Model (LLM) through Amazon Bedrock to generate answers grounded in the retrieved document information.

## Objectives

- Integrate Amazon Bedrock with Spring Boot.
- Understand how foundation models work in real applications.
- Implement Retrieval-Augmented Generation (RAG).
- Explore embeddings and vector search.
- Build secure REST APIs for document management and question answering.
- Reduce hallucinations by grounding answers in retrieved sources.

## Technologies

- Java
- Spring Boot
- Amazon Bedrock
- AWS SDK for Java
- REST API
- Vector database (to be selected)
- Docker (optional)

## Main Features

- Upload banking procedure documents.
- Extract and prepare document content for search.
- Retrieve relevant passages based on user questions.
- Generate answers using Amazon Bedrock.
- Return answers with references to the source documents.
- Handle unsupported questions when the documents do not contain enough information.

## Architecture

1. The user uploads a document through a Spring Boot REST API.
2. The application extracts and splits the document into chunks.
3. The chunks are converted into embeddings and stored in a vector database.
4. The user submits a question.
5. The application retrieves the most relevant document chunks.
6. Amazon Bedrock generates an answer using the retrieved context.
7. The API returns the answer and its supporting sources.

## Learning Roadmap

- [ ] Set up the Spring Boot project.
- [ ] Configure AWS credentials and Bedrock access.
- [ ] Send a prompt to a foundation model.
- [ ] Build document upload and text extraction.
- [ ] Generate embeddings and implement vector search.
- [ ] Implement the RAG workflow.
- [ ] Return answers with document references.
- [ ] Add validation, error handling, and security.
- [ ] Write integration tests and document the API.

## Security

- Never commit AWS credentials or secrets.
- Use IAM permissions with least privilege.
- Avoid uploading real customer or confidential banking data.
- Validate document uploads and protect sensitive information.

## Goal

Learn how to integrate foundation models into a backend application and build a practical AI solution using Amazon Bedrock and Spring Boot.
