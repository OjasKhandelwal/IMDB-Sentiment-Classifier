 # IMDB Sentiment Classifier with BERT
 
A fine-tuned BERT-based sentiment classifier built on the IMDB movie review dataset. Classifies reviews as **Positive** or **Negative** using Hugging Face Transformers and features an interactive Gradio UI — all in ~80 lines of core training code.
 
---
 
## Features
 
- Fine-tuned `bert-base-uncased` with a classification head
- Handles tokenization, training loop, eval, mixed precision and checkpointing via Hugging Face `Trainer`
- Evaluated on accuracy and F1 score
- Inference on custom review text
- Interactive Gradio UI for live predictions
- Model saving and reloading support
---
 
## Project Steps
 
| # | Step | Description |
|---|------|-------------|
| 1 | **Setup** | Install libraries and configure environment |
| 2 | **Load Dataset** | Load the IMDB dataset from Hugging Face `datasets` |
| 3 | **Explore Data** | Examine sample reviews and label distribution |
| 4 | **Split Data** | Split into train, validation, and test sets |
| 5 | **Tokenize** | Tokenize reviews using the BERT tokenizer |
| 6 | **Load Model** | Load pre-trained `bert-base-uncased` with a classification head |
| 7 | **Fine-tune** | Fine-tune using Hugging Face `Trainer` |
| 8 | **Evaluate** | Evaluate on the test set (accuracy + F1) |
| 9 | **Predict** | Run inference on new, unseen reviews |
| 10 | **Save** | Save the trained model to disk |
| 11 | **Gradio UI** | Launch an interactive web UI for real-time predictions |
 
---


## Model Details
 
| Property | Value |
|----------|-------|
| Base Model | `bert-base-uncased` |
| Task | Binary Sentiment Classification |
| Dataset | IMDB (Hugging Face) |
| Labels | `POSITIVE`, `NEGATIVE` |
| Optimizer | AdamW (via Trainer defaults) |
| Metrics | Accuracy, F1 |
 
---


 ## Gradio UI Preview
 
After training, the model is reloaded and served through a Gradio interface where you can type any movie review and get an instant sentiment prediction.


## License
 
This project is licensed under the [MIT License](LICENSE).
