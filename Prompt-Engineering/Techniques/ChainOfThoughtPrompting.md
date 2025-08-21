# Chain-of-thought prompting
- Chain-of-thought (CoT) prompting breaks down complex reasoning tasks through intermediary reasoning steps. You can use both zero-shot and few-shot prompting techniques with CoT prompts.
- Chain-of-thought prompts are specific to a problem type. You can use the phrase "Think step by step" to invoke CoT reasoning from your machine learning model.

# Example

````
Which vehicle requires a larger down payment based on the following information?

The total cost of vehicle A is $40,000, and it requires a 30 percent down payment.

The total cost of vehicle B is $50,000, and it requires a 20 percent down payment.
(Think step by step)
````

## Output

````
The down payment for vehicle
A is 30 percent of $40,000, which is
(30/100) * 40,000 = $12,000.

The down payment for vehicle
B is 20 percent of $50,000, which is
(20/100) * 50,000 = $10,000.

We can see that vehicle A needs a larger down payment than vehicle B.
````

Note: This prompt did not provide any examples to the model. However, the model was still effective in deciphering the task.

# CoT few-shot prompt
- This prompt provided both few-shot context in the form of a question-and-answer example and CoT prompting by asking the model to "Think step by step."

````
In a given week, the viewers for a TV channel are as follows:
Monday: 6,500 viewers
Tuesday: 6,400 viewers
Wednesday: 6,300 viewers

Question: How many viewers can we expect on Friday?
Answer: Based on the numbers given and without any more information, there is a daily decrease of 100 viewers. If we assume this trend will continue during the following days, we can expect 6,200 viewers on the next day that would be Thursday, and therefore 6,100 viewers on the next day that would be Friday.

Question: How many viewers can we expect on Saturday? (Think step by step)
Answer:
````

