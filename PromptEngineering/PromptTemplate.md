# Prompt Template
- A [prompt template](https://docs.aws.amazon.com/bedrock/latest/userguide/prompt-engineering-guidelines.html) specifies the formatting of the prompt with exchangeable content in it. 
- Prompt templates are “recipes” for using LLMs for different use cases such as classification, summarization, question answering, and more.
- A prompt template may include instructions, few-shot examples, and specific context and questions appropriate for a given use case.

````
Prompt template: 
"""Tell me the sentiment of the following 
{{Text Type, e.g., “restaurant review”}} and categorize it 
as either {{Sentiment A}} or {{Sentiment B}}. 
Here are some examples:

Text: {{Example Input 1}} 
Answer: {{Sentiment A}}

Text: {{Example Input 2}}
Answer: {{Sentiment B}}

Text: {{Input}}
Answer:"""
````
