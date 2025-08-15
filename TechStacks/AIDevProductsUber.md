# AI Dev Products @ Uber
- Using [LangGraph](../AgentsDev/LangGraph.md)

# Products

| Product   | Description      |
|-----------|------------------|
| Validator | review the code  |
| AutoCover | tests generation |

# Design Principles

| Principle              | Description                                                                                                                                                                              |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Specialized = Smarter  | Purpose-built agents outperform generation foundation models<br/>- Better Context retention<br/>- Less ambiguity<br/>- Fewer hallucinations                                              |
| Simple, reliable nodes | Bounded responsibilities + Deterministic nodes improve reliability<br/>- Deterministic tools (e.g. linters) ensure consistency<br/>- Clear boundaries simplify development and debugging |
| Fast & Scalable dev    | Reusable agents nodes accelerate development<br/>- Solved scoped problems and reuse across graphs<br/>- Faster composition of new flows<br/>- Reuse nodes, iterate faster                |

# Read more
- [How Uber Built AI Agents That Save 21,000 Developer Hours with LangGraph | LangChain Interrupt](https://www.youtube.com/watch?v=Bugs0dVcNI8)