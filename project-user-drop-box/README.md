# project-user-drop-box

Drop zone for in-progress work: notebooks (`.ipynb`) and their input data (`.csv`, etc.).

```
project-user-drop-box/
├── kaggle/      # work from Kaggle (downloaded kernels + competition/dataset files)
└── local-pc/    # work done on this machine
```

## Adding a project

Copy `_template/` and rename it after the project:

```
kaggle/<project-name>/
├── notebooks/   # .ipynb files
├── input/       # raw data: .csv, .parquet, images, ... (not committed, see below)
└── output/      # generated artifacts: submissions, figures, models
```

Tip for Kaggle: `kaggle kernels pull <user>/<kernel> -p notebooks/` and
`kaggle competitions download -c <comp> -p input/` (or `kaggle datasets download`).

## Data is not committed

Everything inside `input/` and `output/` is git-ignored (except `.gitkeep`), because GitHub
rejects files over 100 MB and datasets can be re-downloaded. Note the data source in a
`README.md` inside each project so it can be fetched again.
