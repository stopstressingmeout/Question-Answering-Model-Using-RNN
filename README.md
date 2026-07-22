# Question Answering Model Using RNN

This repository contains a simple question-answering prototype built with PyTorch using a recurrent neural network (RNN). The project uses a small CSV dataset of general knowledge question-answer pairs and demonstrates the end-to-end workflow in a Jupyter Notebook.

## Contents

- `question_answering_model.ipynb` - Jupyter notebook with data loading, preprocessing, vocabulary construction, dataset creation, model definition, training loop, and prediction examples.
- `gk_qna_dataset.csv` - General knowledge question-answer dataset used to train and evaluate the model.

## Project Overview

The notebook implements a minimal RNN-based model that:

1. Loads and inspects the question-answer dataset.
2. Tokenizes text and builds a vocabulary.
3. Converts questions and answers into numeric token indices.
4. Creates a PyTorch `Dataset` and `DataLoader`.
5. Defines a basic RNN model with an embedding layer and output prediction layer.
6. Trains the model on the dataset.
7. Evaluates the model with a few test questions.

## Requirements

- Python 3.8+ recommended
- `pandas`
- `torch`

## Setup

1. Create and activate a virtual environment (optional but recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install required packages:

```powershell
pip install pandas torch
```

## Usage

1. Open `question_answering_model.ipynb` in Jupyter Notebook or VS Code Notebook.
2. Run the notebook cells sequentially.
3. Inspect the training progress and prediction outputs.

## Notes

- The model architecture is intentionally simple and suited for educational purposes.
- The notebook currently predicts one token per question and uses a small dataset, so it is not production-ready.
- You can extend this work by adding sequence-to-sequence decoding, padding, attention, or larger datasets.

