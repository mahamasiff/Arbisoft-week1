# MNIST Classification with SVM

Handwritten digit classification using Support Vector Machines on the MNIST dataset.

## Setup

Requires [uv](https://docs.astral.sh/uv/). Install dependencies:

    uv sync

## Project Structure

- `task1.ipynb` — main notebook: data loading, training, evaluation
- `test_data_prep.py` — pytest unit tests for data preparation

## Running the Notebook

Open `task1.ipynb` in Jupyter and run all cells. The pipeline:
1. Loads `mnist_784` via `fetch_openml`
2. Downsamples to 5,000 samples (SVM training optimization)
3. Splits 80/20 into train/test sets with stratification
4. Scales features with `StandardScaler`
5. Trains an RBF-kernel SVM (`SVC`)
6. Evaluates accuracy, precision, recall, and plots a confusion matrix

## Running Tests

    uv run pytest test_data_prep.py -v

7 unit tests covering downsampling, train/test split integrity, and scaler behavior.

## Linting

    uv run ruff check .
    uv run ruff format .
