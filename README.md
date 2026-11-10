# my-repo

Workspace that gathers all my projects in one place, organized by category, plus a
drop-box for notebooks and data that are still in progress.

```
my-repo/
├── projects/                 # each project is a git submodule (its own repo + history)
│   ├── deep-learning/
│   ├── machine-learning/
│   └── web-scraping/
└── project-user-drop-box/    # in-progress notebooks + input data
    ├── kaggle/
    └── local-pc/
```

## Projects

| Category | Project | Last commit |
|---|---|---|
| Deep learning | [dl-binaryclassification-tuberculosis-prediction](https://github.com/Pisit-Janthawee/dl-binaryclassification-tuberculosis-prediction) | 2024-09 |
| Deep learning | [dl-multiclassification-face-recognition](https://github.com/Pisit-Janthawee/dl-multiclassification-face-recognition) | 2023-10 |
| Machine learning | [ml-algorithm-taxonomy](https://github.com/Pisit-Janthawee/ml-algorithm-taxonomy) | 2026-11 |
| Machine learning | [ml-binaryclassification-appendicitis-prediction](https://github.com/Pisit-Janthawee/ml-binaryclassification-appendicitis-prediction) | 2023-11 |
| Machine learning | [ml-binaryclassification-credit-card-transactions-fraud-detection](https://github.com/Pisit-Janthawee/ml-binaryclassification-credit-card-transactions-fraud-detection) | empty, not started |
| Machine learning | [ml-recommendationsystem-steamgame](https://github.com/Pisit-Janthawee/ml-recommendationsystem-steamgame) | 2023-10 |
| Web scraping | [web-scraping-drugbank](https://github.com/Pisit-Janthawee/web-scraping-drugbank) | 2023-06 |
| Web scraping | [web-scraping-jobsdb](https://github.com/Pisit-Janthawee/web-scraping-jobsdb) | 2023-12 |
| Web scraping | [web-scraping-redfin](https://github.com/Pisit-Janthawee/web-scraping-redfin) | 2023-12 |

## Clone everything

```bash
git clone --recurse-submodules https://github.com/Pisit-Janthawee/my-repo.git
```

Work inside a project as usual (`cd projects/...`, commit, push to that project's repo),
then come back to the root and `git add projects/<cat>/<name> && git commit` to record the
new pointer.

> **Windows note:** `ml-recommendationsystem-steamgame` contains a placeholder file at
> `repository /test` (folder name with a trailing space), which Windows can't create.
> Every other file checks out fine. Renaming that folder in the source repo fixes it.
