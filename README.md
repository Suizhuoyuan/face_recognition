cat > README.md << 'EOF'
# Face Recognition

A face recognition system built for Pattern Recognition (CA2), implementing classical and deep learning methods on the CMU PIE dataset.

## Overview

This project explores face recognition through two parts:
- **Part 1**: Feature extraction using PCA and LDA
- **Part 2**: Classification and clustering using KNN, GMM, SVM, and CNN

## Dataset

This project uses the CMU PIE dataset. You may also use any other face dataset, but images must be organized as follows:
PIE/
├── 1/   (images of subject 1)
├── 2/   (images of subject 2)
└── ...  (up to 68 subjects)

Additionally, 10 personal selfies are required under `SELFIES/` as an extra class. These are not included in this repository for privacy reasons.

## Methods

| Part | Method | Description |
|------|--------|-------------|
| 1 | PCA | Dimensionality reduction, p = 2, 3, 100, 300 |
| 1 | LDA | Supervised feature extraction, p = 2, 3, 10, 20 |
| 2 | KNN | Classification on PCA/LDA features |
| 2 | GMM | Clustering with 2D visualization |
| 2 | SVM | Linear SVM with C = 0.01, 1, 100 |
| 2 | CNN | End-to-end training on raw 32x32 grayscale images |

## Project Structure
Face_Reco/
├── Face_Reco.ipynb    # Main notebook
├── requirements.txt   # Dependencies
├── README.md
├── PIE/               # Dataset (not included)
└── SELFIES/           # Personal photos (not included)

## Requirements

Python 3.12
pip install -r requirements.txt

## Usage

1. Prepare dataset under `PIE/` and selfies under `SELFIES/`
2. Run all cells in order in `Face_Reco.ipynb`

