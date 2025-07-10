# Comparative Study on Hate Speech Detection

This repository contains all the Jupyter notebooks for our accepted IEEE IMSA 2025 paper:

> **Balancing Efficiency and Accuracy: A Comparative Analysis of LSTM and RoBERTa for Explainable Hate Speech Detection on HateXplain**  
> *Amr Khaled, Ahmed Mounir, John Medhat, Wael Hassan*  
> Accepted to appear in IEEE International Conference on Intelligent Methods, Systems, and Applications (IMSA), August 2025.

## Notebooks

| Notebook                                       | Description                                                                                          |
|-----------------------------------------------|------------------------------------------------------------------------------------------------------|
| `Hate_Speech_Detection_LSTM.ipynb`            | Build, train and evaluate the LSTM-based classifier (macro-F1 = 0.85).                                |
| `Hate_Speech_Detection_RoBERTa.ipynb`         | Fine-tune and test the RoBERTa model (macro-F1 = 0.9211).                                             |
| `Hate_Speech_Detection_DistilBERT.ipynb`      | Run experiments with DistilBERT as a lightweight transformer baseline.                                |
| `Hate_Speech_Detection_QLoRA_Qwen.ipynb`      | Apply QLoRA fine-tuning to Qwen for low-resource LLM adaptation.                                      |

## Getting Started

1. Clone the repo:  
   ```bash
   git clone https://github.com/YourUsername/hate-speech-comparative.git
   cd hate-speech-comparative
