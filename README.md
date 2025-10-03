# Video-Search-Engine - Motive AI Summit 2025
A semantic video search engine built for the Motive AI Summit 2025 hackathon at IISc Bangalore. This system solves the Video Indexing and Search problem by enabling intelligent search through video footage using natural language queries.

## 🎯 Problem Statement

### Challenge
Build an AI model to index and search videos using text queries. Enable users to find relevant video snippets by describing content.

### Expected Deliverable
- Ability to pass in a search text input query and render a set of relevant videos
- Example queries: "videos with snow", "night time driving", "show me vehicle rollovers"
- Interface: Command line, API, or proper UI

### Vanilla Implementation Approach
1. Generate rich text descriptions of video scenes using vision-capable LLM
2. Store representations (vector embeddings) of these descriptions
3. Given a query, embed it and find descriptions with the greatest alignment
4. Return top k results

## 🚀 My Solution
I built a comprehensive video search system that follows the suggested approach with enhanced features:

### Key Features
- Natural Language Search: Query videos using everyday language
- Semantic Understanding: Uses Amazon Titan embeddings for contextual search
- Smart Reranking: Penalizes negated concepts (e.g., "no car crash" vs "car crash")
- Video Previews: Direct video playback with pre-signed S3 URLs
- Interactive UI: Gradio-based web interface
- Scalable Architecture: FAISS-based vector search for efficient similarity matching

### 🛠️ Tech Stack
- AI/ML: Amazon Bedrock (Titan Embeddings), FAISS
- Cloud: AWS S3, AWS IAM
- Backend: Python, Boto3
- Frontend: Gradio
- Vector Database: FAISS

### 📊 Performance
- Search Accuracy: High precision in semantic matching
- Response Time: Sub-second search results
- Scalability: Handles thousands of video descriptions
- Query Understanding: Handles complex queries with negation

### ✨ Beyond Vanilla Implementation
- Advanced Reranking: Context-aware penalty system for negated concepts
- Real-time Video Previews: Direct S3 integration for instant playback
- User-friendly Interface: Gradio UI instead of command-line
- Production-ready: Error handling and scalable architecture








