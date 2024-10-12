# PEFT-for-Text-summarization

This repository demonstrates the parameter-efficient fine-tuning (PEFT) of language models for text summarization tasks using LoRA (Low-Rank Adaptation). We utilize T5 and Facebook's BART-large-cnn models, fine-tuning them on the SAMSum dataset for efficient and effective summarization, all within a single Jupyter Notebook.

## Learning Objectives

By the end of this experiment, you will be able to:
- Understand the workings of LoRA, a parameter-efficient fine-tuning method.
- Fine-tune T5 and Facebook's BART-large-cnn on the SAMSum dataset for summarization using LoRA.
- Push the fine-tuned LoRA adapter to the Hugging Face model hub.
- Load the fine-tuned adapter from the hub for inference.

## Dataset Description

The SAMSum dataset contains about 16,000 messenger-like conversations, each with summaries. These were created by English-fluent linguists to reflect real-life conversations and are annotated with summaries in the third person.

### Data Splits
- **Train**: 14,732 samples
- **Validation**: 818 samples
- **Test**: 819 samples

### Data Fields
- `dialogue`: Text of the dialogue.
- `summary`: Human-written summary of the dialogue.
- `id`: Unique ID of an example.

### Example
```json
{
  "id": "13818513",
  "summary": "Amanda baked cookies and will bring Jerry some tomorrow.",
  "dialogue": "Amanda: I baked cookies. Do you want some?\r\nJerry: Sure!\r\nAmanda: I'll bring you tomorrow :-)"
}
```


### Requirements
Ensure you have Python and the following packages installed:
- `transformers`
- `torch`
- `datasets`

