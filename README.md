# my-repo

Portfolio hub for my data science, statistics, machine learning and deep learning projects.
Each project lives in its own repository and is linked here as a git submodule under
`projects/<category>/`.

## Projects

| Category | Project | Repo | Status |
|---|---|---|---|
| Machine learning | Credit card transactions fraud detection | [repo](https://github.com/Pisit-Janthawee/ml-binaryclassification-credit-card-transactions-fraud-detection) | complete |

## Project layout

Every project uses the same structure:

```
<project>/
├── README.md            # problem, data source, approach, results, how to run
├── requirements.txt
├── notebooks/           # numbered, read top to bottom
│   ├── 01_data_understanding.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_preprocessing.ipynb
│   ├── 04_modeling.ipynb
│   ├── 05_evaluation_explainability.ipynb
│   └── 06_deployment.ipynb      (optional)
├── src/                 # reusable code imported by the notebooks
├── data/raw/            # git-ignored; download instructions in README
├── data/processed/      # git-ignored
├── models/              # git-ignored
└── reports/figures/     # plots used in the README
```

## Clone everything

```bash
git clone --recurse-submodules https://github.com/Pisit-Janthawee/my-repo.git
```
