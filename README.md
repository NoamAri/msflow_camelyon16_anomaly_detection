# msflow_camelyon16_anomaly_detection

Implementation of MSFlow with Glow, SE and FPN for histopathology anomaly detection on Camelyon16.
Includes two specialized models and an XGBoost meta-ensemble.

## Repo layout
notebooks/    Jupyter notebooks for training and analysis
docs/         Final report and paper resources
slides/       Course slides
data/         Placeholder only (do not commit WSI data)
models/       Saved weights or checkpoints (gitignored)

## Quick start
python >= 3.10
pip install -r requirements.txt

# data
Place Camelyon16 patches under data/ as described in docs/DATASET_README.md

# run
Open notebooks in order:
1) notebooks/msflow_camelyon16.ipynb
2) notebooks/msflow_Glow_Focal_Center_margin_Loss_AugThreshold.ipynb
3) notebooks/msflow_Glow_FocalLoss_Center_AugThreshold.ipynb
4) notebooks/msflow_meta_ensemble_tsne.ipynb
