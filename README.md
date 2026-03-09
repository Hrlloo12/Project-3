# Instruction Following with Dolly-15k

This project evaluates instruction-following performance using the Dolly-15k dataset by comparing three approaches: zero-shot prompting, few-shot prompting, and fine-tuning.

##  Objective
The goal of this project is to understand how different prompting strategies affect instruction-following quality under limited data and compute resources.

##  Dataset
We used the Dolly-15k dataset, which contains around 15,000 instruction-response pairs across multiple task categories such as question answering, classification, summarization, and brainstorming.

##  Methods

### Zero-shot
We designed structured prompts using only the instruction (and context when available).

### Few-shot
We added example instruction-response pairs to guide the model.

### Fine-tuning
We fine-tuned a small open-source model (TinyLlama-1.1B) using LoRA on a small subset of the dataset.

## 📊 Results

Zero-shot achieved the best performance in this project. It scored 21.4 in BLEU and achieved an average LLM judge score of 9.6.

Few-shot showed slightly lower performance, with a BLEU score of 12.0 and an average judge score of 9.3.

Fine-tuning performed the weakest, achieving a BLEU score of 5.1 and an average judge score of 3.75 due to limited training data and compute.

##  Conclusion

Overall, zero-shot performed best in this setup. The results show that prompt-based approaches can outperform fine-tuning when resources are limited. Using both BLEU and LLM judge helped provide a more reliable evaluation.



👩‍💻  Hala Alotaibi
