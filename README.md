## Folder structure for an ML project

ml-project/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│ ├── raw/
│ ├── processed/
│ └── external/
│
├── notebooks/
│ ├── 01_eda.ipynb
│ ├── 02_preprocessing.ipynb
│ ├── 03_model_training.ipynb
│ └── 04_model_evaluation.ipynb
│
├── src/
│ ├── **init**.py
│ │
│ ├── preprocessing/
│ │ ├── **init**.py
│ │ ├── missing_values.py
│ │ ├── outliers.py
│ │ ├── scaling.py
│ │ ├── encoding.py
│ │
│ ├── features/
│ │ ├── **init**.py
│ │ ├── binning.py
│ │ ├── polynomial.py
│ │ ├── text_features.py
│ │
│ ├── eda/
│ │ ├── **init**.py
│ │ ├── summary_stats.py
│ │ ├── correlation.py
│ │ ├── plots.py
│ │
│ ├── models/
│ │ ├── **init**.py
│ │ ├── train_regression.py
│ │ ├── train_classification.py
│ │ ├── train_clustering.py
│ │
│ ├── utils/
│ │ ├── **init**.py
│ │ ├── load_data.py
│ │ ├── save_model.py
│ │ ├── logger.py
│ │
│ ├── pipelines/
│ ├── **init**.py
│ ├── model_pipeline.py
│
├── configs/
│ ├── train_config.yaml
│ ├── model_params.yaml
│
├── models/
│ ├── saved/
│ └── metrics/
│
├── mlruns/ (MLflow placeholder)
│
└── scripts/
├── run_training.py
├── run_pipeline.py
