# LangChain
- [LangChain](https://python.langchain.com/docs/introduction/) is a framework for building LLM-powered applications. 
- It helps you chain together interoperable components and third-party integrations to simplify AI application development — all while future-proofing decisions as the underlying technology evolves.

# System Diagram

                ┌─────────────┐
                │  User Input │
                └──────┬──────┘
                       │
                       ▼
                ┌─────────────┐
                │  Prompts    │
                │  (Templates)│
                └──────┬──────┘
                       │
                       ▼
                 ┌───────────────┐
                 │   LLM / Model │
                 │ (OpenAI, Gemini, etc.) │
                 └──────┬────────┘
                        │
           ┌────────────┼─────────────┐
           │            │             │
           ▼            ▼             ▼
  ┌─────────────┐ ┌─────────────┐ ┌───────────────┐
  │Chains/      │ │Agents       │ │Memory         │
  │Pipelines    │ │(Tool use)   │ │(Context)      │
  └─────┬───────┘ └─────┬───────┘ └──────┬────────┘
        │               │                │
        ▼               ▼                ▼
  ┌─────────────┐  ┌─────────────┐  ┌───────────────┐
  │ Multi-step  │  │ External    │  │ Session       │
  │ Workflows   │  │ Tools/APIs  │  │ Memory        │
  └─────────────┘  └─────────────┘  └───────────────┘
       │               │                │
       └───────────────┴────────────────┘
       │
       ▼
  ┌─────────────┐
  │  Output     │
  └─────────────┘

# Popular Use Cases
- Chained steps
- Dynamic tool use
- Context retention / memory
- Integration with external data