# MCP
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) is an open standard—like a universal interface—that enables [large language models (LLMs)](../Foundational-Models/LLM.md) to access tools, data, or external services through a standardized protocol. 
- It solves the problem of having to build bespoke integrations for each LLM-tool pair, simplifying the “N×M” integration challenge and supports [various transport types]().

![](https://mintcdn.com/mcp/4ZXF1PrDkEaJvXpn/images/mcp-simple-diagram.png?w=1100&fit=max&auto=format&n=4ZXF1PrDkEaJvXpn&q=85&s=0a319cb6a2504659377de862e889b8da)

# Transport types

|                            | Remarks        |
|----------------------------|----------------|
| stdio (local stdin/stdout) |                |
| SSE (server-sent events)   | using JSON-RPC |
| HTTP, WebSocket            | using JSON-RPC |

# Example Use Cases
- Agents can access your Google Calendar and Notion, acting as a more personalized AI assistant.
- Claude Code can generate an entire web app using a Figma design.
- Enterprise chatbots can connect to multiple databases across an organization, empowering users to analyze data using chat.
- AI models can create 3D designs on Blender and print them out using a 3D printer.

# References
- [Supercharging AWS database development with AWS MCP servers](../AWS-Services/AWSMCP.md)
- [OpenAI adds MCP support to ChatGPT](https://www.reddit.com/r/singularity/comments/1l3bwdi/openai_adds_mcp_support_to_chatgpt/)