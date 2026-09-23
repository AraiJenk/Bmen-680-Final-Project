# Skin lesion classification

Course project: **Developing a Machine Learning Approach for Benign and Malignant Skin Lesion Classification using Dermatoscopic Imaging**.

The half-page project draft is in [docs/project-summary.md](docs/project-summary.md). The course submission also requires the group contract as page 1 and the title/summary as page 2 in one PDF.

## Proposed data and approach

- Dataset: [HAM10000 / ISIC Archive](https://api.isic-archive.com/collections/212/) (proposal; confirm with group).
- Task: binary lesion classification. Define class mappings and exclusions in `docs/label-policy.md` before analysis.
- Preprocessing: pandas, NumPy, Pillow/OpenCV.
- Models: scikit-learn feature baseline and PyTorch transfer learning.
- Evaluation: lesion-grouped splits; malignant sensitivity, specificity, precision, F1, ROC-AUC, and confusion matrix.

## Layout

| Path | Purpose |
| --- | --- |
| `docs/` | Project summary, dataset and label decisions |
| `data/raw/` | Downloaded source images and labels (ignored by Git) |
| `data/processed/` | Processed inputs (ignored by Git) |
| `notebooks/` | Exploratory work |
| `src/` | Reusable preprocessing, training, evaluation code |
| `models/` | Model weights (ignored by Git) |
| `results/` | Figures and metric tables |
| `tests/` | Checks for data integrity and splits |

## Next steps

1. Confirm the dataset and binary label mapping with the group.
2. Record provenance and license terms in `docs/dataset.md`; download images into `data/raw/`.
3. Make grouped train/validation/test splits and record class counts.
4. Train a baseline, then compare a pretrained image model on the same held-out test set.

No downloaded dataset or fitted model is included here.
