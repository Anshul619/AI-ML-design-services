# Foundational Models
- A foundational model is a large-scale, pre-trained AI model trained on broad and diverse data (e.g. text, images, code).

# Stages

| Stage              | Description                                                                                                                                                                                                                                       |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pre-training       | During the training stage, FMs use self-supervised learning or reinforcement learning from human feedback (RLHF), to capture data from vast datasets. (large amount of unlabeled data)                                                            |                                                                                      |
| Fine-tuning        | [Fine tuning](FineTuning.md) is a technique used to improve the performance of a pre-trained AI model on a specific task.                                                                                                                         |                                                                                      |
| Prompt Engineering | [Prompt engineering](../Prompt-Engineering/Readme.md) is a more efficient and faster way to tune LLM responses (with guidance, practices, parameter settings), as opposed to fine-tuning, which requires labeled data and training infrastructure. |

# Types of FMs

|                      | Description                                                                                                                             |
|----------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Text-to-text models  | Text-to-text models are large language models (LLMs) that are pretrained to process vast quantities of textual data and human language. |
| Text-to-image models | Text-to-image models take natural language input and produce a high-quality image that matches the input text description.              |

# Unlabeled data
- Unlabeled data can be used at scale for pretraining because it is a lot easier to obtain compared to labeled data. 
- The latter requires a human task force to create laborious annotations, such as explicitly adding the tag dog to an image that contains one. 
- During the pretraining process, the model automatically takes context into account from all this training data.
- It then tracks the relationships in sequential data, such as the position and the context of the words so that it can predict the next word in a sentence.