# Text Generation with GPT-2 and LSTM  
A Python-based project showcasing two approaches to text generation:  

- **GPT-2 (Transformer-based)**: Delivers high-quality, context-aware text generation.  
- **LSTM (RNN-based)**: Provides simpler, sequential text prediction.  

## Project Details  
- **Company:** CODETECH IT SOLUTIONS  
- **Intern Name:** Aalay Kabariya 
- **Intern ID:** C0DF49  
- **Domain:** Artificial Intelligence  
- **Duration:** 4 Weeks  
- **Mentor:** Neela Santosh  

## Features  
### GPT-2 Implementation  
- Uses pre-trained **GPT-2** model from Hugging Face Transformers.  
- Generates text with configurable sampling (`top_k`, `temperature`).  

### LSTM Implementation  
- Trains a custom **LSTM model** on a small corpus.  
- Predicts next words using token sequences.  

### User-Friendly Enhancements  
- Includes example prompts (e.g., _"The importance of biodiversity"_).  
- Handles **GPU/CPU compatibility**, disabling GPU if unavailable.  

## Technologies Used  
- **Python** – Core programming language  
- **PyTorch** – Model loading/inference for GPT-2  
- **TensorFlow/Keras** – LSTM model implementation  
- **Hugging Face Transformers** – GPT-2 tokenizer & model  
- **NLTK/Tokenizer** – Text preprocessing for LSTM  

## How It Works  
### GPT-2  
1. **Model Load:** Uses `GPT2LMHeadModel` and `GPT2Tokenizer`.  
2. **Text Generation:**  
   - Encodes input prompt.  
   - Generates text via `model.generate()` with diverse sampling techniques.  

### LSTM  
1. **Data Preparation:**  
   - Tokenizes corpus and constructs n-gram sequences.  
2. **Model Architecture:**  
   - Embedding → LSTM → Dense layers.  
   - Predicts next word probabilities.  
3. **Inference:**  
   - Takes seed text → Processes → Predicts next words iteratively.  

## Installation  
```bash
git clone https://github.com/yourusername/text-generation.git
cd text-generation
pip install -r requirements.txt
