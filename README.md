# finetuningLLM

This repo contains 2 notebook
# 1) Fine_tuning_large_language_models.ipynb : 

Before executing any code, we need to make sure that we are running this notebook in Google Colab and that we have selected the T4 GPU runtime. 
This is important because fine-tuning large language models requires considerable compute and memory resources and the T4 GPU is a powerful processor that provides 16 GB VRAM. 
This is enough to fine-tune smaller models.

### Models used : Llama-2-7b-hf and Llama-2-7b-chat-hf.
We will use the library provided by Lamini for this purpose. This library can be used to conveniently load, prompt, and fine-tune large language models. Although we are loading and prompting the two variants of Llama 2 using this library, we will perform fine-tuning using the lower-level functions provided by the transformers library.

To initialise the llama library, we first need to make an account on Lamini and retrieve our API token from the Account page. Note that this is required only for exploring the outputs of the two versions of Llama and not for the actual fine-tuning code, so you may choose to skip this step. You can then add this as a secret in Google Colab and use the following code to initialise the API.


# 2) Fine_Tuning_LoRA_Code.ipynb : 
### PEFT for fine tuning
PEFT refers to a set of techniques that reduce the resources required in the fine-tuning process. The two main techniques that come under this umbrella are Low-Rank Adaptation (LoRA) and Quantized Low-Rank Adaptation (qLoRA).


