# Fake News Classification with an LSTM

A natural-language classification notebook that preprocesses news text, builds token sequences, and trains an LSTM network for binary fake-news classification.

## Workflow

- Clean and normalize text with regular expressions
- Remove stopwords and apply Porter stemming
- Convert text to one-hot token representations
- Pad sequences to a fixed length
- Train an embedding and LSTM classifier
- Evaluate training and validation accuracy
- Save and reload the trained Keras model

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -c "import nltk; nltk.download('stopwords')"
jupyter notebook FakeNewsClassifierUsingLSTM.ipynb
```

The dataset must be obtained separately and its source and license documented before reproducing the notebook.

## Evaluation notes

The notebook records peak validation accuracy around 92%, followed by a growing train/validation gap that suggests overfitting. A stronger evaluation should use source-aware or time-aware splitting, compare TF-IDF and transformer baselines, and report precision, recall, F1, ROC-AUC, and calibration.

## Responsible use

A text classifier cannot independently establish whether a claim is true. Real fact-checking requires source evidence, provenance, human review, and safeguards against domain shift.

## Author

**Purnendu Kale** · [LinkedIn](https://www.linkedin.com/in/purnendukale/)
