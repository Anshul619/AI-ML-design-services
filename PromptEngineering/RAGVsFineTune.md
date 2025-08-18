# RAG vs Fine Tune
- RAG is similar to [fine-tuning](../FoundationalModels/FineTuning.md).
- However, rather than having to fine-tune an FM with a small set of labeled examples, RAG retrieves a small set of relevant documents from a large corpus and uses that to provide context to answer the question.
- RAG will not change the weights of the [foundation model](../FoundationalModels/Readme.md) whereas fine-tuning will change model weights.