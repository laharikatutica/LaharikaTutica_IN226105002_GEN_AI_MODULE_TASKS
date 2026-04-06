# POS Tagging & Chunking using BERT – NLP Assignment 5

## Important Note:
### If the GitHub preview shows **"Invalid Notebook"** or does not display outputs, please open the notebook using the **Google Colab link below**.

All outputs, results and comparisons can be viewed using the following Google Colab link.

### Google Colab link: https://colab.research.google.com/drive/1w_eR07K5rJPOGMznYTeKJieWX6VDX0I4#scrollTo=PT7mwVm4a3s_

## Objective
- Fine-tune BERT for POS tagging (token classification).  
- Handle tokenization & label alignment.  
- Evaluate performance using precision, recall, F1, accuracy.  
- Understand Chunking conceptually.

## Technologies
- Python, PyTorch  
- Hugging Face Transformers  
- SeqEval (metric)

## Dataset
- Universal Dependencies (POS tagging)  
- Sample labels: NOUN, VERB, ADJ, ADV, PRON, DET, ADP, PROPN, PUNCT

## Pipeline
Raw Data → Tokenization → Label Alignment → Model Setup → Training → Evaluation → Inference

## Implementation
1. **Data Loading:** Parsed `.conllu` files; extracted tokens & POS tags.  
2. **Preprocessing:** Limited dataset for quick experiments; created `label2id` & `id2label`.  
3. **Tokenization:** `bert-base-uncased` tokenizer; applied padding, truncation, attention masks.  
4. **Label Alignment:** Handled subword tokens; assigned -100 to special tokens.  
5. **Model Setup:** Loaded BERT via `AutoModelForTokenClassification` with correct number of labels.  
6. **Training:** Trainer API, learning rate 2e-5, epochs 3, batch size 16, weight decay 0.01.  
7. **Evaluation:** Precision, recall, F1, accuracy (SeqEval).  
8. **Inference:** Tested custom sentences, generated POS tags.

## Conclusion
BERT fine-tuning for POS tagging shows strong performance, learning contextual dependencies between words. Proper preprocessing, especially token-label alignment, is key for accurate sequence labeling.  
