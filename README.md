# QLoRA_finetuning_LLM
Testing QLoRA and LoRA as a finetuning method of LLM for task of classifying text sentiment

_Results:_
Llama-3.2-1B model (for general text generation tasks) before finetuning:
**Accuracy: 18.5%**
![image](https://github.com/user-attachments/assets/72a1ee5b-56de-4cbf-8e25-6226df2d7edc)

Llama-3.2-1B model after LoRA finetuning:
**Accuracy: 83%**
![image](https://github.com/user-attachments/assets/25f3b391-7a3c-4c53-8619-773892582088)

Additionall tests that were carried out:
* tuning of hyperparameters for LoRA (decomposition rank, alpha coefficient)
* tuning of hyperparameters for QLoRA (quantization type, double quantization)
* testing the impact of training dataset size on model effectiveness
* testing whether it is better to use smaller data but more epochs or bigger data and less epochs
* testing generalisation abilities of trained model on one dataset - testing model accuracy on a different dataset
