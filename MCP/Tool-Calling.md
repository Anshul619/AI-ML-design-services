# Tool Calling
- [Tool calling](https://www.ibm.com/think/topics/tool-calling) refers to the ability of artificial intelligence (AI) models to interact with external tools, application programming interfaces (APIs) or systems to enhance their functions.
- Instead of relying solely on pretrained knowledge, an AI system with tool-calling capabilities can query databases, fetch real-time information, execute functions or perform complex operations beyond its native capabilities.
- Tool calling, sometimes referred to as function calling, is a key enabler of [agentic AI](../Agent-Engineering/Readme.md). It allows autonomous systems to complete complex tasks by dynamically accessing and acting upon external resources.
- Instead of just answering questions, [large language models (LLMs)](../Foundational-Models/LLM.md) with tool calling can automate workflows, interact with databases, perform multistep problem-solving, make real-time decisions and more.
- This shift is turning LLMs from passive assistants into proactive digital agents capable of carrying out complex tasks.

# Function vs Tool Calling

| Aspect            | Function Calling                                        | Tool Calling                                             |
| ----------------- | ------------------------------------------------------- | -------------------------------------------------------- |
| **Definition**    | Calling a predefined function with structured arguments | Calling any external capability (functions, APIs, tools) |
| **Level**         | Low-level API feature                                   | Higher-level abstraction                                 |
| **Scope**         | Usually limited to functions you define                 | Can include APIs, DB queries, search, code execution     |
| **Output Format** | Structured JSON (name + arguments)                      | Same, but may include richer tool metadata               |
| **Flexibility**   | Narrow                                                  | Broad                                                    |
| **Modern Usage**  | Older terminology                                       | Preferred term in newer systems                          |

# Relationship
- Every function call is a tool call.
- But not every tool call is just a simple function.