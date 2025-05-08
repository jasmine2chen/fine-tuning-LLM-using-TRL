# Direct Preference Optimization with Hugging Face TRL

### Project Overview
This project demonstrates how to fine-tune open LLMs using Hugging Face TRL, Transformers & datasets to generate SQL queries based on a natural language instruction.

The goal is to reduce the time it takes to create a SQL query and make it easier for non-technical users to create SQL queries

### Key highlights

SFTTrainer from trl is used to fine-tune the model. The SFTTrainer makes it straightfoward to supervise fine-tune open LLMs. The SFTTrainer is a subclass of the Trainer from the transformers library and supports all the same features, including logging, evaluation, and checkpointing, but adds additiional quality of life features.

As peft method, QLoRA is used to reduce the memory footprint of large language models during finetuning, without sacrificing performance by using quantization

### Workflow
- Setup development environment
- Create and prepare the dataset
- Fine-tune LLM using trl and the SFTTrainer
- Test and evaluate the LLM
- Deploy the LLM for Production

### Model Used
meta-llama/Meta-Llama-3.1-8B


