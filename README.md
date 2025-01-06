# QLoRA Finetuning for LLM: Text Sentiment Classification

This repository demonstrates the use of **QLoRA** and **LoRA** as fine-tuning methods for Large Language Models (LLM) in the task of text sentiment classification.

## Results

### Llama-3.2-1B Model (Before Fine-tuning)
The Llama-3.2-1B model, which was initially trained for general text generation tasks, showed a sentiment classification accuracy of **18.5%** before fine-tuning.

![Before Fine-tuning](https://github.com/user-attachments/assets/72a1ee5b-56de-4cbf-8e25-6226df2d7edc)

### Llama-3.2-1B Model (After LoRA Fine-tuning)
After fine-tuning the Llama-3.2-1B model with **LoRA**, the accuracy increased to **83%**, demonstrating the effectiveness of LoRA for sentiment classification.

![After LoRA Fine-tuning](https://github.com/user-attachments/assets/25f3b391-7a3c-4c53-8619-773892582088)

## Additional Tests Conducted

1. **Hyperparameter Tuning for LoRA:**
   - Decomposition rank
   - Alpha coefficient

2. **Hyperparameter Tuning for QLoRA:**
   - Quantization type
   - Double quantization

3. **Dataset Size Impact:**
   - Testing the effect of training dataset size on model effectiveness.

4. **Epochs vs. Dataset Size:**
   - Comparing the performance of smaller datasets with more epochs versus larger datasets with fewer epochs.

5. **Generalization Abilities:**
   - Evaluating the model's ability to generalize by testing it on a different dataset (fien-tuned on tweets dataset and tested on financial dataset).
