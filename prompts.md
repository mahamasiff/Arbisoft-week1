# Prompting Log 

## Environment Setup
* **Prompt:** "Initialize a uv project with numpy, pandas, scikit-learn, pytest, and ruff."
* **Model:** Claude Code 
* **Outcome:** The agent successfully initialized the `.venv` virtual environment, and generated the `pyproject.toml` file locking in the core and development dependencies.

## Loading Dataset
* **Prompt:** "Write a python script in the next cell that loads the 'mnist_784' dataset directly using fetch_openml and downsamples it to 5,000 samples to optimize SVM training speed and splits it 80/20, and scales the features using StandardScaler."
* **Model:** Claude Code 
* **Outcome:** successfully produced an 80/20 split with training shape `(4000, 784)` and testing shape `(1000, 784)`

## Notebook Documentation & Refinement
* **Prompt:** "Please add markdown cells with short descriptions of each cell just to give an idea of what it's doing."
* **Model:** Claude Code 
* **Outcome:** The agent successfully documented the entire Jupyter Notebook, adding clear markdown headers and context descriptions above each code block. This ensures the experiment is self-documenting and easy for reviewers to follow.

