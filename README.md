### Fine-tune a Llama-3.2-1B model for news summarization using Unsloth for faster, memory-efficient training.

This notebook demonstrates how to fine-tune a lightweight Large Language Model (LLM) for text summarization using the Unsloth library, which enables ultra-fast LoRA training and 4-bit quantization. We use the News Summary Dataset to train a model that generates concise summaries from news articles.
### Key Features:

# Uses Unsloth for 2x faster training and lower memory usage
Implements LoRA (Low-Rank Adaptation) for parameter-efficient fine-tuning
Supports 4-bit quantization via bitsandbytes
Cleaned text preprocessing pipeline
Ready for inference and export
Use Case: Automatically generate short, accurate summaries from long-form news articles.

## Technologies & Libraries Used
Library	Purpose
unsloth	Fast LoRA training with 4-bit support
transformers, peft, trl	Hugging Face ecosystem for LLM training
datasets	Efficient dataset handling
pandas, numpy	Data manipulation
contractions	Expand English contractions (e.g., "you're" → "you are")
re	Text cleaning and preprocessing
Dataset
### Source: News Summary Dataset by sunnysai12345

Structure
text: Full news article (input)
ctext: Human-written summary (target)
Note: The dataset uses ISO-8859-1 encoding, which is handled during loading.
