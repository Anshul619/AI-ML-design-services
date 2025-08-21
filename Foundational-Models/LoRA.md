# LoRA
- [LoRA: Low-Rank Adaptation of Large Language Models](https://huggingface.co/blog/lora) is a novel technique introduced by Microsoft researchers to deal with the problem of fine-tuning large-language models.
- Powerful models with billions of parameters, such as [GPT-3](https://openai.com/index/gpt-3-apps/), are prohibitively expensive to fine-tune in order to adapt them to particular tasks or domains. 
- LoRA proposes to freeze pre-trained model weights and inject trainable layers (rank-decomposition matrices) in each transformer block. 
- [Read more](https://huggingface.co/blog/lora)

![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/blog/lora-assets/latent-diffusion.png)