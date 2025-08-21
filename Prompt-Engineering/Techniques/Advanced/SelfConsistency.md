# Self-consistency
- Self-consistency is a prompting technique that is similar to chain-of-thought prompting. 
- However, instead of taking the obvious step-by-step, or greedy path, self-consistency prompts the model to sample a variety of reasoning paths. 
- Then, the model aggregates the final answer based on multiple data points from the various paths.

````
Q. Terry had 12 apples. He gave half to Jane. John gave Terry three more apples. How many apples does Terry have?
A. Terry originally had 12 apples. He gave half to Jane, which means he gave 6 away. So now, Terry has 12 - 6 = 6 apples. John gave Terry three more apples, which means 3 + 6, so Terry now has 9 apples.

Q. When I was 10, my sister was half my age. Now I’m 40 years old. How old is my sister?
A.
```