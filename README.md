# Direct Preference Optimization with Hugging Face TRL

### Project Overview
This project demonstrates how to fine-tune open LLMs using Hugging Face TRL, Transformers & datasets. 

The goal is to generate SQL queries based on a natural language instruction, that reduces the time it takes to create a SQL query and make it easier for non-technical users to create SQL queries
 
### Why SFT Before DPO?
Research shows DPO performs best when applied after Supervised Fine-Tuning (SFT):

- SFT teaches task fundamentals (e.g., generating coherent responses).

- DPO refines outputs using preference data (e.g., chosen vs. rejected responses).

- Skipping SFT leads to unstable training and poor convergence.

### Workflow
- Setup development environment
- Create and prepare the dataset
- Fine-tune LLM using trl and the SFTTrainer
- Test and evaluate the LLM
- Deploy the LLM for Production

### Model Used
meta-llama/Meta-Llama-3.1-8B


