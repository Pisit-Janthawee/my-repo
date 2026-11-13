# my-repo

Portfolio hub for my data science, statistics, machine learning and deep learning projects.
Each project lives in its own repository and is linked here as a git submodule under
`projects/<category>/`.

## Projects

| Category | Project | Repo |
|---|---|---|
| Deep learning | Melanoma classification, EfficientNetB0 + LIME | [repo](https://github.com/Pisit-Janthawee/dl-binaryclassification-siim-isic-melanoma-cnn-lime) |
| Deep learning | Tuberculosis chest X-ray classification, CNN + LIME | [repo](https://github.com/Pisit-Janthawee/dl-binaryclassification-tuberculosis-chest-xray-cnn-lime) |
| Deep learning | Stock triple-barrier classification (RNN / LSTM / GRU) | [repo](https://github.com/Pisit-Janthawee/dl-multiclassification-stock-triple-barrier-rnn-lstm) |
| Machine learning | Credit card transactions fraud detection | [repo](https://github.com/Pisit-Janthawee/ml-binaryclassification-credit-card-transactions-fraud-detection) |
| Machine learning | Everything about ensemble learning (Titanic) | [repo](https://github.com/Pisit-Janthawee/ml-binaryclassification-titanic-ensemble-learning.) |
| Machine learning | House prices, linear regression | [repo](https://github.com/Pisit-Janthawee/ml-regression-house-prices-linear-regression) |
| Machine learning | Chicago crime 2022: exploration, forecasting and classification | [repo](https://github.com/Pisit-Janthawee/ml-classification-chicago-crime-2022) |
| Machine learning | Steam game recommendation system, clustering and thumbnail GAN | [repo](https://github.com/Pisit-Janthawee/ml-recommendationsystem-clustering-steam-games) |

## Project layout

Each project is built to run on Kaggle and to be read top to bottom:

```
<project>/
├── README.md        # overview, results, how to run on Kaggle, findings
├── <project>.ipynb  # one self-contained notebook: settings cell on top, numbered [k/N] sections
├── assets/          # figures used in the README
└── arch/            # earlier versions of the project, kept for reference
```

The first rebuilt projects (credit card fraud, stock) also have a multi-notebook version with a `src/` package,
plus a single-file notebook in `kaggle/`. Datasets are never committed; each README says where to get them.

## Clone everything

```bash
git clone --recurse-submodules https://github.com/Pisit-Janthawee/my-repo.git
```
