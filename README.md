# Comparative Study on Hate Speech Detection

This repository contains all the code and Jupyter notebooks for our accepted IEEE IMSA 2025 paper:

> **Balancing Efficiency and Accuracy: A Comparative Analysis of LSTM and RoBERTa for Explainable Hate Speech Detection on HateXplain**  
> *Amr Khaled, Ahmed Mounir, John Medhat, Wael Hassan*  
> Accepted to appear in IEEE International Conference on Intelligent Methods, Systems, and Applications (IMSA), August 2025.

We compare four different NLP architectures—LSTM, RoBERTa, DistilBERT, and Qwen fine-tuned via QLoRA—on the HateXplain dataset. Our experiments evaluate each model’s classification performance (accuracy, precision, recall, macro-F1) as well as computational efficiency and inference throughput.

---

## 📁 Repository Structure

```
hate-speech-comparative/
├── Hate_Speech_Detection_LSTM.ipynb
├── Hate_Speech_Detection_RoBERTa.ipynb
├── Hate_Speech_Detection_DistilBERT.ipynb
├── Hate_Speech_Detection_QLoRA_Qwen.ipynb
├── requirements.txt
└── README.md
```

- **Hate_Speech_Detection_LSTM.ipynb**  
  Builds, trains, and evaluates a bidirectional LSTM classifier (3.5 M parameters, macro-F1 ≈ 0.85).

- **Hate_Speech_Detection_RoBERTa.ipynb**  
  Fine-tunes `roberta-base` for hate speech detection (125 M parameters, macro-F1 ≈ 0.9211).

- **Hate_Speech_Detection_DistilBERT.ipynb**  
  Experiments with `distilbert-base` as a lightweight transformer baseline.

- **Hate_Speech_Detection_QLoRA_Qwen.ipynb**  
  Applies QLoRA low-rank adaptation to the Qwen large-language model.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YourUsername/hate-speech-comparative.git
cd hate-speech-comparative
```

### 2. Create a virtual environment (recommended)

```bash
python3 -m venv venv
source venv/bin/activate        # Linux / macOS
venv\Scripts\activate           # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

> **Note:** The `requirements.txt` includes  
> - `transformers`  
> - `torch` or `tensorflow` (depending on which notebook)  
> - `datasets`  
> - `scikit-learn`  
> - `pandas`, `numpy`, `matplotlib`  
> - etc.

### 4. Launch Jupyter

```bash
jupyter notebook
```

Open any notebook and run all cells to reproduce the experiments.

---

## 📊 Results Summary

| Model             | Parameters | Macro-F1 | Throughput (samples/s) |
|-------------------|------------|----------|------------------------|
| LSTM              | 3.5 M      | 0.85     | 150                    |
| RoBERTa (base)    | 125 M      | 0.9211   | 60                     |
| DistilBERT        | 66 M       | ~0.90    | ~100                   |
| Qwen + QLoRA      | 7 B        | ~0.93    | ~30                    |

*(Exact numbers are detailed in each notebook.)*

---

Thank you for exploring our work! Contributions, issues, and feature requests are welcome.
