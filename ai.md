### How it works

BM25 ranks documents based on:

- Term frequency (how often a word appears)
- Inverse document frequency (how rare the word is)
- Document length normalization

👉 It matches **exact words** between query and documents.

### Key characteristics

- No embeddings
- No semantic understanding
- Fast and lightweight
- Works best for exact keyword matching

### Example

Query: `"bank transfer delay"`

BM25 will favor documents containing:

- “bank”
- “transfer”
- “delay”

Even if the meaning is similar but words differ, it may miss them.

**Type:** Vector similarity search (semantic retrieval)  
**Developed by:** Meta (Facebook AI)

### How it works

- Text is converted into **embeddings** using models (e.g., BERT, OpenAI embeddings)
- FAISS indexes these vectors
- It retrieves documents based on **vector similarity** (cosine similarity / L2 distance)

👉 It matches **meaning**, not just words.

### Key characteristics

- Semantic understanding
- Handles synonyms and paraphrasing
- Requires embedding model
- Highly scalable for large datasets
- Faster approximate nearest neighbor (ANN) search

### Example

Query: `"bank transfer delay"`

FAISS may retrieve documents containing:

- “payment not received”
- “transaction pending”
- “funds not credited”

Even if exact words don’t match.
