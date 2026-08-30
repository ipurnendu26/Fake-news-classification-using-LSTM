# Fake-News Text Classification with an LSTM

A Jupyter notebook exploring sequence-based binary text classification with tokenization, padded sequences, embeddings, and an LSTM network.

## Project file

- `FakeNewsClassifierUsingLSTM.ipynb`: preprocessing, model training, and evaluation

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

The source dataset is not committed; configure the notebook with a properly licensed local copy.

## Skills demonstrated

- Text normalization and vocabulary construction
- Sequence padding
- Embedding and recurrent neural-network layers
- Binary classification evaluation

## Limitations and responsible use

“Fake news” is context-dependent and cannot be reliably determined from wording alone. This notebook is a modeling exercise, not a fact-checking system. A defensible study needs clear label provenance, source/time-aware splits, duplicate detection, strong TF-IDF baselines, calibration, subgroup and publisher analysis, drift monitoring, citations, and human review. Do not use this model to censor, rank, or make decisions about people or publishers.

## License

Code is available under the [MIT License](LICENSE). Dataset rights remain with its original publisher.
