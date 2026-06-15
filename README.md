# Project Title: UDACITY - Data Science Pipelines

This repository demonstrates building reproducible data science pipelines for text-based classification tasks. The included Jupyter notebook (`starter/starter.ipynb`) walks through data loading, preprocessing, feature engineering (TF-IDF + text features), model training and tuning, evaluation (accuracy, AUC, confusion matrix), and saving reusable pipelines to the `models/` folder.

**This project is completly done in a Jupyter notebook (`starter/starter.ipynb`) to show the project fullfillment.**
**Next steps would include to refactor the code and create dedicated `*.py`-files.**   

## Getting Started

Follow these steps to reproduce the notebook results locally.

### Quick Steps
- Create and activate a virtual environment
- Install the required Python packages
- Download the spaCy English model `en_core_web_sm`
- Open and run cells in `starter/starter.ipynb` in order

### Dependencies

Key external libraries used (examples — see `PROJECT_requirements.txt` for full list):

- python>=3.13
- pandas>=3.0.3
- joblib>=1.5.3
- numpy>=2.4.6
- scipy>=1.17.1
- scikit-learn>=1.9.0
- matplotlib>=3.11.0
- seaborn>=0.13.2
- wordcloud>=1.9.6

- spacy>=3.8.14 (plus `en_core_web_sm` model)


Install with:

```
python -m pip install -r PROJECT_requirements.txt
python -m pip install /path/to/en_core_web_sm-3.8.0-py3-none-any.whl
```

### Installation

1. Create and activate a virtual environment (PowerShell example):

```
python -m venv .venv
. .\.venv\Scripts\Activate.ps1
```

2. Install dependencies:

```
pip install -r PROJECT_requirements.txt
```

3. If encountering problems with spaCy, install the spaCy model used in the notebook:

```
pip install --trusted-host github.com --trusted-host objects.githubusercontent.com "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.8.0/en_core_web_sm-3.8.0-py3-none-any.whl"
```

4. Start Jupyter Lab/Notebook and open `starter/starter.ipynb`.

## Testing

- Run the `starter/starter.ipynb` notebook cells sequentially.
- Confirm that the `models/` directory contains saved pipeline files (joblib) after training cells complete.

### Break Down Tests

- Data loading cells: validate that `data/reviews.csv` loads with expected columns.
- Preprocessing cells: tokenization, stopword removal and TF-IDF generation produce expected shapes.
- Training cells: grid search / cross-validation report metrics and save the best pipeline.

## Project Instructions

Deliverables and checkpoints in the notebook:

- Data exploration and summary statistics
- Text preprocessing and feature extraction
- Baseline models and tuning (e.g., Logistic Regression, RandomForest, GradientBoosting)
- Evaluation: accuracy, AUC, confusion matrix, and visualizations
- Exporting and versioning trained pipelines in `models/`

Refer to the notebook sections (markdown headings) for step-by-step tasks.

## Built With key packages used (recommended versions are listed in `PROJECT_requirements.txt`):

- [Python](https://www.python.org/) - runtime (see `python>=3.13` in dependencies)
- [numpy](https://numpy.org/) - numerical computing
- [scipy](https://www.scipy.org/) - scientific computing
- [joblib](https://joblib.readthedocs.io/) - pipeline serialization and caching
- [wordcloud](https://github.com/amueller/word_cloud) - word cloud visualizations
- [seaborn](https://seaborn.pydata.org/) - statistical visualizations
- [matplotlib](https://matplotlib.org/) - plotting library

## License

[License](LICENSE.txt)
