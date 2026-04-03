# Task 4: BERT Fine-Tuning for Text Classification
## Objective

To fine-tune a pre-trained BERT model for sentiment analysis and evaluate its performance using different training strategies.

## Description

This project involves building a text classification model using BERT on the IMDB dataset. The model processes text data through tokenization and learns contextual representations. Multiple experiments are conducted by freezing and unfreezing layers to compare performance.

## Technologies Used
- Python
- Hugging Face Transformers
- PyTorch
- Scikit-learn
- Matplotlib & Seaborn

## How to Run
### Install dependencies:
- pip install transformers torch sklearn matplotlib seaborn
- Open the notebook and run all cells.

## Experiments
- Frozen BERT (only classifier trained)
- Fine-tuning last 2 layers
  
## Evaluation
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve

## Conclusion

This project shows that fine-tuning BERT improves performance in text classification tasks. Allowing more layers to train helps the model capture deeper contextual information, leading to better results.
