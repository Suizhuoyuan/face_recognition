# Face Recognition — Pattern Recognition CA2

## Overview
Face recognition using PCA, LDA, KNN, GMM, SVM and CNN
on the CMU PIE dataset combined with personal selfies.

## Dataset
- CMU PIE: 25 randomly selected subjects (from 68 total)
- SELFIES: 10 personal photos (not included, privacy)

Place CMU PIE images under `PIE/` and selfies under `SELFIES/`.

## Methods
| Part | Method | Features |
|------|--------|---------|
| 1 | PCA | p = 2, 3, 100, 300 |
| 1 | LDA | p = 2, 3, 10, 20 |
| 2 | KNN | PCA/LDA features |
| 2 | GMM | Raw, PCA features |
| 2 | SVM | Raw, PCA/LDA features |
| 2 | CNN | Raw 32x32 grayscale |

## Requirements
pip install -r requirements.txt

## Usage
Run all cells in order in the notebook.
