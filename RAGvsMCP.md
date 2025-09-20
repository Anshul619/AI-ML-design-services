# MCP vs RAG

| Aspect              | MCP (Model Context Protocol)                                 | RAG                                   |
|---------------------|--------------------------------------------------------------|---------------------------------------|
| Purpose             | Standardize/structure model input context                    | Retrieve external info for the model  |
| Scope               | Broader: includes memory, prompt, instructions, context flow | Narrower: fetching relevant knowledge |
| Context Engineering | Yes, formal protocol for organizing context                  | Yes, but only via retrieval           |
| Interaction         | Can manage multi-turn, dynamic context                       | Usually stateless retrieval per query |


# High level diagram

            ┌──────────────────┐
            │   User Query /   │
            │   Input Prompt   │
            └────────┬─────────┘
                     │
                     ▼
            ┌──────────────────┐
            │   MCP Layer      │
            │ (Context Manager)│
            │------------------│
            │ - Maintain       │
            │   conversation   │
            │ - Prioritize     │
            │   relevant info  │
            │ - Chunk context  │
            └────────┬─────────┘
                     │
                     ▼
            ┌──────────────────┐
            │   RAG Module     │
            │------------------│
            │ - Retrieve       │
            │   documents /    │
            │   knowledge      │
            │ - Rank relevance │
            └────────┬─────────┘
                     │
                     ▼
            ┌──────────────────┐
            │   Combined Input │
            │  (Context +      │
            │   Retrieved Data)│
            └────────┬─────────┘
                     │
                     ▼
            ┌──────────────────┐
            │   LLM / Model    │
            │------------------│
            │ - Generates      │
            │   response using │
            │   structured     │
            │   context        │
            └──────────────────┘
                     │
                     ▼
            ┌──────────────────┐
            │   User Response  │
            └──────────────────┘

# Summary
- RAG is like a component you could use within an MCP system, but MCP is broader - it defines how all context is structured, updated, and delivered to the model.