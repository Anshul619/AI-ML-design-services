# Inference parameters
- When interacting with foundational models, you can often configure inference parameters (settings) to limit or influence the model response.`
- Inference parameters fit into a range of categories, with the most common being randomness and diversity and length.

# Randomness and diversity
- Randomness and diversity parameters influence the variation in generated responses by limiting the outputs to more likely outcomes or by changing the shape of the probability distribution of outputs.

|             | Description                                                                                                                                                                                                      |
|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Temperature | This parameter controls the randomness or creativity of the model's output. A higher temperature makes the output more diverse and unpredictable, and a lower temperature makes it more focused and predictable. |
| Top p       | Top p is a setting that controls the diversity of the text by limiting the number of words that the model can choose from based on their probabilities.<br/>- Top p is also set on a scale from 0 to 1.          |
| Top k       | Top k limits the number of words to the top k most probable words, regardless of their percent probabilities.                                                                                                    |

# Length
- The length inference parameter category refers to the settings that control the maximum length of the generated output and specify the stop sequences that signal the end of the generation process.

|                | Description                                                                                                                                                                                                                                                                                 |
|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Maximal Length | The maximum length setting determines the maximum number of tokens that the model can generate during the inference process.<br/>- This parameter helps to prevent the model from generating excessive or infinite output, which could lead to resource exhaustion or undesirable behavior. |
| Stop sequence  | Stop sequences are special tokens or sequences of tokens that signal the model to stop generating further output. <br/>- When the model encounters a stop sequence during the inference process, it will terminate the generation regardless of the maximum length setting.                 |