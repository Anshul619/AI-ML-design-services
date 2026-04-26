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
- Every function call is a tool call
- But not every tool call is just a simple function
