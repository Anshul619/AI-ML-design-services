# Foundational Models
- A foundational model is a large-scale, pre-trained AI model trained on broad and diverse data (e.g. text, images, code).

![](https://render.skillbuilder.aws/cds/2be77fc1-127a-4069-8107-c773f69ae789/assets/illustration_foundationModel_v4.png)

# Stages

| Stage              | Description                                                                                                                                                                                                                                       |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pre-training       | During the training stage, FMs use self-supervised learning or reinforcement learning from human feedback (RLHF), to capture data from vast datasets.                                                                                             |                                                                                      |
| Fine-tuning        | [Fine tuning](FineTuning.md) is a technique used to improve the performance of a pre-trained AI model on a specific task.                                                                                                                         |                                                                                      |
| Prompt Engineering | [Prompt engineering](../PromptEngineering/Readme.md) is a more efficient and faster way to tune LLM responses (with guidance, practices, parameter settings), as opposed to fine-tuning, which requires labeled data and training infrastructure. |

# Types of FMs

|                      | Description                                                                                                                             |
|----------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Text-to-text models  | Text-to-text models are large language models (LLMs) that are pretrained to process vast quantities of textual data and human language. |
| Text-to-image models | Text-to-image models take natural language input and produce a high-quality image that matches the input text description.              |