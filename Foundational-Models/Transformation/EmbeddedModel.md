# Embedding Model
- An embedding model is a neural network trained to map inputs into this vector space. During training it processes billions of text examples and adjusts its weights so that words appearing in similar contexts get similar vectors. The result is a function:
- The specific numbers don't mean anything on their own. What matters is the relative positions — the distances and angles between vectors.

```
text → fixed-length vector (e.g. 768 or 1536 numbers)
```

# Measuring similarity: cosine similarity
- The most common way to compare two vectors is cosine similarity — it measures the angle between them, not their raw distance. The formula:
- Using angle rather than raw distance is important because it's length-invariant — a short sentence and a long sentence about the same topic should still be "similar" even if their vectors have different magnitudes.

````
similarity = (A · B) / (|A| × |B|)
````

This returns a value between −1 and 1:
- 1.0 → identical direction (very similar meaning)
- 0.0 → perpendicular (unrelated)
- −1.0 → opposite direction (antonyms, conceptually)

# Where embeddings are used?
- Semantic search — instead of matching keywords, you embed both the query and all documents, then find the nearest vectors. "How do I fix a leaky pipe?" finds plumbing guides even if they never contain those exact words.
- Retrieval-Augmented Generation (RAG) — store document embeddings in a vector database (Pinecone, pgvector, Chroma), embed the user's question at query time, retrieve the closest chunks, and feed them to an LLM.
- Recommendation systems — items and users are embedded; nearest-neighbor lookup finds "people like you also liked…"
- Clustering and anomaly detection — group similar items or flag outliers that are far from all clusters.
- Classification — train a lightweight classifier on top of embeddings rather than raw text.

