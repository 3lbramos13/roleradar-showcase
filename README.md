# RoleRadar

RoleRadar is an AI-assisted career preparation platform that converts complex resumes into structured candidate profiles, preserves source evidence, and generates role-relevant preparation experiences.

> This repository is a public project showcase. Production source code is maintained privately and is not distributed because of intellectual-property, privacy, and security requirements.

## My Role

**AI / Full-Stack Engineer**

- Designed the document-ingestion and structured-profile pipeline.
- Built layout-aware resume extraction with conditional OCR fallback.
- Developed full-stack product surfaces for resume review, saved roles, and interview preparation.
- Designed evidence-grounded retrieval and candidate-profile data models.
- Integrated voice-based interview experiences with controlled transcript capture.
- Implemented validation, privacy boundaries, and expiring browser workspaces.

## What the Product Demonstrates

- Native PDF text extraction with coordinate-aware layout reconstruction
- OCR fallback for scanned or low-quality documents
- Structured work history, skills, education, target roles, and search keywords
- Evidence-linked resume chunks for grounded retrieval
- Role analysis and interview preparation based on candidate context
- Voice-based mock interview interaction
- Privacy-conscious temporary workspaces with automatic expiration

## Architecture

1. **Classify** - evaluate native text quality and determine whether OCR is required
2. **Reconstruct** - recover columns, blocks, and reading order from document coordinates
3. **Structure** - normalize candidate roles, employers, dates, skills, and education
4. **Persist** - store candidate facts, source evidence, and application state in PostgreSQL
5. **Retrieve** - use embeddings and pgvector to ground downstream AI features
6. **Interact** - deliver role preparation and voice-based interview experiences

## Technology

- Next.js, React, and TypeScript
- Custom responsive CSS
- PostgreSQL and pgvector
- PDF parsing and layout reconstruction
- Tesseract.js OCR
- Zod validation
- Vapi Voice AI
- Vercel deployment

## Demo

- [Live Demo](https://role-radar-neon.vercel.app/)
- [Product Walkthrough](https://youtu.be/mMojkcUaCUg)

## Source Availability

This repository intentionally contains no production source code, environment configuration, credentials, uploaded resumes, candidate information, database exports, or proprietary assets.

A technical walkthrough and selected implementation details are available upon request.

## Usage and Rights

All project descriptions and materials are provided for portfolio review only. No license is granted to copy, redistribute, or reuse the private implementation.
