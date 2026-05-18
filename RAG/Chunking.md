# Types of Chunking

|                                 | Description                                                                                      | Use Cases                                                                  |
|---------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| :star: Recursive Chunking       | Split hierarchically - paragraphs, sentences, words                                              | Default RAG<br/>- PDF<br/>- documentation                                  |
| :star: Structure-Aware Chunking | Chunk according to headings, sections, markdown HTML,tables, code blocks                         | API docs, notion, confluence                                               |
| :star: Sliding Window Chunking  | Overlapping chunks.                                                                              | Most production RAG systems use overlap.                                   |
| Semantic Chunking               | Split where topic meaning changes. Uses embeddings to detect - semantic drift, topic boundaries  | Research papers, enterprise knowledge systems, long reports, legal content |
| Code / AST-Based Chunking       | Chunk based on functions, classes, modules, syntax trees (AST)                                   |                                                                            |
| Fixed-Size Chunking             | Split text every N characters/tokens.<br/>examples - 500 tokens per chunk<br/>- 50 token overlap |                                                                            |

# Real-world mapping
- Most strong RAG systems combine multiple methods

| Company/Product Type | Common Strategy       |
|----------------------|-----------------------|
| SaaS docs chatbot    | recursive + structure |
| Coding copilot       | AST chunking          |
| Enterprise search    | semantic + metadata   |
| PDF assistant        | recursive + semantic  |
| Legal AI             | sentence + semantic   |
| Meeting assistant    | sliding window        |




