# ReAct Prompting
- With ReAct prompting, an LLM can combine reasoning and action.
- With a ReAct framework, LLMs can generate both reasoning traces and task-specific actions that are based on external tools, such as Wikipedia pages or SQL databases. 
- This external context leads to more accurate and reliable output.

# Example prompt and output providing the LLM with a calculator tool

````
Prompt:
What is 3.14 raised to the power of 0.12345? 

Output (Anthropic Claude v1 without calculator) - wrong answer:
3.14^(0.12345) = 2.8337112781979765
So the answer is: 2.8337112781979765

Output (Anthropic Claude v1 with calculator) - right answer:

Entering new AgentExecutor chain...
I will need to use the calculator for this.
Action: Calculator
Action Input: 3.14^0.12345
Observation: Answer: 1.1517174978619817
Thought: I have the final answer.
Final Answer: 1.1517174978619817
> Finished chain.
````

