# Tips for Zero-shot prompting
- The larger the LLM, the more likely the zero-shot prompt will yield effective results.
- Instruction tuning can improve improve zero-shot learning. You can adopt reinforcement learning from human feedback (RLHF) to scale instruction tuning, aligning modern LLMs to better fit human preferences.

# Example

````
Tell me the sentiment of the following social media post and categorize it as positive, negative, or neutral:
Don't miss the electric vehicle revolution! AnyCompany is ditching muscle cars for EVs, creating a huge opportunity for investors.

Output - Positive
````

Note: This prompt did not provide any examples to the model. However, the model was still effective in deciphering the task.