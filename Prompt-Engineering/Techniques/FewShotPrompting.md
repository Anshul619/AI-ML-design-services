# Tips for few-shot prompting
- The labels in a few-shot prompt do not need to be correct to improve model performance.
    - Usually, applying random labels outperforms using no labels at all.
    - However, the label space and distribution of the input text specified by the demonstrations are important.
    - The use of the term label in this context refers to the output of the prompt examples.
    - The sentiment expressed by a statement in a ”prompt example“ is an example of a label.
- If you have access to a large set of examples, use techniques to obey the token limits of your model and dynamically populate prompt templates.
    - You can use an example selector that is based on semantic similarity to help.
    - To try out an example selector, refer to [Python Langchain Example Selectors](https://python.langchain.com/docs/how_to/example_selectors/).

# Example

````
Tell me the sentiment of the following headline and categorize it as either positive, negative, or neutral. Here are some examples:

Research firm fends off allegations of impropriety over new technology.
Answer: Negative

Offshore windfarms continue to thrive as vocal minority in opposition dwindles.
Answer: Positive


Manufacturing plant is the latest target in investigation by state officials.
Answer:

Output: Negative
````

Note: The **Amazon Titan Text model** was used in this example. For other models, please refer to the  'Model-Specific Prompt Techniques' lesson.